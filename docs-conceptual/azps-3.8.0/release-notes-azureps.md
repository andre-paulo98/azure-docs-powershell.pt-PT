---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: bee24af99da4b36e89cff9852c77214e2e09a542
ms.sourcegitcommit: 6a91b4c545350d316d3cf8c62f384478e3f3ba24
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "81740546"
---
## <a name="380---april-2020"></a><span data-ttu-id="67887-103">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="67887-103">3.8.0 - April 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-104">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-104">Az.Accounts</span></span>
* <span data-ttu-id="67887-105">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="67887-105">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="67887-106">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-106">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-107">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="67887-107">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="67887-108">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="67887-108">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-109">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-109">Az.Cdn</span></span>
* <span data-ttu-id="67887-110">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="67887-110">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-111">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-111">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-112">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="67887-112">Supported Identity, Encryption, UserOwnedStorage</span></span> 

#### <a name="azcompute"></a><span data-ttu-id="67887-113">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-113">Az.Compute</span></span>
* <span data-ttu-id="67887-114">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="67887-114">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="67887-115">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="67887-115">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-116">Az.IotHub</span></span>
* <span data-ttu-id="67887-117">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-117">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="67887-118">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="67887-118">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="67887-119">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="67887-119">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="67887-120">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-120">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="67887-121">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-121">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="67887-122">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="67887-122">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="67887-123">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="67887-123">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="67887-124">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="67887-124">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="67887-125">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-125">New cmdlets are:</span></span>
    - <span data-ttu-id="67887-126">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="67887-126">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="67887-127">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="67887-127">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="67887-128">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="67887-128">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="67887-129">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="67887-129">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="67887-130">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-130">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-131">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-131">Az.KeyVault</span></span>
* <span data-ttu-id="67887-132">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="67887-132">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="67887-133">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="67887-133">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="67887-134">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="67887-134">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="67887-135">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="67887-135">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="67887-136">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="67887-136">Az.Maintenance</span></span>
* <span data-ttu-id="67887-137">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="67887-137">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-138">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-138">Az.Monitor</span></span>
* <span data-ttu-id="67887-139">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="67887-139">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="67887-140">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="67887-140">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="67887-141">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="67887-141">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="67887-142">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="67887-142">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="67887-143">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="67887-143">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="67887-144">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="67887-144">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="67887-145">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="67887-145">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="67887-146">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="67887-146">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-147">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-147">Az.Network</span></span>
* <span data-ttu-id="67887-148">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="67887-148">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="67887-149">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="67887-149">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="67887-150">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="67887-150">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="67887-151">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="67887-151">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="67887-152">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="67887-152">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="67887-153">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="67887-153">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="67887-154">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="67887-154">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="67887-155">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="67887-155">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="67887-156">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="67887-156">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="67887-157">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="67887-157">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="67887-158">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="67887-158">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="67887-159">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="67887-159">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="67887-160">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="67887-160">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="67887-161">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="67887-161">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="67887-162">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="67887-162">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="67887-163">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="67887-163">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-164">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-164">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-165">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="67887-165">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="67887-166">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="67887-166">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-167">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-167">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-168">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="67887-168">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-169">Az.Sql</span></span>
* <span data-ttu-id="67887-170">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="67887-170">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="67887-171">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="67887-171">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-172">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-172">Az.Storage</span></span>
* <span data-ttu-id="67887-173">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="67887-173">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="67887-174">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="67887-174">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="67887-175">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="67887-175">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="67887-176">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="67887-176">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="67887-177">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="67887-177">Supported DataLake Gen2</span></span> 
    - <span data-ttu-id="67887-178">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="67887-178">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="67887-179">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="67887-179">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="67887-180">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="67887-180">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="67887-181">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="67887-181">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="67887-182">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="67887-182">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="67887-183">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="67887-183">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="67887-184">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="67887-184">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="67887-185">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="67887-185">'Remove-AzDataLakeGen2Item'</span></span>

# <a name="azure-powershell-release-notes"></a><span data-ttu-id="67887-186">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="67887-186">Azure PowerShell release notes</span></span>
## <a name="370---march-2020"></a><span data-ttu-id="67887-187">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="67887-187">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-188">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-188">Az.Accounts</span></span>
* <span data-ttu-id="67887-189">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="67887-189">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-190">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-190">Az.Compute</span></span>
* <span data-ttu-id="67887-191">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="67887-191">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span> 
    - <span data-ttu-id="67887-192">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="67887-192">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="67887-193">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="67887-193">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="67887-194">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="67887-194">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="67887-195">[#11354]</span><span class="sxs-lookup"><span data-stu-id="67887-195">[#11354]</span></span>
* <span data-ttu-id="67887-196">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="67887-196">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="67887-197">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="67887-197">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="67887-198">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="67887-198">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="67887-199">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="67887-199">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="67887-200">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="67887-200">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="67887-201">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-201">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="67887-202">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="67887-202">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="67887-203">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="67887-203">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="67887-204">[#11257]</span><span class="sxs-lookup"><span data-stu-id="67887-204">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-205">Az.DataFactory</span></span>
* <span data-ttu-id="67887-206">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="67887-206">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="67887-207">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="67887-207">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-208">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-208">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-209">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="67887-209">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="67887-210">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="67887-210">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="67887-211">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-211">Az.HDInsight</span></span>
* <span data-ttu-id="67887-212">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="67887-212">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-213">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-213">Az.IotHub</span></span>
* <span data-ttu-id="67887-214">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67887-214">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="67887-215">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-215">New Cmdlets are:</span></span>
    - <span data-ttu-id="67887-216">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="67887-216">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="67887-217">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="67887-217">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-218">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-218">Az.KeyVault</span></span>
* <span data-ttu-id="67887-219">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="67887-219">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-220">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-220">Az.Monitor</span></span>
* <span data-ttu-id="67887-221">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="67887-221">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-222">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-222">Az.Network</span></span>
* <span data-ttu-id="67887-223">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="67887-223">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="67887-224">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="67887-224">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="67887-225">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="67887-225">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="67887-226">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="67887-226">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="67887-227">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="67887-227">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="67887-228">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="67887-228">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-229">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-229">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-230">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="67887-230">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-231">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-231">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-232">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-232">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="67887-233">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="67887-233">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="67887-234">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="67887-234">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="67887-235">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="67887-235">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="67887-236">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="67887-236">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="67887-237">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="67887-237">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-238">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-238">Az.Resources</span></span>
* <span data-ttu-id="67887-239">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="67887-239">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="67887-240">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="67887-240">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="67887-241">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="67887-241">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="67887-242">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="67887-242">Added example.</span></span>
* <span data-ttu-id="67887-243">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="67887-243">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="67887-244">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="67887-244">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-245">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-245">Az.Sql</span></span>
* <span data-ttu-id="67887-246">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="67887-246">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="67887-247">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="67887-247">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="67887-248">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="67887-248">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="67887-249">Az.Support</span><span class="sxs-lookup"><span data-stu-id="67887-249">Az.Support</span></span>
* <span data-ttu-id="67887-250">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="67887-250">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-251">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-251">Az.Websites</span></span>
* <span data-ttu-id="67887-252">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="67887-252">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="67887-253">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="67887-253">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="67887-254">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="67887-254">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="67887-255">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="67887-255">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="67887-256">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="67887-256">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="67887-257">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="67887-257">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-258">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-258">Az.Accounts</span></span>
* <span data-ttu-id="67887-259">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="67887-259">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="67887-260">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="67887-260">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="67887-261">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="67887-261">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="67887-262">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-262">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-263">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="67887-263">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="67887-264">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="67887-264">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="67887-265">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="67887-265">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="67887-266">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="67887-266">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-267">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-267">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-268">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="67887-268">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-269">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-269">Az.IotHub</span></span>
* <span data-ttu-id="67887-270">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-270">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="67887-271">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-271">New Cmdlets are:</span></span>
    - <span data-ttu-id="67887-272">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-272">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="67887-273">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-273">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="67887-274">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-274">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="67887-275">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-275">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="67887-276">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-276">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="67887-277">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-277">New Cmdlets are:</span></span>
    - <span data-ttu-id="67887-278">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="67887-278">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="67887-279">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="67887-279">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="67887-280">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="67887-280">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="67887-281">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="67887-281">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="67887-282">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-282">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="67887-283">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-283">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="67887-284">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-284">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="67887-285">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-285">New Cmdlets are:</span></span>
    - <span data-ttu-id="67887-286">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="67887-286">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="67887-287">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="67887-287">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="67887-288">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67887-288">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-289">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-289">Az.Monitor</span></span>
* <span data-ttu-id="67887-290">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="67887-290">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-291">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-291">Az.Network</span></span>
* <span data-ttu-id="67887-292">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="67887-292">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="67887-293">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="67887-293">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="67887-294">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="67887-294">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="67887-295">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="67887-295">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-296">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-296">Az.Resources</span></span>
* <span data-ttu-id="67887-297">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="67887-297">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="67887-298">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="67887-298">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="67887-299">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="67887-299">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="67887-300">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="67887-300">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="67887-301">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="67887-301">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="67887-302">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="67887-302">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="67887-303">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="67887-303">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="67887-304">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="67887-304">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="67887-305">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="67887-305">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="67887-306">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="67887-306">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="67887-307">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="67887-307">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="67887-308">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="67887-308">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="67887-309">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="67887-309">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="67887-310">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="67887-310">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-311">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-311">Az.Sql</span></span>
* <span data-ttu-id="67887-312">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="67887-312">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="67887-313">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="67887-313">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="67887-314">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="67887-314">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="67887-315">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="67887-315">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="67887-316">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="67887-316">Remove an LTR backup</span></span>
    - <span data-ttu-id="67887-317">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="67887-317">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="67887-318">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="67887-318">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="67887-319">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="67887-319">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="67887-320">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-320">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-321">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-321">Az.Storage</span></span>
* <span data-ttu-id="67887-322">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-322">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="67887-323">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="67887-323">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="67887-324">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="67887-324">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="67887-325">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="67887-325">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="67887-326">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="67887-326">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-327">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-327">Az.Websites</span></span>
* <span data-ttu-id="67887-328">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="67887-328">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="67887-329">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="67887-329">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="67887-330">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="67887-330">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="67887-331">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="67887-331">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="67887-332">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="67887-332">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="67887-333">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="67887-333">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="67887-334">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="67887-334">Highlights since the last major release</span></span>
* <span data-ttu-id="67887-335">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="67887-335">Updated client side telemetry.</span></span>
* <span data-ttu-id="67887-336">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="67887-336">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="67887-337">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="67887-337">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-338">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-338">Az.Accounts</span></span>
* <span data-ttu-id="67887-339">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="67887-339">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-340">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-340">Az.Automation</span></span>
* <span data-ttu-id="67887-341">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="67887-341">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-342">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-342">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-343">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="67887-343">Updated SDK to 7.0</span></span>
* <span data-ttu-id="67887-344">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="67887-344">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-345">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-345">Az.Compute</span></span>
* <span data-ttu-id="67887-346">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="67887-346">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="67887-347">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-347">Az.FrontDoor</span></span>
* <span data-ttu-id="67887-348">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="67887-348">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-349">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-349">Az.IotHub</span></span>
* <span data-ttu-id="67887-350">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="67887-350">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="67887-351">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-351">New Cmdlets are:</span></span>
    - <span data-ttu-id="67887-352">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-352">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="67887-353">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-353">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="67887-354">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-354">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="67887-355">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="67887-355">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-356">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-356">Az.KeyVault</span></span>
* <span data-ttu-id="67887-357">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="67887-357">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-358">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-358">Az.Monitor</span></span>
* <span data-ttu-id="67887-359">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="67887-359">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="67887-360">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="67887-360">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="67887-361">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="67887-361">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-362">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-362">Az.Network</span></span>
* <span data-ttu-id="67887-363">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="67887-363">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="67887-364">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="67887-364">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="67887-365">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="67887-365">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="67887-366">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="67887-366">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="67887-367">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="67887-367">No new cmdlets are added.</span></span> <span data-ttu-id="67887-368">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="67887-368">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-369">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-369">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-370">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="67887-370">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-371">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-371">Az.Resources</span></span>
* <span data-ttu-id="67887-372">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="67887-372">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="67887-373">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="67887-373">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="67887-374">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="67887-374">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="67887-375">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="67887-375">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="67887-376">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="67887-376">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="67887-377">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="67887-377">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="67887-378">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="67887-378">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="67887-379">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="67887-379">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-380">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-380">Az.Sql</span></span>
* <span data-ttu-id="67887-381">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="67887-381">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="67887-382">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="67887-382">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="67887-383">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="67887-383">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="67887-384">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="67887-384">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="67887-385">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="67887-385">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="67887-386">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="67887-386">Az.StorageSync</span></span>
* <span data-ttu-id="67887-387">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="67887-387">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="67887-388">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="67887-388">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="67887-389">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="67887-389">Highlights since the last major release</span></span>
* <span data-ttu-id="67887-390">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="67887-390">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="67887-391">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="67887-391">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-392">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-392">Az.Accounts</span></span>
* <span data-ttu-id="67887-393">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="67887-393">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="67887-394">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="67887-394">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="67887-395">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-395">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-396">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="67887-396">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="67887-397">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="67887-397">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="67887-398">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="67887-398">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="67887-399">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="67887-399">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-400">Az.Compute</span></span>
* <span data-ttu-id="67887-401">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="67887-401">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="67887-402">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="67887-402">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="67887-403">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-403">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="67887-404">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="67887-404">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="67887-405">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="67887-405">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-406">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-406">Az.DataFactory</span></span>
* <span data-ttu-id="67887-407">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="67887-407">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="67887-408">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="67887-408">Az.DeploymentManager</span></span>
* <span data-ttu-id="67887-409">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="67887-409">Adds LIST operations for resources</span></span>
* <span data-ttu-id="67887-410">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="67887-410">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="67887-411">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-411">Az.HDInsight</span></span>
* <span data-ttu-id="67887-412">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="67887-412">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-413">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-413">Az.KeyVault</span></span>
* <span data-ttu-id="67887-414">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="67887-414">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-415">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-415">Az.Network</span></span>
* <span data-ttu-id="67887-416">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="67887-416">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="67887-417">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="67887-417">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="67887-418">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="67887-418">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="67887-419">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="67887-419">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="67887-420">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="67887-420">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="67887-421">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="67887-421">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="67887-422">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="67887-422">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="67887-423">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="67887-423">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="67887-424">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-424">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-425">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-425">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="67887-426">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-426">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="67887-427">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="67887-427">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="67887-428">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="67887-428">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-429">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-429">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-430">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="67887-430">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="67887-431">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="67887-431">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="67887-432">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="67887-432">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="67887-433">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="67887-433">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-434">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-434">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-435">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="67887-435">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="67887-436">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="67887-436">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-437">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-437">Az.Resources</span></span>
* <span data-ttu-id="67887-438">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="67887-438">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="67887-439">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="67887-439">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-440">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-440">Az.Sql</span></span>
<span data-ttu-id="67887-441">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="67887-441">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-442">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-442">Az.Storage</span></span>
* <span data-ttu-id="67887-443">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="67887-443">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="67887-444">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-444">New-AzStorageAccount</span></span>
* <span data-ttu-id="67887-445">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="67887-445">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="67887-446">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="67887-446">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-447">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-447">Az.Websites</span></span>
* <span data-ttu-id="67887-448">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="67887-448">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="67887-449">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="67887-449">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="67887-450">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="67887-450">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-451">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-451">Az.Accounts</span></span>
* <span data-ttu-id="67887-452">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="67887-452">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-453">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-453">Az.Cdn</span></span>
* <span data-ttu-id="67887-454">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="67887-454">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-455">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-455">Az.Compute</span></span>
* <span data-ttu-id="67887-456">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="67887-456">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="67887-457">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="67887-457">Az.ContainerInstance</span></span>
* <span data-ttu-id="67887-458">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="67887-458">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="67887-459">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="67887-459">Az.DataBoxEdge</span></span>
* <span data-ttu-id="67887-460">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="67887-460">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="67887-461">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-461">Get the Edge Storage Container</span></span>
* <span data-ttu-id="67887-462">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="67887-462">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="67887-463">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-463">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="67887-464">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="67887-464">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="67887-465">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-465">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="67887-466">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="67887-466">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="67887-467">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-467">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="67887-468">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="67887-468">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="67887-469">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-469">Get the Edge Storage Account</span></span>
* <span data-ttu-id="67887-470">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="67887-470">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="67887-471">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-471">Create new Edge Storage Account</span></span>
* <span data-ttu-id="67887-472">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="67887-472">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="67887-473">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="67887-473">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="67887-474">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="67887-474">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="67887-475">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="67887-475">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="67887-476">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="67887-476">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="67887-477">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="67887-477">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-478">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-478">Az.DataFactory</span></span>
* <span data-ttu-id="67887-479">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="67887-479">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="67887-480">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="67887-480">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="67887-481">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="67887-481">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="67887-482">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="67887-482">Az.DevTestLabs</span></span>
* <span data-ttu-id="67887-483">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="67887-483">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-484">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-484">Az.EventHub</span></span>
* <span data-ttu-id="67887-485">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="67887-485">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="67887-486">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-486">Az.HDInsight</span></span>
* <span data-ttu-id="67887-487">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="67887-487">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="67887-488">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="67887-488">Az.MachineLearning</span></span>
* <span data-ttu-id="67887-489">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="67887-489">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="67887-490">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="67887-490">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="67887-491">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="67887-491">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="67887-492">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="67887-492">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="67887-493">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="67887-493">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="67887-494">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="67887-494">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="67887-495">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="67887-495">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="67887-496">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="67887-496">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-497">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-497">Az.Network</span></span>
* <span data-ttu-id="67887-498">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="67887-498">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-499">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-499">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-500">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-500">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="67887-501">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-501">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="67887-502">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-502">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="67887-503">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-503">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-504">Az.Resources</span></span>
* <span data-ttu-id="67887-505">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="67887-505">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-506">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-506">Az.Sql</span></span>
* <span data-ttu-id="67887-507">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="67887-507">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="67887-508">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="67887-508">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="67887-509">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="67887-509">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="67887-510">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="67887-510">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-511">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-511">Az.Storage</span></span>
* <span data-ttu-id="67887-512">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="67887-512">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="67887-513">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-513">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="67887-514">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="67887-514">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="67887-515">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-515">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="67887-516">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-516">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="67887-517">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-517">General</span></span>
* <span data-ttu-id="67887-518">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="67887-518">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-519">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-519">Az.Accounts</span></span>
* <span data-ttu-id="67887-520">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="67887-520">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="67887-521">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="67887-521">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="67887-522">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="67887-522">Az.Batch</span></span>
* <span data-ttu-id="67887-523">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="67887-523">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-524">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-524">Az.DataFactory</span></span>
* <span data-ttu-id="67887-525">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="67887-525">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="67887-526">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-526">Az.FrontDoor</span></span>
* <span data-ttu-id="67887-527">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="67887-527">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="67887-528">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="67887-528">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="67887-529">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="67887-529">Az.HealthcareApis</span></span>
* <span data-ttu-id="67887-530">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="67887-530">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-531">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-531">Az.KeyVault</span></span>
* <span data-ttu-id="67887-532">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="67887-532">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="67887-533">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="67887-533">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="67887-534">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="67887-534">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-535">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-535">Az.Monitor</span></span>
* <span data-ttu-id="67887-536">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="67887-536">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="67887-537">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="67887-537">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="67887-538">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="67887-538">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-539">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-539">Az.Network</span></span>
* <span data-ttu-id="67887-540">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="67887-540">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-541">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-541">Az.Resources</span></span>
* <span data-ttu-id="67887-542">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="67887-542">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="67887-543">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="67887-543">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-544">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-544">Az.Sql</span></span>
* <span data-ttu-id="67887-545">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="67887-545">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-546">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-546">Az.Storage</span></span>
* <span data-ttu-id="67887-547">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="67887-547">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="67887-548">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="67887-548">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="67887-549">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="67887-549">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="67887-550">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="67887-550">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="67887-551">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="67887-551">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="67887-552">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="67887-552">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="67887-553">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="67887-553">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="67887-554">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="67887-554">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="67887-555">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="67887-555">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="67887-556">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="67887-556">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="67887-557">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="67887-557">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="67887-558">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="67887-558">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="67887-559">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="67887-559">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="67887-560">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-560">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="67887-561">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="67887-561">Highlights since the last major release</span></span>
* <span data-ttu-id="67887-562">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="67887-562">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="67887-563">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="67887-563">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-564">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-564">Az.Compute</span></span>
* <span data-ttu-id="67887-565">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="67887-565">VM Reapply feature</span></span>
    - <span data-ttu-id="67887-566">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="67887-566">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="67887-567">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="67887-567">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="67887-568">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-568">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="67887-569">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="67887-569">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="67887-570">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-570">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="67887-571">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="67887-571">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="67887-572">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="67887-572">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="67887-573">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="67887-573">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="67887-574">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="67887-574">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="67887-575">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-575">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="67887-576">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="67887-576">Az.DataBoxEdge</span></span>
* <span data-ttu-id="67887-577">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="67887-577">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="67887-578">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="67887-578">Get the Order</span></span>
* <span data-ttu-id="67887-579">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="67887-579">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="67887-580">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="67887-580">Create new Order</span></span>
* <span data-ttu-id="67887-581">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="67887-581">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="67887-582">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="67887-582">Remove the Order</span></span>
* <span data-ttu-id="67887-583">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="67887-583">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="67887-584">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="67887-584">Now creates Local Share</span></span>
* <span data-ttu-id="67887-585">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="67887-585">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="67887-586">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="67887-586">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="67887-587">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="67887-587">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="67887-588">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="67887-588">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="67887-589">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="67887-589">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="67887-590">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="67887-590">Gets the information about Triggers</span></span>
* <span data-ttu-id="67887-591">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="67887-591">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="67887-592">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="67887-592">Create new Triggers</span></span>
* <span data-ttu-id="67887-593">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="67887-593">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="67887-594">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="67887-594">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-595">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-595">Az.DataFactory</span></span>
* <span data-ttu-id="67887-596">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="67887-596">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="67887-597">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="67887-597">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-598">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-598">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-599">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="67887-599">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-600">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-600">Az.EventHub</span></span>
* <span data-ttu-id="67887-601">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="67887-601">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="67887-602">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-602">Az.FrontDoor</span></span>
* <span data-ttu-id="67887-603">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="67887-603">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="67887-604">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="67887-604">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="67887-605">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="67887-605">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="67887-606">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="67887-606">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-607">Az.Network</span></span>
* <span data-ttu-id="67887-608">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="67887-608">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="67887-609">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="67887-609">Az.PrivateDns</span></span>
* <span data-ttu-id="67887-610">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="67887-610">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-611">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-611">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-612">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="67887-612">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="67887-613">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="67887-613">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="67887-614">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="67887-614">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="67887-615">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="67887-615">Az.RedisCache</span></span>
* <span data-ttu-id="67887-616">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="67887-616">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="67887-617">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="67887-617">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="67887-618">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="67887-618">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-619">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-619">Az.Resources</span></span>
- <span data-ttu-id="67887-620">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="67887-620">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="67887-621">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="67887-621">Updated create policy definition help example</span></span>
- <span data-ttu-id="67887-622">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="67887-622">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="67887-623">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="67887-623">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="67887-624">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="67887-624">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-625">Az.Sql</span></span>
* <span data-ttu-id="67887-626">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="67887-626">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="67887-627">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="67887-627">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="67887-628">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-628">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="67887-629">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-629">General</span></span>
* <span data-ttu-id="67887-630">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="67887-630">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-631">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-631">Az.Accounts</span></span>
* <span data-ttu-id="67887-632">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="67887-632">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="67887-633">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="67887-633">Az.Advisor</span></span>
* <span data-ttu-id="67887-634">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="67887-634">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="67887-635">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="67887-635">Az.Batch</span></span>
* <span data-ttu-id="67887-636">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="67887-636">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="67887-637">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="67887-637">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="67887-638">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="67887-638">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="67887-639">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="67887-639">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="67887-640">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="67887-640">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="67887-641">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="67887-641">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="67887-642">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="67887-642">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="67887-643">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="67887-643">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="67887-644">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="67887-644">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="67887-645">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="67887-645">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="67887-646">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="67887-646">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="67887-647">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="67887-647">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="67887-648">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="67887-648">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="67887-649">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="67887-649">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="67887-650">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="67887-650">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="67887-651">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="67887-651">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="67887-652">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="67887-652">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="67887-653">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="67887-653">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="67887-654">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="67887-654">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="67887-655">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="67887-655">This operation is no longer supported.</span></span>
* <span data-ttu-id="67887-656">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="67887-656">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="67887-657">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="67887-657">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="67887-658">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="67887-658">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="67887-659">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="67887-659">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="67887-660">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="67887-660">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="67887-661">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="67887-661">New non-verified images are also now returned.</span></span> <span data-ttu-id="67887-662">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="67887-662">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="67887-663">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="67887-663">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="67887-664">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="67887-664">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="67887-665">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="67887-665">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="67887-666">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="67887-666">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="67887-667">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="67887-667">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="67887-668">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="67887-668">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="67887-669">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="67887-669">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="67887-670">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="67887-670">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="67887-671">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="67887-671">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-672">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-672">Az.Cdn</span></span>
* <span data-ttu-id="67887-673">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="67887-673">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="67887-674">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="67887-674">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-675">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-675">Az.Compute</span></span>
* <span data-ttu-id="67887-676">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="67887-676">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="67887-677">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="67887-677">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="67887-678">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="67887-678">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="67887-679">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="67887-679">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="67887-680">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="67887-680">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="67887-681">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="67887-681">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="67887-682">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-682">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="67887-683">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="67887-683">Breaking changes</span></span>
    - <span data-ttu-id="67887-684">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="67887-684">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="67887-685">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="67887-685">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-686">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-686">Az.DataFactory</span></span>
* <span data-ttu-id="67887-687">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="67887-687">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-688">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-688">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-689">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="67887-689">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="67887-690">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="67887-690">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="67887-691">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="67887-691">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="67887-692">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="67887-692">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="67887-693">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="67887-693">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="67887-694">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="67887-694">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="67887-695">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-695">Az.FrontDoor</span></span>
* <span data-ttu-id="67887-696">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="67887-696">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="67887-697">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-697">Az.HDInsight</span></span>
* <span data-ttu-id="67887-698">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="67887-698">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="67887-699">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="67887-699">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="67887-700">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="67887-700">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="67887-701">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-701">Removed five cmdlets:</span></span>
    - <span data-ttu-id="67887-702">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="67887-702">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="67887-703">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="67887-703">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="67887-704">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="67887-704">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="67887-705">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="67887-705">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="67887-706">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="67887-706">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="67887-707">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-707">Added three cmdlets:</span></span>
    - <span data-ttu-id="67887-708">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="67887-708">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="67887-709">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="67887-709">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="67887-710">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="67887-710">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="67887-711">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="67887-711">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="67887-712">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="67887-712">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="67887-713">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="67887-713">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="67887-714">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-714">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="67887-715">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="67887-715">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="67887-716">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="67887-716">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="67887-717">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="67887-717">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="67887-718">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="67887-718">Added some scenario test cases.</span></span>
* <span data-ttu-id="67887-719">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="67887-719">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-720">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-720">Az.IotHub</span></span>
* <span data-ttu-id="67887-721">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="67887-721">Breaking changes:</span></span>
    - <span data-ttu-id="67887-722">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="67887-722">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="67887-723">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="67887-723">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="67887-724">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="67887-724">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="67887-725">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="67887-725">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="67887-726">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="67887-726">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="67887-727">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="67887-727">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="67887-728">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="67887-728">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="67887-729">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="67887-729">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="67887-730">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="67887-730">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="67887-731">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="67887-731">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="67887-732">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="67887-732">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="67887-733">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="67887-733">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-734">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-734">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-735">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-735">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="67887-736">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-736">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="67887-737">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-737">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="67887-738">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-738">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="67887-739">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-739">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="67887-740">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-740">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="67887-741">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-741">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="67887-742">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-742">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="67887-743">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="67887-743">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-744">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-744">Az.Resources</span></span>
* <span data-ttu-id="67887-745">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="67887-745">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-746">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-746">Az.Network</span></span>
* <span data-ttu-id="67887-747">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="67887-747">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="67887-748">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="67887-748">Updated cmdlet:</span></span>
        - <span data-ttu-id="67887-749">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-749">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-750">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-750">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-751">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-751">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-752">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-752">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-753">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-753">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="67887-754">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="67887-754">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="67887-755">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="67887-755">New cmdlet:</span></span>
        - <span data-ttu-id="67887-756">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="67887-756">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="67887-757">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="67887-757">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="67887-758">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-758">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="67887-759">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-759">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="67887-760">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="67887-760">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="67887-761">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="67887-761">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="67887-762">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-762">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="67887-763">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="67887-763">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="67887-764">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-764">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-765">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="67887-765">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="67887-766">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="67887-766">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="67887-767">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="67887-767">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="67887-768">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="67887-768">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="67887-769">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="67887-769">Set-AzVirtualHub</span></span>
* <span data-ttu-id="67887-770">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="67887-770">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="67887-771">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="67887-771">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="67887-772">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="67887-772">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="67887-773">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="67887-773">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="67887-774">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="67887-774">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="67887-775">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="67887-775">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="67887-776">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="67887-776">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="67887-777">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-777">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-778">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="67887-778">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="67887-779">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="67887-779">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="67887-780">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="67887-780">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="67887-781">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="67887-781">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="67887-782">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="67887-782">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="67887-783">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="67887-783">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="67887-784">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="67887-784">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="67887-785">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="67887-785">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="67887-786">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-786">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-787">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="67887-787">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="67887-788">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="67887-788">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="67887-789">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="67887-789">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="67887-790">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="67887-790">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="67887-791">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="67887-791">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="67887-792">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-792">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="67887-793">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="67887-793">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="67887-794">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="67887-794">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="67887-795">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="67887-795">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="67887-796">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="67887-796">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="67887-797">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="67887-797">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="67887-798">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="67887-798">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="67887-799">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="67887-799">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="67887-800">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="67887-800">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="67887-801">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="67887-801">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="67887-802">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="67887-802">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="67887-803">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="67887-803">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="67887-804">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-804">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-805">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="67887-805">New-AzIpGroup</span></span>
        - <span data-ttu-id="67887-806">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="67887-806">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="67887-807">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="67887-807">Get-AzIpGroup</span></span>
        - <span data-ttu-id="67887-808">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="67887-808">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-809">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-809">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-810">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="67887-810">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-811">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-811">Az.Sql</span></span>
* <span data-ttu-id="67887-812">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="67887-812">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="67887-813">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="67887-813">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="67887-814">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="67887-814">Removed deprecated aliases:</span></span>
* <span data-ttu-id="67887-815">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="67887-815">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="67887-816">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="67887-816">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="67887-817">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-817">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="67887-818">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="67887-818">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="67887-819">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="67887-819">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="67887-820">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="67887-820">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-821">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-821">Az.Storage</span></span>
* <span data-ttu-id="67887-822">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="67887-822">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="67887-823">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-823">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="67887-824">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-824">Set-AzStorageAccount</span></span>
* <span data-ttu-id="67887-825">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="67887-825">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="67887-826">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="67887-826">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="67887-827">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="67887-827">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="67887-828">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-828">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="67887-829">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-829">General</span></span>
* <span data-ttu-id="67887-830">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="67887-830">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-831">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-831">Az.Accounts</span></span>
* <span data-ttu-id="67887-832">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="67887-832">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="67887-833">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-833">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-834">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="67887-834">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="67887-835">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="67887-835">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-836">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-836">Az.Automation</span></span>
* <span data-ttu-id="67887-837">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="67887-837">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="67887-838">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="67887-838">Az.Batch</span></span>
* <span data-ttu-id="67887-839">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="67887-839">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-840">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-840">Az.Compute</span></span>
* <span data-ttu-id="67887-841">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-841">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="67887-842">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="67887-842">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="67887-843">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="67887-843">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="67887-844">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="67887-844">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-845">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-845">Az.DataFactory</span></span>
* <span data-ttu-id="67887-846">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="67887-846">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="67887-847">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="67887-847">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="67887-848">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="67887-848">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-849">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-849">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-850">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="67887-850">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="67887-851">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="67887-851">Az.HealthcareApis</span></span>
* <span data-ttu-id="67887-852">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="67887-852">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="67887-853">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="67887-853">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="67887-854">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="67887-854">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="67887-855">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="67887-855">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-856">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-856">Az.IotHub</span></span>
* <span data-ttu-id="67887-857">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="67887-857">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="67887-858">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="67887-858">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-859">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-859">Az.Monitor</span></span>
* <span data-ttu-id="67887-860">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="67887-860">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="67887-861">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="67887-861">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="67887-862">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="67887-862">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="67887-863">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="67887-863">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-864">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-864">Az.Network</span></span>
* <span data-ttu-id="67887-865">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="67887-865">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="67887-866">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="67887-866">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="67887-867">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-867">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-868">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-868">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="67887-869">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="67887-869">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="67887-870">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="67887-870">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="67887-871">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="67887-871">Updated cmdlets:</span></span>
        - <span data-ttu-id="67887-872">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-872">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="67887-873">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-873">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="67887-874">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-874">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="67887-875">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="67887-875">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="67887-876">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="67887-876">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="67887-877">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="67887-877">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="67887-878">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="67887-878">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="67887-879">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="67887-879">Az.RedisCache</span></span>
* <span data-ttu-id="67887-880">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="67887-880">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-881">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-881">Az.Sql</span></span>
* <span data-ttu-id="67887-882">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="67887-882">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-883">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-883">Az.Storage</span></span>
* <span data-ttu-id="67887-884">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="67887-884">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="67887-885">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="67887-885">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="67887-886">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="67887-886">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="67887-887">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="67887-887">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="67887-888">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-888">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="67887-889">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="67887-889">Az.StorageSync</span></span>
* <span data-ttu-id="67887-890">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="67887-890">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-891">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-891">Az.Websites</span></span>
* <span data-ttu-id="67887-892">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="67887-892">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="67887-893">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-893">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="67887-894">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-894">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-895">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="67887-895">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="67887-896">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="67887-896">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="67887-897">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="67887-897">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-898">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-898">Az.Automation</span></span>
* <span data-ttu-id="67887-899">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="67887-899">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="67887-900">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="67887-900">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="67887-901">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="67887-901">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-902">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-902">Az.Compute</span></span>
* <span data-ttu-id="67887-903">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="67887-903">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="67887-904">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="67887-904">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="67887-905">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="67887-905">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="67887-906">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="67887-906">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="67887-907">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="67887-907">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="67887-908">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="67887-908">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="67887-909">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="67887-909">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="67887-910">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="67887-910">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="67887-911">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="67887-911">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-912">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-912">Az.DataFactory</span></span>
* <span data-ttu-id="67887-913">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="67887-913">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="67887-914">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="67887-914">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="67887-915">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-915">Az.HDInsight</span></span>
* <span data-ttu-id="67887-916">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="67887-916">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-917">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-917">Az.IotHub</span></span>
* <span data-ttu-id="67887-918">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="67887-918">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="67887-919">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="67887-919">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="67887-920">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="67887-920">New cmdlets are:</span></span>
    - <span data-ttu-id="67887-921">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="67887-921">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="67887-922">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="67887-922">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="67887-923">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="67887-923">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="67887-924">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="67887-924">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-925">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-925">Az.Monitor</span></span>
* <span data-ttu-id="67887-926">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="67887-926">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="67887-927">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="67887-927">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="67887-928">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="67887-928">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="67887-929">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="67887-929">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="67887-930">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="67887-930">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="67887-931">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="67887-931">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="67887-932">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="67887-932">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="67887-933">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="67887-933">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="67887-934">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="67887-934">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="67887-935">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="67887-935">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="67887-936">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="67887-936">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="67887-937">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="67887-937">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="67887-938">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="67887-938">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="67887-939">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="67887-939">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="67887-940">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="67887-940">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="67887-941">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="67887-941">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="67887-942">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="67887-942">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="67887-943">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-943">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="67887-944">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="67887-944">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="67887-945">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-945">Overall improved help files</span></span>
* <span data-ttu-id="67887-946">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="67887-946">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-947">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-947">Az.Network</span></span>
* <span data-ttu-id="67887-948">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="67887-948">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="67887-949">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="67887-949">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="67887-950">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="67887-950">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="67887-951">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="67887-951">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="67887-952">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="67887-952">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="67887-953">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="67887-953">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="67887-954">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="67887-954">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="67887-955">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="67887-955">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="67887-956">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-956">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="67887-957">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="67887-957">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="67887-958">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="67887-958">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="67887-959">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="67887-959">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="67887-960">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-960">New cmdlets</span></span>
        - <span data-ttu-id="67887-961">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="67887-961">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="67887-962">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="67887-962">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="67887-963">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="67887-963">Updated cmdlet:</span></span>
        - <span data-ttu-id="67887-964">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="67887-964">New-VpnSite</span></span>
        - <span data-ttu-id="67887-965">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="67887-965">Update-VpnSite</span></span>
        - <span data-ttu-id="67887-966">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="67887-966">New-VpnConnection</span></span>
        - <span data-ttu-id="67887-967">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="67887-967">Update-VpnConnection</span></span>
* <span data-ttu-id="67887-968">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="67887-968">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-969">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-969">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-970">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="67887-970">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="67887-971">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="67887-971">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-972">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-972">Az.Resources</span></span>
* <span data-ttu-id="67887-973">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="67887-973">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-974">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-974">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-975">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="67887-975">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="67887-976">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="67887-976">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="67887-977">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="67887-977">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="67887-978">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="67887-978">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="67887-979">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="67887-979">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="67887-980">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="67887-980">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="67887-981">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="67887-981">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="67887-982">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="67887-982">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="67887-983">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="67887-983">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="67887-984">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="67887-984">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="67887-985">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="67887-985">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="67887-986">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="67887-986">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="67887-987">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="67887-987">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="67887-988">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="67887-988">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="67887-989">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="67887-989">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="67887-990">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="67887-990">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="67887-991">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="67887-991">Az.SignalR</span></span>
* <span data-ttu-id="67887-992">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="67887-992">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-993">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-993">Az.Sql</span></span>
* <span data-ttu-id="67887-994">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="67887-994">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="67887-995">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="67887-995">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="67887-996">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-996">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="67887-997">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="67887-997">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="67887-998">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="67887-998">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-999">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-999">Az.Storage</span></span>
* <span data-ttu-id="67887-1000">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="67887-1000">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="67887-1001">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="67887-1001">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="67887-1002">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="67887-1002">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="67887-1003">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="67887-1003">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="67887-1004">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="67887-1004">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="67887-1005">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="67887-1005">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="67887-1006">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="67887-1006">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="67887-1007">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="67887-1007">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="67887-1008">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="67887-1008">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="67887-1009">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="67887-1009">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="67887-1010">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="67887-1010">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1011">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1011">Az.Websites</span></span>
* <span data-ttu-id="67887-1012">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="67887-1012">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="67887-1013">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="67887-1013">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="67887-1014">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="67887-1014">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="67887-1015">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1015">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="67887-1016">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-1016">General</span></span>
* <span data-ttu-id="67887-1017">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="67887-1017">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-1018">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1018">Az.Accounts</span></span>
* <span data-ttu-id="67887-1019">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="67887-1019">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="67887-1020">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="67887-1020">Az.Aks</span></span>
* <span data-ttu-id="67887-1021">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="67887-1021">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="67887-1022">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="67887-1022">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="67887-1023">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-1023">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-1024">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="67887-1024">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="67887-1025">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="67887-1025">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="67887-1026">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="67887-1026">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="67887-1027">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="67887-1027">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="67887-1028">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="67887-1028">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="67887-1029">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="67887-1029">Az.Batch</span></span>
* <span data-ttu-id="67887-1030">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="67887-1030">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-1031">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-1031">Az.Cdn</span></span>
* <span data-ttu-id="67887-1032">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="67887-1032">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1033">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1033">Az.Compute</span></span>
* <span data-ttu-id="67887-1034">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1034">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="67887-1035">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-1035">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="67887-1036">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="67887-1036">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="67887-1037">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="67887-1037">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="67887-1038">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="67887-1038">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="67887-1039">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="67887-1039">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="67887-1040">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="67887-1040">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="67887-1041">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="67887-1041">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1042">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1042">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1043">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="67887-1043">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="67887-1044">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="67887-1044">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="67887-1045">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="67887-1045">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="67887-1046">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="67887-1046">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-1047">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-1047">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-1048">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="67887-1048">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-1049">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-1049">Az.EventHub</span></span>
* <span data-ttu-id="67887-1050">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-1050">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="67887-1051">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="67887-1051">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="67887-1052">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="67887-1052">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="67887-1053">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="67887-1053">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="67887-1054">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="67887-1054">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="67887-1055">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="67887-1055">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-1056">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-1056">Az.Monitor</span></span>
* <span data-ttu-id="67887-1057">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-1057">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1058">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1058">Az.Network</span></span>
* <span data-ttu-id="67887-1059">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="67887-1059">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="67887-1060">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="67887-1060">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="67887-1061">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="67887-1061">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="67887-1062">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="67887-1062">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="67887-1063">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="67887-1063">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="67887-1064">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="67887-1064">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="67887-1065">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="67887-1065">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="67887-1066">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1066">Az.OperationalInsights</span></span>
* <span data-ttu-id="67887-1067">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="67887-1067">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="67887-1068">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="67887-1068">Added example</span></span>
    - <span data-ttu-id="67887-1069">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="67887-1069">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="67887-1070">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="67887-1070">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="67887-1071">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="67887-1071">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1072">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1072">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1073">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1073">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1074">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1074">Az.Resources</span></span>
* <span data-ttu-id="67887-1075">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="67887-1075">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="67887-1076">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="67887-1076">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="67887-1077">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="67887-1077">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="67887-1078">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-1078">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="67887-1079">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="67887-1079">Az.ServiceBus</span></span>
* <span data-ttu-id="67887-1080">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-1080">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="67887-1081">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="67887-1081">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="67887-1082">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="67887-1082">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-1083">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-1083">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-1084">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="67887-1084">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="67887-1085">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="67887-1085">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="67887-1086">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="67887-1086">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="67887-1087">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="67887-1087">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="67887-1088">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="67887-1088">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="67887-1089">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="67887-1089">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1090">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1090">Az.Sql</span></span>
* <span data-ttu-id="67887-1091">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="67887-1091">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1092">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1092">Az.Storage</span></span>
* <span data-ttu-id="67887-1093">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="67887-1093">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="67887-1094">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="67887-1094">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="67887-1095">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="67887-1095">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="67887-1096">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="67887-1096">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="67887-1097">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="67887-1097">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="67887-1098">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="67887-1098">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1099">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1099">Az.Websites</span></span>
* <span data-ttu-id="67887-1100">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="67887-1100">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="67887-1101">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1101">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1102">Az.Accounts</span></span>
* <span data-ttu-id="67887-1103">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="67887-1103">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="67887-1104">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1104">Az.ApplicationInsights</span></span>
* <span data-ttu-id="67887-1105">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="67887-1105">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1106">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1106">Az.Automation</span></span>
* <span data-ttu-id="67887-1107">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="67887-1107">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-1108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-1108">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-1109">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="67887-1109">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1110">Az.Compute</span></span>
* <span data-ttu-id="67887-1111">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="67887-1111">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="67887-1112">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="67887-1112">Az.ContainerRegistry</span></span>
* <span data-ttu-id="67887-1113">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="67887-1113">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="67887-1114">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="67887-1114">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1115">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1115">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1116">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="67887-1116">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="67887-1117">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="67887-1117">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-1118">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-1118">Az.EventHub</span></span>
* <span data-ttu-id="67887-1119">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="67887-1119">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="67887-1120">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="67887-1120">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-1121">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-1121">Az.KeyVault</span></span>
* <span data-ttu-id="67887-1122">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="67887-1122">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="67887-1123">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="67887-1123">Az.LogicApp</span></span>
* <span data-ttu-id="67887-1124">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="67887-1124">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="67887-1125">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="67887-1125">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="67887-1126">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="67887-1126">Az.ManagedServices</span></span>
* <span data-ttu-id="67887-1127">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="67887-1127">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1128">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1128">Az.Network</span></span>
* <span data-ttu-id="67887-1129">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="67887-1129">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="67887-1130">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1130">New cmdlets</span></span>
        - <span data-ttu-id="67887-1131">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="67887-1131">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="67887-1132">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-1132">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="67887-1133">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1133">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-1134">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1134">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-1135">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1135">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-1136">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1136">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="67887-1137">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="67887-1137">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="67887-1138">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-1138">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="67887-1139">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="67887-1139">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="67887-1140">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1140">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="67887-1141">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="67887-1141">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="67887-1142">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="67887-1142">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="67887-1143">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="67887-1143">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="67887-1144">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="67887-1144">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="67887-1145">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="67887-1145">Updated cmdlets</span></span>
        - <span data-ttu-id="67887-1146">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1146">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="67887-1147">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1147">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="67887-1148">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1148">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="67887-1149">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1149">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="67887-1150">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1150">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="67887-1151">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="67887-1151">Updated cmdlet:</span></span>
        - <span data-ttu-id="67887-1152">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1152">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="67887-1153">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1153">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="67887-1154">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1154">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="67887-1155">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="67887-1155">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="67887-1156">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="67887-1156">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="67887-1157">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="67887-1157">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="67887-1158">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1158">Az.OperationalInsights</span></span>
* <span data-ttu-id="67887-1159">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="67887-1159">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="67887-1160">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="67887-1160">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1161">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1162">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1162">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="67887-1163">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1163">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="67887-1164">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1164">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="67887-1165">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1165">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="67887-1166">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1166">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="67887-1167">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1167">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="67887-1168">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1168">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="67887-1169">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1169">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="67887-1170">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1170">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="67887-1171">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="67887-1171">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1172">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1172">Az.Resources</span></span>
- <span data-ttu-id="67887-1173">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="67887-1173">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="67887-1174">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="67887-1174">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="67887-1175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="67887-1175">Az.ServiceBus</span></span>
* <span data-ttu-id="67887-1176">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="67887-1176">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="67887-1177">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="67887-1177">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1178">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1178">Az.Sql</span></span>
* <span data-ttu-id="67887-1179">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="67887-1179">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="67887-1180">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="67887-1180">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="67887-1181">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="67887-1181">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1182">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1182">Az.Storage</span></span>
* <span data-ttu-id="67887-1183">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="67887-1183">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="67887-1184">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="67887-1184">Az.StorageSync</span></span>
* <span data-ttu-id="67887-1185">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="67887-1185">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="67887-1186">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="67887-1186">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1187">Az.Websites</span></span>
* <span data-ttu-id="67887-1188">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="67887-1188">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="67887-1189">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="67887-1189">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="67887-1190">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="67887-1190">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="67887-1191">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1191">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1192">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1192">Az.Accounts</span></span>
* <span data-ttu-id="67887-1193">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="67887-1193">Add support for profile cmdlets</span></span>
* <span data-ttu-id="67887-1194">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="67887-1194">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="67887-1195">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="67887-1195">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="67887-1196">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="67887-1196">Az.Advisor</span></span>
* <span data-ttu-id="67887-1197">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="67887-1197">GA release of Az.Advisor</span></span>
* <span data-ttu-id="67887-1198">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="67887-1198">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="67887-1199">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-1199">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-1200">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="67887-1200">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="67887-1201">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="67887-1201">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="67887-1202">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="67887-1202">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="67887-1203">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="67887-1203">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="67887-1204">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="67887-1204">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="67887-1205">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="67887-1205">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="67887-1206">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="67887-1206">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1207">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1207">Az.Automation</span></span>
* <span data-ttu-id="67887-1208">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="67887-1208">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1209">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1209">Az.Compute</span></span>
* <span data-ttu-id="67887-1210">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1210">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1211">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1211">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1212">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="67887-1212">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="67887-1213">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="67887-1213">Az.EventGrid</span></span>
* <span data-ttu-id="67887-1214">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="67887-1214">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-1215">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-1215">Az.IotHub</span></span>
* <span data-ttu-id="67887-1216">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="67887-1216">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1217">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1217">Az.Network</span></span>
* <span data-ttu-id="67887-1218">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="67887-1218">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="67887-1219">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="67887-1219">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-1220">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1220">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-1221">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="67887-1221">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="67887-1222">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="67887-1222">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="67887-1223">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1223">Az.OperationalInsights</span></span>
* <span data-ttu-id="67887-1224">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="67887-1224">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1225">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1225">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1226">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="67887-1226">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1227">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1227">Az.Resources</span></span>
    - <span data-ttu-id="67887-1228">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="67887-1228">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="67887-1229">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="67887-1229">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="67887-1230">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="67887-1230">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="67887-1231">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="67887-1231">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="67887-1232">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="67887-1232">Az.ServiceBus</span></span>
* <span data-ttu-id="67887-1233">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="67887-1233">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1234">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1234">Az.Sql</span></span>
* <span data-ttu-id="67887-1235">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="67887-1235">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="67887-1236">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="67887-1236">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="67887-1237">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="67887-1237">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="67887-1238">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="67887-1238">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="67887-1239">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="67887-1239">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="67887-1240">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="67887-1240">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="67887-1241">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="67887-1241">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="67887-1242">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="67887-1242">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="67887-1243">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="67887-1243">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1244">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1244">Az.Storage</span></span>
* <span data-ttu-id="67887-1245">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="67887-1245">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="67887-1246">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="67887-1246">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="67887-1247">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="67887-1247">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="67887-1248">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="67887-1248">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="67887-1249">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1249">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="67887-1250">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1250">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="67887-1251">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1251">Set-AzStorageAccount</span></span>
* <span data-ttu-id="67887-1252">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="67887-1252">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="67887-1253">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="67887-1253">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="67887-1254">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="67887-1254">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="67887-1255">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="67887-1255">Az.StorageSync</span></span>
* <span data-ttu-id="67887-1256">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="67887-1256">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="67887-1257">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1257">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1258">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1258">Az.Accounts</span></span>
* <span data-ttu-id="67887-1259">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="67887-1259">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="67887-1260">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="67887-1260">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="67887-1261">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="67887-1261">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="67887-1262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="67887-1262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="67887-1263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="67887-1263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1264">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1264">Az.Compute</span></span>
* <span data-ttu-id="67887-1265">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="67887-1265">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="67887-1266">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="67887-1266">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="67887-1267">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="67887-1267">Az.Dns</span></span>
* <span data-ttu-id="67887-1268">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="67887-1268">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="67887-1269">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="67887-1269">Az.EventGrid</span></span>
* <span data-ttu-id="67887-1270">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="67887-1270">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="67887-1271">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-1271">New cmdlets:</span></span>
    - <span data-ttu-id="67887-1272">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="67887-1272">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="67887-1273">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="67887-1273">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="67887-1274">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="67887-1274">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="67887-1275">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-1275">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="67887-1276">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="67887-1276">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="67887-1277">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="67887-1277">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="67887-1278">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="67887-1278">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="67887-1279">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="67887-1279">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="67887-1280">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="67887-1280">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="67887-1281">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="67887-1281">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="67887-1282">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="67887-1282">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="67887-1283">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="67887-1283">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="67887-1284">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="67887-1284">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="67887-1285">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="67887-1285">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="67887-1286">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="67887-1286">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="67887-1287">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="67887-1287">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="67887-1288">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="67887-1288">Updated cmdlets:</span></span>
    - <span data-ttu-id="67887-1289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="67887-1289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="67887-1290">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="67887-1290">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="67887-1291">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="67887-1291">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="67887-1292">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="67887-1292">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="67887-1293">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="67887-1293">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="67887-1294">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="67887-1294">Event subscription expiration date,</span></span>
            - <span data-ttu-id="67887-1295">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="67887-1295">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="67887-1296">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="67887-1296">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="67887-1297">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="67887-1297">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="67887-1298">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="67887-1298">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="67887-1299">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="67887-1299">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="67887-1300">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="67887-1300">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="67887-1301">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="67887-1301">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="67887-1302">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="67887-1302">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="67887-1303">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-1303">Az.FrontDoor</span></span>
* <span data-ttu-id="67887-1304">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="67887-1304">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="67887-1305">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="67887-1305">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="67887-1306">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="67887-1306">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="67887-1307">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="67887-1307">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1308">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1308">Az.Network</span></span>
* <span data-ttu-id="67887-1309">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="67887-1309">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="67887-1310">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1310">New cmdlets</span></span>
        - <span data-ttu-id="67887-1311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="67887-1311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="67887-1312">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="67887-1312">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="67887-1313">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1313">New cmdlets</span></span>
        - <span data-ttu-id="67887-1314">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="67887-1314">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="67887-1315">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-1315">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="67887-1316">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1316">New cmdlets</span></span>
        - <span data-ttu-id="67887-1317">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-1317">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="67887-1318">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-1318">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="67887-1319">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="67887-1319">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="67887-1320">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1320">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="67887-1321">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1321">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="67887-1322">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="67887-1322">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="67887-1323">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1323">New cmdlets</span></span>
        - <span data-ttu-id="67887-1324">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="67887-1324">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="67887-1325">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="67887-1325">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="67887-1326">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="67887-1326">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="67887-1327">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1327">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="67887-1328">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="67887-1328">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="67887-1329">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="67887-1329">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="67887-1330">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="67887-1330">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="67887-1331">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="67887-1331">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="67887-1332">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="67887-1332">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="67887-1333">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="67887-1333">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="67887-1334">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1334">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="67887-1335">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="67887-1335">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="67887-1336">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1336">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="67887-1337">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="67887-1337">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="67887-1338">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="67887-1338">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="67887-1339">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="67887-1339">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="67887-1340">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="67887-1340">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="67887-1341">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="67887-1341">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="67887-1342">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="67887-1342">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="67887-1343">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="67887-1343">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="67887-1344">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="67887-1344">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="67887-1345">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="67887-1345">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="67887-1346">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="67887-1346">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="67887-1347">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="67887-1347">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="67887-1348">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1348">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="67887-1349">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1349">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="67887-1350">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1350">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="67887-1351">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1351">Az.OperationalInsights</span></span>
* <span data-ttu-id="67887-1352">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="67887-1352">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1353">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1353">Az.Resources</span></span>
* <span data-ttu-id="67887-1354">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="67887-1354">Support for additional Template Export options</span></span>
    - <span data-ttu-id="67887-1355">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="67887-1355">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="67887-1356">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="67887-1356">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="67887-1357">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="67887-1357">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-1358">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-1358">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-1359">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="67887-1359">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1360">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1360">Az.Sql</span></span>
* <span data-ttu-id="67887-1361">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="67887-1361">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="67887-1362">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="67887-1362">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="67887-1363">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="67887-1363">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="67887-1364">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="67887-1364">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="67887-1365">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="67887-1365">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="67887-1366">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="67887-1366">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="67887-1367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="67887-1367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="67887-1368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="67887-1368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1369">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1369">Az.Storage</span></span>
* <span data-ttu-id="67887-1370">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="67887-1370">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="67887-1371">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1371">New-AzStorageAccount</span></span>
* <span data-ttu-id="67887-1372">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="67887-1372">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="67887-1373">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1373">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1374">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1374">Az.Websites</span></span>
* <span data-ttu-id="67887-1375">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="67887-1375">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="67887-1376">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="67887-1376">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="67887-1377">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1377">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="67887-1378">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-1378">Az.Cdn</span></span>
* <span data-ttu-id="67887-1379">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="67887-1379">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1380">Az.Compute</span></span>
* <span data-ttu-id="67887-1381">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="67887-1381">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="67887-1382">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="67887-1382">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-1383">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-1383">Az.EventHub</span></span>
* <span data-ttu-id="67887-1384">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="67887-1384">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="67887-1385">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="67887-1385">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1386">Az.Network</span></span>
* <span data-ttu-id="67887-1387">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="67887-1387">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="67887-1388">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="67887-1388">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-1389">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1389">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-1390">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="67887-1390">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1391">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1392">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="67887-1392">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="67887-1393">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="67887-1393">Az.ServiceBus</span></span>
* <span data-ttu-id="67887-1394">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="67887-1394">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-1395">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-1395">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-1396">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="67887-1396">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="67887-1397">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="67887-1397">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1398">Az.Sql</span></span>
* <span data-ttu-id="67887-1399">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="67887-1399">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="67887-1400">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1400">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="67887-1401">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="67887-1401">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="67887-1402">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="67887-1402">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1403">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1403">Az.Websites</span></span>
* <span data-ttu-id="67887-1404">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="67887-1404">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="67887-1405">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1405">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="67887-1406">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-1406">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-1407">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="67887-1407">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="67887-1408">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="67887-1408">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="67887-1409">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="67887-1409">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="67887-1410">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="67887-1410">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="67887-1411">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1411">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="67887-1412">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="67887-1412">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="67887-1413">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="67887-1413">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="67887-1414">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="67887-1414">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="67887-1415">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-1415">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="67887-1416">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="67887-1416">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="67887-1417">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="67887-1417">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="67887-1418">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="67887-1418">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="67887-1419">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="67887-1419">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="67887-1420">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="67887-1420">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="67887-1421">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="67887-1421">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="67887-1422">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="67887-1422">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="67887-1423">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="67887-1423">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="67887-1424">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="67887-1424">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="67887-1425">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="67887-1425">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="67887-1426">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="67887-1426">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="67887-1427">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="67887-1427">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="67887-1428">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="67887-1428">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="67887-1429">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="67887-1429">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="67887-1430">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-1430">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="67887-1431">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="67887-1431">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="67887-1432">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="67887-1432">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="67887-1433">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="67887-1433">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="67887-1434">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="67887-1434">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="67887-1435">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="67887-1435">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="67887-1436">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="67887-1436">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="67887-1437">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="67887-1437">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="67887-1438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="67887-1438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="67887-1439">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="67887-1439">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="67887-1440">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="67887-1440">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="67887-1441">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="67887-1441">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="67887-1442">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="67887-1442">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="67887-1443">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="67887-1443">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="67887-1444">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="67887-1444">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="67887-1445">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="67887-1445">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="67887-1446">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="67887-1446">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="67887-1447">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="67887-1447">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="67887-1448">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="67887-1448">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="67887-1449">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="67887-1449">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="67887-1450">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="67887-1450">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="67887-1451">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="67887-1451">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="67887-1452">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="67887-1452">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="67887-1453">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="67887-1453">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="67887-1454">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="67887-1454">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="67887-1455">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="67887-1455">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="67887-1456">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="67887-1456">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="67887-1457">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="67887-1457">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="67887-1458">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="67887-1458">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="67887-1459">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="67887-1459">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="67887-1460">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="67887-1460">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="67887-1461">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="67887-1461">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="67887-1462">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="67887-1462">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="67887-1463">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="67887-1463">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="67887-1464">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="67887-1464">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="67887-1465">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="67887-1465">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="67887-1466">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="67887-1466">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="67887-1467">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="67887-1467">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="67887-1468">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="67887-1468">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="67887-1469">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="67887-1469">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="67887-1470">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="67887-1470">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="67887-1471">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="67887-1471">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="67887-1472">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="67887-1472">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="67887-1473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="67887-1473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="67887-1474">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="67887-1474">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="67887-1475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="67887-1475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="67887-1476">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="67887-1476">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="67887-1477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="67887-1477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="67887-1478">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="67887-1478">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="67887-1479">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="67887-1479">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="67887-1480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="67887-1480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="67887-1481">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="67887-1481">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="67887-1482">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="67887-1482">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="67887-1483">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="67887-1483">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1484">Az.Automation</span></span>
* <span data-ttu-id="67887-1485">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="67887-1485">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="67887-1486">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="67887-1486">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="67887-1487">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="67887-1487">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="67887-1488">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="67887-1488">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="67887-1489">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="67887-1489">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="67887-1490">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="67887-1490">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="67887-1491">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="67887-1491">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1492">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1492">Az.Compute</span></span>
* <span data-ttu-id="67887-1493">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="67887-1493">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="67887-1494">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="67887-1494">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-1495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-1495">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-1496">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1496">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-1497">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-1497">Az.Monitor</span></span>
* <span data-ttu-id="67887-1498">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-1498">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1499">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1499">Az.Network</span></span>
* <span data-ttu-id="67887-1500">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="67887-1500">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="67887-1501">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="67887-1501">Updated cmdlet:</span></span>
        - <span data-ttu-id="67887-1502">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="67887-1502">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="67887-1503">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="67887-1503">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1504">Az.Resources</span></span>
* <span data-ttu-id="67887-1505">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="67887-1505">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1506">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1506">Az.Sql</span></span>
* <span data-ttu-id="67887-1507">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="67887-1507">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="67887-1508">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1508">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1509">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1509">Az.Accounts</span></span>
* <span data-ttu-id="67887-1510">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="67887-1510">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-1511">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-1511">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-1512">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="67887-1512">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="67887-1513">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="67887-1513">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1514">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1514">Az.Compute</span></span>
* <span data-ttu-id="67887-1515">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="67887-1515">Proximity placement group feature.</span></span>
    - <span data-ttu-id="67887-1516">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="67887-1516">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="67887-1517">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1517">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="67887-1518">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="67887-1518">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="67887-1519">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="67887-1519">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="67887-1520">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-1520">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="67887-1521">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="67887-1521">Breaking changes</span></span>
    - <span data-ttu-id="67887-1522">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="67887-1522">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="67887-1523">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="67887-1523">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="67887-1524">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="67887-1524">Az.DeploymentManager</span></span>
* <span data-ttu-id="67887-1525">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1525">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="67887-1526">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="67887-1526">Az.Dns</span></span>
* <span data-ttu-id="67887-1527">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="67887-1527">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="67887-1528">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="67887-1528">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="67887-1529">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="67887-1529">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="67887-1530">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-1530">Az.FrontDoor</span></span>
* <span data-ttu-id="67887-1531">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="67887-1531">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="67887-1532">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="67887-1532">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="67887-1533">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-1533">Az.HDInsight</span></span>
* <span data-ttu-id="67887-1534">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-1534">Removed two cmdlets:</span></span>
    - <span data-ttu-id="67887-1535">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="67887-1535">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="67887-1536">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="67887-1536">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="67887-1537">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="67887-1537">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="67887-1538">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="67887-1538">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="67887-1539">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="67887-1539">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="67887-1540">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="67887-1540">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-1541">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-1541">Az.Monitor</span></span>
* <span data-ttu-id="67887-1542">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="67887-1542">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="67887-1543">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="67887-1543">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="67887-1544">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="67887-1544">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="67887-1545">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="67887-1545">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="67887-1546">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="67887-1546">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="67887-1547">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="67887-1547">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="67887-1548">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="67887-1548">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="67887-1549">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="67887-1549">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="67887-1550">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="67887-1550">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="67887-1551">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="67887-1551">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="67887-1552">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="67887-1552">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="67887-1553">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="67887-1553">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="67887-1554">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="67887-1554">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="67887-1555">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="67887-1555">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1556">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1556">Az.Network</span></span>
* <span data-ttu-id="67887-1557">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="67887-1557">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="67887-1558">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1558">New cmdlets</span></span>
        - <span data-ttu-id="67887-1559">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="67887-1559">New-AzNatGateway</span></span>
        - <span data-ttu-id="67887-1560">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="67887-1560">Get-AzNatGateway</span></span>
        - <span data-ttu-id="67887-1561">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="67887-1561">Set-AzNatGateway</span></span>
        - <span data-ttu-id="67887-1562">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="67887-1562">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="67887-1563">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="67887-1563">Updated cmdlets</span></span>
        - <span data-ttu-id="67887-1564">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="67887-1564">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="67887-1565">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="67887-1565">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="67887-1566">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1566">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="67887-1567">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1567">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="67887-1568">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="67887-1568">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-1569">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1569">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-1570">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="67887-1570">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="67887-1571">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="67887-1571">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="67887-1572">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="67887-1572">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1573">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1573">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1574">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="67887-1574">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="67887-1575">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="67887-1575">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="67887-1576">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="67887-1576">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="67887-1577">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-1577">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="67887-1578">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="67887-1578">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="67887-1579">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="67887-1579">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="67887-1580">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="67887-1580">Az.Relay</span></span>
* <span data-ttu-id="67887-1581">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="67887-1581">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="67887-1582">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="67887-1582">Az.ServiceBus</span></span>
* <span data-ttu-id="67887-1583">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="67887-1583">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1584">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1584">Az.Storage</span></span>
* <span data-ttu-id="67887-1585">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="67887-1585">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="67887-1586">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="67887-1586">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="67887-1587">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="67887-1587">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="67887-1588">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1588">New-AzStorageAccount</span></span>
* <span data-ttu-id="67887-1589">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="67887-1589">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="67887-1590">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1590">New-AzStorageAccount</span></span>
    - <span data-ttu-id="67887-1591">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1591">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="67887-1592">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1592">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1593">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1593">Az.Websites</span></span>
* <span data-ttu-id="67887-1594">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="67887-1594">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="67887-1595">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="67887-1595">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="67887-1596">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1596">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="67887-1597">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="67887-1597">Highlights since the last major release</span></span>
* <span data-ttu-id="67887-1598">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="67887-1598">General availability of `Az` module</span></span>
* <span data-ttu-id="67887-1599">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="67887-1599">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="67887-1600">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="67887-1600">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="67887-1601">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1601">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="67887-1602">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="67887-1602">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="67887-1603">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1603">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="67887-1604">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="67887-1604">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-1605">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1605">Az.Accounts</span></span>
* <span data-ttu-id="67887-1606">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="67887-1606">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="67887-1607">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="67887-1607">Az.Batch</span></span>
* <span data-ttu-id="67887-1608">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1608">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-1609">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-1609">Az.Cdn</span></span>
* <span data-ttu-id="67887-1610">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1610">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-1611">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-1611">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-1612">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1612">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1613">Az.Compute</span></span>
* <span data-ttu-id="67887-1614">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="67887-1614">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="67887-1615">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1615">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="67887-1616">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="67887-1616">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1617">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1618">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="67887-1618">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-1619">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-1619">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-1620">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1620">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="67887-1621">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="67887-1621">Az.EventGrid</span></span>
* <span data-ttu-id="67887-1622">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="67887-1622">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-1623">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-1623">Az.EventHub</span></span>
* <span data-ttu-id="67887-1624">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="67887-1624">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="67887-1625">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="67887-1625">Az.HDInsight</span></span>
* <span data-ttu-id="67887-1626">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1626">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-1627">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-1627">Az.IotHub</span></span>
* <span data-ttu-id="67887-1628">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1628">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-1629">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-1629">Az.KeyVault</span></span>
* <span data-ttu-id="67887-1630">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1630">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="67887-1631">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="67887-1631">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="67887-1632">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="67887-1632">Az.MachineLearning</span></span>
* <span data-ttu-id="67887-1633">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1633">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="67887-1634">Az.Media</span><span class="sxs-lookup"><span data-stu-id="67887-1634">Az.Media</span></span>
* <span data-ttu-id="67887-1635">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1635">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-1636">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-1636">Az.Monitor</span></span>
  * <span data-ttu-id="67887-1637">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="67887-1637">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="67887-1638">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="67887-1638">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="67887-1639">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="67887-1639">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="67887-1640">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="67887-1640">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="67887-1641">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="67887-1641">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="67887-1642">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="67887-1642">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="67887-1643">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="67887-1643">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1644">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1644">Az.Network</span></span>
* <span data-ttu-id="67887-1645">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1645">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="67887-1646">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="67887-1646">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="67887-1647">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="67887-1647">Az.NotificationHubs</span></span>
* <span data-ttu-id="67887-1648">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1648">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="67887-1649">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1649">Az.OperationalInsights</span></span>
* <span data-ttu-id="67887-1650">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1650">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="67887-1651">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="67887-1651">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="67887-1652">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1652">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1653">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1653">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1654">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1654">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="67887-1655">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1655">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="67887-1656">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="67887-1656">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="67887-1657">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="67887-1657">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="67887-1658">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="67887-1658">Az.RedisCache</span></span>
* <span data-ttu-id="67887-1659">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1659">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1660">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1660">Az.Resources</span></span>
* <span data-ttu-id="67887-1661">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="67887-1661">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1662">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1662">Az.Sql</span></span>
* <span data-ttu-id="67887-1663">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="67887-1663">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="67887-1664">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1664">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="67887-1665">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="67887-1665">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="67887-1666">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="67887-1666">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="67887-1667">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="67887-1667">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="67887-1668">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="67887-1668">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="67887-1669">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="67887-1669">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1670">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1670">Az.Websites</span></span>
* <span data-ttu-id="67887-1671">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="67887-1671">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="67887-1672">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="67887-1672">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="67887-1673">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="67887-1673">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="67887-1674">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="67887-1674">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="67887-1675">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1675">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="67887-1676">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="67887-1676">Highlights since the last major release</span></span>
* <span data-ttu-id="67887-1677">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="67887-1677">General availability of `Az` module</span></span>
* <span data-ttu-id="67887-1678">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="67887-1678">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="67887-1679">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="67887-1679">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="67887-1680">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1680">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="67887-1681">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="67887-1681">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="67887-1682">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1682">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="67887-1683">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="67887-1683">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="67887-1684">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1684">Az.Accounts</span></span>
* <span data-ttu-id="67887-1685">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="67887-1685">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="67887-1686">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="67887-1686">Az.AnalysisServices</span></span>
* <span data-ttu-id="67887-1687">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="67887-1687">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="67887-1688">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="67887-1688">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1689">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1689">Az.Automation</span></span>
* <span data-ttu-id="67887-1690">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="67887-1690">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="67887-1691">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="67887-1691">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="67887-1692">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="67887-1692">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1693">Az.Compute</span></span>
* <span data-ttu-id="67887-1694">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="67887-1694">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="67887-1695">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="67887-1695">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="67887-1696">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="67887-1696">Az.ContainerInstance</span></span>
* <span data-ttu-id="67887-1697">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="67887-1697">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1698">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1698">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1699">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="67887-1699">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="67887-1700">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="67887-1700">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1701">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1701">Az.Resources</span></span>
* <span data-ttu-id="67887-1702">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="67887-1702">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="67887-1703">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="67887-1703">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="67887-1704">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="67887-1704">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="67887-1705">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="67887-1705">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="67887-1706">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="67887-1706">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="67887-1707">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="67887-1707">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1708">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1708">Az.Sql</span></span>
* <span data-ttu-id="67887-1709">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="67887-1709">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1710">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1710">Az.Storage</span></span>
* <span data-ttu-id="67887-1711">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1711">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="67887-1712">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="67887-1712">New-AzStorageContext</span></span>
* <span data-ttu-id="67887-1713">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="67887-1713">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="67887-1714">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="67887-1714">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="67887-1715">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="67887-1715">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="67887-1716">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1716">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="67887-1717">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1717">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="67887-1718">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="67887-1718">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="67887-1719">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="67887-1719">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="67887-1720">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="67887-1720">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="67887-1721">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="67887-1721">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="67887-1722">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="67887-1722">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="67887-1723">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1723">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="67887-1724">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="67887-1724">Highlights since the last major release</span></span>
* <span data-ttu-id="67887-1725">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="67887-1725">General availability of `Az` module</span></span>
* <span data-ttu-id="67887-1726">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="67887-1726">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="67887-1727">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="67887-1727">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="67887-1728">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1728">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="67887-1729">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="67887-1729">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="67887-1730">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1730">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="67887-1731">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="67887-1731">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1732">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1732">Az.Automation</span></span>
* <span data-ttu-id="67887-1733">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="67887-1733">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="67887-1734">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="67887-1734">Dynamic grouping</span></span>
    * <span data-ttu-id="67887-1735">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="67887-1735">Pre-Post script</span></span>
    * <span data-ttu-id="67887-1736">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="67887-1736">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1737">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1737">Az.Compute</span></span>
* <span data-ttu-id="67887-1738">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="67887-1738">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="67887-1739">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="67887-1739">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-1740">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-1740">Az.KeyVault</span></span>
* <span data-ttu-id="67887-1741">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-1741">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1742">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1742">Az.Network</span></span>
* <span data-ttu-id="67887-1743">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="67887-1743">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="67887-1744">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="67887-1744">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1745">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1745">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1746">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="67887-1746">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="67887-1747">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="67887-1747">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1748">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1748">Az.Resources</span></span>
* <span data-ttu-id="67887-1749">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="67887-1749">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="67887-1750">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="67887-1750">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1751">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1751">Az.Sql</span></span>
* <span data-ttu-id="67887-1752">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="67887-1752">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1753">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1753">Az.Storage</span></span>
* <span data-ttu-id="67887-1754">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="67887-1754">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="67887-1755">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1755">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="67887-1756">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1756">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="67887-1757">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1757">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="67887-1758">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="67887-1758">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="67887-1759">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="67887-1759">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="67887-1760">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="67887-1760">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1761">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1761">Az.Websites</span></span>
* <span data-ttu-id="67887-1762">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="67887-1762">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="67887-1763">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1763">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1764">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1764">Az.Accounts</span></span>
* <span data-ttu-id="67887-1765">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="67887-1765">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="67887-1766">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1766">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1767">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1767">Az.Automation</span></span>
* <span data-ttu-id="67887-1768">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1768">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="67887-1769">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="67887-1769">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="67887-1770">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="67887-1770">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-1771">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-1771">Az.Cdn</span></span>
* <span data-ttu-id="67887-1772">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="67887-1772">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1773">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1773">Az.Compute</span></span>
* <span data-ttu-id="67887-1774">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="67887-1774">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1775">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1775">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1776">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="67887-1776">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="67887-1777">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="67887-1777">Az.LogicApp</span></span>
* <span data-ttu-id="67887-1778">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="67887-1778">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1779">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1779">Az.Network</span></span>
* <span data-ttu-id="67887-1780">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="67887-1780">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1781">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1781">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1782">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-1782">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="67887-1783">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="67887-1783">SDK Update</span></span>
* <span data-ttu-id="67887-1784">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="67887-1784">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="67887-1785">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="67887-1785">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1786">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1786">Az.Resources</span></span>
* <span data-ttu-id="67887-1787">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="67887-1787">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="67887-1788">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="67887-1788">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="67887-1789">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="67887-1789">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="67887-1790">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="67887-1790">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="67887-1791">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="67887-1791">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="67887-1792">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="67887-1792">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1793">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1793">Az.Sql</span></span>
* <span data-ttu-id="67887-1794">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="67887-1794">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="67887-1795">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="67887-1795">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1796">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1796">Az.Storage</span></span>
* <span data-ttu-id="67887-1797">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-1797">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="67887-1798">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1798">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="67887-1799">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="67887-1799">Az.AnalysisServices</span></span>
* <span data-ttu-id="67887-1800">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="67887-1800">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1801">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1801">Az.Automation</span></span>
* <span data-ttu-id="67887-1802">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1802">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="67887-1803">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1803">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="67887-1804">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1804">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-1805">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-1805">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-1806">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="67887-1806">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1807">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1807">Az.Compute</span></span>
* <span data-ttu-id="67887-1808">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="67887-1808">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="67887-1809">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="67887-1809">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="67887-1810">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="67887-1810">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="67887-1811">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="67887-1811">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-1812">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-1812">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-1813">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="67887-1813">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="67887-1814">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="67887-1814">Az.EventHub</span></span>
* <span data-ttu-id="67887-1815">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="67887-1815">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-1816">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-1816">Az.KeyVault</span></span>
* <span data-ttu-id="67887-1817">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="67887-1817">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="67887-1818">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="67887-1818">Az.LogicApp</span></span>
* <span data-ttu-id="67887-1819">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="67887-1819">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="67887-1820">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="67887-1820">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="67887-1821">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="67887-1821">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="67887-1822">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="67887-1822">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="67887-1823">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="67887-1823">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="67887-1824">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="67887-1824">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="67887-1825">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="67887-1825">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="67887-1826">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="67887-1826">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="67887-1827">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1827">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="67887-1828">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1828">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="67887-1829">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1829">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="67887-1830">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-1830">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="67887-1831">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="67887-1831">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="67887-1832">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-1832">Az.Monitor</span></span>
* <span data-ttu-id="67887-1833">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="67887-1833">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1834">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1834">Az.Network</span></span>
* <span data-ttu-id="67887-1835">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="67887-1835">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="67887-1836">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-1836">Az.OperationalInsights</span></span>
* <span data-ttu-id="67887-1837">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="67887-1837">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="67887-1838">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="67887-1838">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="67887-1839">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="67887-1839">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1840">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1840">Az.Resources</span></span>
* <span data-ttu-id="67887-1841">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="67887-1841">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="67887-1842">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="67887-1842">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="67887-1843">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="67887-1843">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="67887-1844">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="67887-1844">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1845">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1845">Az.Sql</span></span>
* <span data-ttu-id="67887-1846">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="67887-1846">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="67887-1847">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="67887-1847">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1848">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1848">Az.Websites</span></span>
* <span data-ttu-id="67887-1849">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="67887-1849">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="67887-1850">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1850">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1851">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1851">Az.Accounts</span></span>
* <span data-ttu-id="67887-1852">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="67887-1852">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="67887-1853">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="67887-1853">Az.AnalysisServices</span></span>
<span data-ttu-id="67887-1854">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="67887-1854">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1855">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1855">Az.Compute</span></span>
* <span data-ttu-id="67887-1856">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="67887-1856">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="67887-1857">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="67887-1857">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="67887-1858">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="67887-1858">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1859">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1859">Az.RecoveryServices</span></span>
<span data-ttu-id="67887-1860">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="67887-1860">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1861">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1861">Az.Resources</span></span>
* <span data-ttu-id="67887-1862">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="67887-1862">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="67887-1863">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="67887-1863">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="67887-1864">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="67887-1864">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="67887-1865">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="67887-1865">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1866">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1866">Az.Sql</span></span>
* <span data-ttu-id="67887-1867">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="67887-1867">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="67887-1868">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="67887-1868">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="67887-1869">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="67887-1869">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="67887-1870">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1870">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1871">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1871">Az.Accounts</span></span>
* <span data-ttu-id="67887-1872">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="67887-1872">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="67887-1873">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="67887-1873">Az.AnalysisServices</span></span>
* <span data-ttu-id="67887-1874">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="67887-1874">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="67887-1875">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-1875">Az.RecoveryServices</span></span>
* <span data-ttu-id="67887-1876">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="67887-1876">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="67887-1877">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1877">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1878">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1878">Az.Accounts</span></span>
* <span data-ttu-id="67887-1879">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="67887-1879">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="67887-1880">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1880">Update incorrect online help URLs</span></span>
* <span data-ttu-id="67887-1881">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="67887-1881">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="67887-1882">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="67887-1882">Az.Aks</span></span>
* <span data-ttu-id="67887-1883">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1883">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="67887-1884">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-1884">Az.Automation</span></span>
* <span data-ttu-id="67887-1885">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="67887-1885">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="67887-1886">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1886">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="67887-1887">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="67887-1887">Az.Cdn</span></span>
* <span data-ttu-id="67887-1888">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1888">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1889">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1889">Az.Compute</span></span>
* <span data-ttu-id="67887-1890">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="67887-1890">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="67887-1891">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="67887-1891">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="67887-1892">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="67887-1892">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="67887-1893">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="67887-1893">Az.ContainerRegistry</span></span>
* <span data-ttu-id="67887-1894">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1894">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="67887-1895">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="67887-1895">Az.DataFactory</span></span>
* <span data-ttu-id="67887-1896">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="67887-1896">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-1897">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-1897">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-1898">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="67887-1898">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="67887-1899">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="67887-1899">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="67887-1900">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1900">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-1901">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-1901">Az.IotHub</span></span>
* <span data-ttu-id="67887-1902">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="67887-1902">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="67887-1903">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-1903">Az.KeyVault</span></span>
* <span data-ttu-id="67887-1904">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1904">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-1905">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-1905">Az.Network</span></span>
* <span data-ttu-id="67887-1906">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1906">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1907">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1907">Az.Resources</span></span>
* <span data-ttu-id="67887-1908">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="67887-1908">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="67887-1909">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="67887-1909">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="67887-1910">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="67887-1910">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="67887-1911">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="67887-1911">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="67887-1912">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="67887-1912">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="67887-1913">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="67887-1913">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="67887-1914">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="67887-1914">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-1915">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-1915">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-1916">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="67887-1916">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="67887-1917">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="67887-1917">Fix some error messages.</span></span>
* <span data-ttu-id="67887-1918">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="67887-1918">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="67887-1919">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="67887-1919">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="67887-1920">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="67887-1920">Az.SignalR</span></span>
* <span data-ttu-id="67887-1921">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1921">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1922">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1922">Az.Sql</span></span>
* <span data-ttu-id="67887-1923">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1923">Update incorrect online help URLs</span></span>
* <span data-ttu-id="67887-1924">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="67887-1924">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="67887-1925">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="67887-1925">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="67887-1926">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="67887-1926">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1927">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1927">Az.Storage</span></span>
* <span data-ttu-id="67887-1928">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1928">Update incorrect online help URLs</span></span>
* <span data-ttu-id="67887-1929">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="67887-1929">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="67887-1930">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="67887-1930">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="67887-1931">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="67887-1931">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="67887-1932">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="67887-1932">Az.TrafficManager</span></span>
* <span data-ttu-id="67887-1933">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1933">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1934">Az.Websites</span></span>
* <span data-ttu-id="67887-1935">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="67887-1935">Update incorrect online help URLs</span></span>
* <span data-ttu-id="67887-1936">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="67887-1936">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="67887-1937">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="67887-1937">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="67887-1938">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="67887-1938">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="67887-1939">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1939">Az.Accounts</span></span>
* <span data-ttu-id="67887-1940">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="67887-1940">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-1941">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-1941">Az.Compute</span></span>
* <span data-ttu-id="67887-1942">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="67887-1942">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="67887-1943">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="67887-1943">Updated the description of ID in help files</span></span>
* <span data-ttu-id="67887-1944">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1944">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-1945">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-1945">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-1946">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="67887-1946">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="67887-1947">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="67887-1947">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="67887-1948">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="67887-1948">Az.EventGrid</span></span>
* <span data-ttu-id="67887-1949">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="67887-1949">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="67887-1950">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="67887-1950">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="67887-1951">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="67887-1951">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="67887-1952">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="67887-1952">Event Time-To-Live,</span></span>
        - <span data-ttu-id="67887-1953">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="67887-1953">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="67887-1954">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="67887-1954">Dead letter endpoint.</span></span>
    - <span data-ttu-id="67887-1955">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="67887-1955">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="67887-1956">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="67887-1956">Event Time-To-Live,</span></span>
        - <span data-ttu-id="67887-1957">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="67887-1957">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="67887-1958">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="67887-1958">Dead letter endpoint.</span></span>
* <span data-ttu-id="67887-1959">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="67887-1959">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="67887-1960">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="67887-1960">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="67887-1961">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-1961">Az.IotHub</span></span>
* <span data-ttu-id="67887-1962">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="67887-1962">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="67887-1963">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="67887-1963">Az.LogicApp</span></span>
* <span data-ttu-id="67887-1964">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="67887-1964">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-1965">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-1965">Az.Resources</span></span>
* <span data-ttu-id="67887-1966">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="67887-1966">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="67887-1967">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="67887-1967">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="67887-1968">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="67887-1968">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="67887-1969">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="67887-1969">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="67887-1970">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="67887-1970">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="67887-1971">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="67887-1971">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="67887-1972">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="67887-1972">Az.SignalR</span></span>
* <span data-ttu-id="67887-1973">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1973">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-1974">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-1974">Az.Sql</span></span>
* <span data-ttu-id="67887-1975">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="67887-1975">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="67887-1976">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-1976">Az.Storage</span></span>
* <span data-ttu-id="67887-1977">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="67887-1977">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="67887-1978">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="67887-1978">New-AzStorageContext</span></span>
* <span data-ttu-id="67887-1979">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="67887-1979">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="67887-1980">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="67887-1980">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-1981">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-1981">Az.Websites</span></span>
* <span data-ttu-id="67887-1982">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="67887-1982">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="67887-1983">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1983">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="67887-1984">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-1984">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="67887-1985">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-1985">General</span></span>

- <span data-ttu-id="67887-1986">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="67887-1986">General Availability of Az Module</span></span>
- <span data-ttu-id="67887-1987">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="67887-1987">Online help for each module</span></span>
- <span data-ttu-id="67887-1988">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="67887-1988">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="67887-1989">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="67887-1989">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="67887-1990">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-1990">Az.Accounts</span></span>
- <span data-ttu-id="67887-1991">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="67887-1991">Changed from Az.Profile</span></span>
- <span data-ttu-id="67887-1992">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="67887-1992">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="67887-1993">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-1993">Az.ApiManagement</span></span>
- <span data-ttu-id="67887-1994">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="67887-1994">Fixes for #7002</span></span>
- <span data-ttu-id="67887-1995">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-1995">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="67887-1996">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="67887-1996">Az.Batch</span></span>
- <span data-ttu-id="67887-1997">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="67887-1997">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="67887-1998">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="67887-1998">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="67887-1999">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-1999">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="67887-2000">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="67887-2000">Az.Billing</span></span>
- <span data-ttu-id="67887-2001">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2001">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="67887-2002">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="67887-2002">Az.CognitivServices</span></span>
- <span data-ttu-id="67887-2003">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="67887-2003">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="67887-2004">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="67887-2004">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="67887-2005">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="67887-2005">Az.ContainerInstance</span></span>
- <span data-ttu-id="67887-2006">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="67887-2006">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="67887-2007">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="67887-2007">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="67887-2008">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2008">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="67887-2009">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-2009">Az.DataLakeStore</span></span>
- <span data-ttu-id="67887-2010">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2010">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="67887-2011">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="67887-2011">Az.Monitor</span></span>
- <span data-ttu-id="67887-2012">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2012">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="67887-2013">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="67887-2013">Az.KeyVault</span></span>
- <span data-ttu-id="67887-2014">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="67887-2014">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="67887-2015">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="67887-2015">Az.MachineLearning</span></span>
- <span data-ttu-id="67887-2016">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="67887-2016">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="67887-2017">Az.Media</span><span class="sxs-lookup"><span data-stu-id="67887-2017">Az.Media</span></span>
- <span data-ttu-id="67887-2018">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="67887-2018">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="67887-2019">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-2019">Az.Network</span></span>
<span data-ttu-id="67887-2020">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="67887-2020">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="67887-2021">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67887-2021">New cmdlets added:</span></span>
        - <span data-ttu-id="67887-2022">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-2022">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="67887-2023">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-2023">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="67887-2024">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-2024">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="67887-2025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-2025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="67887-2026">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-2026">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="67887-2027">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="67887-2027">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="67887-2028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="67887-2028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="67887-2029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="67887-2029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="67887-2030">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="67887-2030">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="67887-2031">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="67887-2031">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="67887-2032">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="67887-2032">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="67887-2033">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="67887-2033">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="67887-2034">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="67887-2034">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="67887-2035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="67887-2035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="67887-2036">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="67887-2036">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="67887-2037">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="67887-2037">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="67887-2038">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="67887-2038">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="67887-2039">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="67887-2039">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="67887-2040">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="67887-2040">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="67887-2041">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="67887-2041">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="67887-2042">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2042">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="67887-2043">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="67887-2043">Az.OperationalInsights</span></span>
- <span data-ttu-id="67887-2044">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2044">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="67887-2045">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="67887-2045">Az.Profile</span></span>
- <span data-ttu-id="67887-2046">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="67887-2046">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="67887-2047">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-2047">Az.RecoveryServices</span></span>
- <span data-ttu-id="67887-2048">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2048">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="67887-2049">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-2049">Az.Resources</span></span>
- <span data-ttu-id="67887-2050">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2050">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="67887-2051">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-2051">Az.ServiceFabric</span></span>
- <span data-ttu-id="67887-2052">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="67887-2052">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="67887-2053">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2053">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="67887-2054">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="67887-2054">Az.SIgnalR</span></span>
- <span data-ttu-id="67887-2055">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="67887-2055">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="67887-2056">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-2056">Az.Sql</span></span>
- <span data-ttu-id="67887-2057">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="67887-2057">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="67887-2058">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="67887-2058">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="67887-2059">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2059">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="67887-2060">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-2060">Az.Storage</span></span>
- <span data-ttu-id="67887-2061">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2061">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="67887-2062">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-2062">Az.Websites</span></span>
- <span data-ttu-id="67887-2063">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="67887-2063">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="67887-2064">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-2064">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="67887-2065">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-2065">General</span></span>

* <span data-ttu-id="67887-2066">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="67887-2066">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="67887-2067">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-2067">Az.Compute</span></span>

* <span data-ttu-id="67887-2068">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="67887-2068">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="67887-2069">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-2069">Az.DataLakeStore</span></span>

* <span data-ttu-id="67887-2070">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="67887-2070">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="67887-2071">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="67887-2071">Az.FrontDoor</span></span>

* <span data-ttu-id="67887-2072">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="67887-2072">Fixed some broken links</span></span>
    - <span data-ttu-id="67887-2073">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="67887-2073">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="67887-2074">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="67887-2074">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="67887-2075">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="67887-2075">Az.RecoveryServices</span></span>

* <span data-ttu-id="67887-2076">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-2076">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="67887-2077">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="67887-2077">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="67887-2078">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-2078">Az.Resources</span></span>

* <span data-ttu-id="67887-2079">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="67887-2079">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="67887-2080">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="67887-2080">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="67887-2081">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-2081">Az.Sql</span></span>

* <span data-ttu-id="67887-2082">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="67887-2082">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="67887-2083">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="67887-2083">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="67887-2084">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="67887-2084">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="67887-2085">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-2085">Az.Storage</span></span>

* <span data-ttu-id="67887-2086">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="67887-2086">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="67887-2087">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="67887-2087">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="67887-2088">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="67887-2088">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="67887-2089">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="67887-2089">Support Static Website configuration</span></span>
    - <span data-ttu-id="67887-2090">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="67887-2090">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="67887-2091">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="67887-2091">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="67887-2092">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-2092">Az.Websites</span></span>

* <span data-ttu-id="67887-2093">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="67887-2093">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="67887-2094">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="67887-2094">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="67887-2095">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-2095">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="67887-2096">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-2096">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="67887-2097">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="67887-2097">Az.ApiManagement</span></span>
* <span data-ttu-id="67887-2098">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="67887-2098">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="67887-2099">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="67887-2099">Az.Automation</span></span>
* <span data-ttu-id="67887-2100">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="67887-2100">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="67887-2101">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="67887-2101">Added Update Management cmdlets</span></span>
* <span data-ttu-id="67887-2102">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="67887-2102">Added Source Control cmdlets</span></span>
* <span data-ttu-id="67887-2103">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="67887-2103">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="67887-2104">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="67887-2104">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="67887-2105">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-2105">Az.Compute</span></span>
* <span data-ttu-id="67887-2106">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="67887-2106">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="67887-2107">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="67887-2107">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="67887-2108">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="67887-2108">Az.ContainerInstance</span></span>
* <span data-ttu-id="67887-2109">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="67887-2109">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="67887-2110">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="67887-2110">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="67887-2111">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="67887-2111">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="67887-2112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-2112">Az.Network</span></span>
* <span data-ttu-id="67887-2113">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="67887-2113">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="67887-2114">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="67887-2114">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="67887-2115">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="67887-2115">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="67887-2116">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="67887-2116">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="67887-2117">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="67887-2117">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="67887-2118">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="67887-2118">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="67887-2119">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="67887-2119">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="67887-2120">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="67887-2120">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="67887-2121">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="67887-2121">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="67887-2122">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="67887-2122">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="67887-2123">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="67887-2123">Az.Relay</span></span>
* <span data-ttu-id="67887-2124">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="67887-2124">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="67887-2125">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-2125">Az.Resources</span></span>
* <span data-ttu-id="67887-2126">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="67887-2126">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="67887-2127">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="67887-2127">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="67887-2128">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="67887-2128">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="67887-2129">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-2129">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-2130">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="67887-2130">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="67887-2131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-2131">Az.Sql</span></span>
* <span data-ttu-id="67887-2132">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-2132">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="67887-2133">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="67887-2133">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="67887-2134">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="67887-2134">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="67887-2135">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="67887-2135">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="67887-2136">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="67887-2136">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="67887-2137">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="67887-2137">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="67887-2138">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="67887-2138">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="67887-2139">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="67887-2139">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="67887-2140">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="67887-2140">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="67887-2141">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="67887-2141">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="67887-2142">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="67887-2142">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="67887-2143">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="67887-2143">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="67887-2144">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="67887-2144">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="67887-2145">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="67887-2145">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="67887-2146">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="67887-2146">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="67887-2147">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="67887-2147">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="67887-2148">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="67887-2148">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="67887-2149">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-2149">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="67887-2150">Geral</span><span class="sxs-lookup"><span data-stu-id="67887-2150">General</span></span>
* <span data-ttu-id="67887-2151">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="67887-2151">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="67887-2152">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="67887-2152">Az.Profile</span></span>
* <span data-ttu-id="67887-2153">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="67887-2153">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="67887-2154">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="67887-2154">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="67887-2155">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="67887-2155">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="67887-2156">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="67887-2156">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="67887-2157">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="67887-2157">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="67887-2158">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="67887-2158">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="67887-2159">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="67887-2159">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-2160">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-2160">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-2161">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="67887-2161">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-2162">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-2162">Az.Compute</span></span>
* <span data-ttu-id="67887-2163">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="67887-2163">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="67887-2164">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="67887-2164">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="67887-2165">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="67887-2165">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-2166">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-2166">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-2167">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="67887-2167">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="67887-2168">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="67887-2168">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="67887-2169">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="67887-2169">Az.Insights</span></span>
* <span data-ttu-id="67887-2170">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="67887-2170">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="67887-2171">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="67887-2171">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="67887-2172">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="67887-2172">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="67887-2173">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="67887-2173">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-2174">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-2174">Az.Network</span></span>
* <span data-ttu-id="67887-2175">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="67887-2175">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="67887-2176">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="67887-2176">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="67887-2177">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="67887-2177">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="67887-2178">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="67887-2178">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="67887-2179">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="67887-2179">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="67887-2180">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="67887-2180">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="67887-2181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="67887-2181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="67887-2182">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="67887-2182">Az.PolicyInsights</span></span>
* <span data-ttu-id="67887-2183">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="67887-2183">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-2184">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-2184">Az.Resources</span></span>
* <span data-ttu-id="67887-2185">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="67887-2185">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="67887-2186">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="67887-2186">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="67887-2187">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="67887-2187">Az.ServiceBus</span></span>
* <span data-ttu-id="67887-2188">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="67887-2188">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="67887-2189">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="67887-2189">Az.ServiceFabric</span></span>
* <span data-ttu-id="67887-2190">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="67887-2190">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="67887-2191">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="67887-2191">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="67887-2192">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="67887-2192">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="67887-2193">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="67887-2193">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="67887-2194">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="67887-2194">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="67887-2195">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-2195">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="67887-2196">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="67887-2196">Az.Profile</span></span>
* <span data-ttu-id="67887-2197">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="67887-2197">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="67887-2198">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="67887-2198">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-2199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-2199">Az.Compute</span></span>
* <span data-ttu-id="67887-2200">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="67887-2200">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="67887-2201">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="67887-2201">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="67887-2202">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="67887-2202">Az.DataLakeStore</span></span>
* <span data-ttu-id="67887-2203">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="67887-2203">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="67887-2204">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-2204">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="67887-2205">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="67887-2205">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="67887-2206">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="67887-2206">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="67887-2207">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="67887-2207">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-2208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-2208">Az.Network</span></span>
* <span data-ttu-id="67887-2209">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="67887-2209">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="67887-2210">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="67887-2210">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-2211">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-2211">Az.Resources</span></span>
* <span data-ttu-id="67887-2212">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="67887-2212">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="67887-2213">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="67887-2213">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="67887-2214">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-2214">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="67887-2215">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="67887-2215">Azure.Storage</span></span>
* <span data-ttu-id="67887-2216">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="67887-2216">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="67887-2217">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="67887-2217">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="67887-2218">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="67887-2218">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="67887-2219">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="67887-2219">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="67887-2220">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="67887-2220">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="67887-2221">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="67887-2221">Az.CognitiveServices</span></span>
* <span data-ttu-id="67887-2222">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="67887-2222">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="67887-2223">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="67887-2223">Az.Compute</span></span>
* <span data-ttu-id="67887-2224">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="67887-2224">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="67887-2225">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="67887-2225">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="67887-2226">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="67887-2226">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="67887-2227">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="67887-2227">Az.DataFactoryV2</span></span>
* <span data-ttu-id="67887-2228">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="67887-2228">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="67887-2229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="67887-2229">Az.Network</span></span>
* <span data-ttu-id="67887-2230">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="67887-2230">Added NetworkProfile functionality.</span></span> <span data-ttu-id="67887-2231">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="67887-2231">new cmdlets added</span></span>
    - <span data-ttu-id="67887-2232">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="67887-2232">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="67887-2233">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="67887-2233">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="67887-2234">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="67887-2234">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="67887-2235">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="67887-2235">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="67887-2236">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="67887-2236">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="67887-2237">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="67887-2237">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="67887-2238">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="67887-2238">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="67887-2239">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="67887-2239">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="67887-2240">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="67887-2240">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="67887-2241">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="67887-2241">Az.RedisCache</span></span>
* <span data-ttu-id="67887-2242">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="67887-2242">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="67887-2243">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="67887-2243">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="67887-2244">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="67887-2244">Az.Resources</span></span>
* <span data-ttu-id="67887-2245">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="67887-2245">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="67887-2246">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="67887-2246">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="67887-2247">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="67887-2247">Az.Sql</span></span>
* <span data-ttu-id="67887-2248">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="67887-2248">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="67887-2249">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="67887-2249">Az.Websites</span></span>
* <span data-ttu-id="67887-2250">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="67887-2250">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="67887-2251">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="67887-2251">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="67887-2252">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="67887-2252">0.2.0 - September 2018</span></span>
 <span data-ttu-id="67887-2253">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="67887-2253">Initial Release</span></span>
