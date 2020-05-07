---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: a9c5394a5fac8a8a3de96925b3563776783ea9fe
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "82080203"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="e0305-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e0305-103">Azure PowerShell release notes</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="e0305-104">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-104">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="e0305-105">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="e0305-105">Highlights since the last release</span></span>
* <span data-ttu-id="e0305-106">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="e0305-106">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-107">Az.Accounts</span></span>
* <span data-ttu-id="e0305-108">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="e0305-108">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="e0305-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-109">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-110">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="e0305-110">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="e0305-111">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="e0305-111">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-112">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-112">Az.Cdn</span></span>
* <span data-ttu-id="e0305-113">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="e0305-113">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-114">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-114">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-115">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="e0305-115">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-116">Az.Compute</span></span>
* <span data-ttu-id="e0305-117">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="e0305-117">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="e0305-118">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="e0305-118">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-119">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-119">Az.IotHub</span></span>
* <span data-ttu-id="e0305-120">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-120">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="e0305-121">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="e0305-121">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="e0305-122">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="e0305-122">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="e0305-123">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-123">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="e0305-124">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-124">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="e0305-125">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="e0305-125">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="e0305-126">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="e0305-126">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="e0305-127">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="e0305-127">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="e0305-128">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-128">New cmdlets are:</span></span>
    - <span data-ttu-id="e0305-129">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="e0305-129">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="e0305-130">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="e0305-130">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="e0305-131">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="e0305-131">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="e0305-132">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="e0305-132">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="e0305-133">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-133">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-134">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-134">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-135">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="e0305-135">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="e0305-136">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="e0305-136">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="e0305-137">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="e0305-137">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="e0305-138">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="e0305-138">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="e0305-139">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="e0305-139">Az.Maintenance</span></span>
* <span data-ttu-id="e0305-140">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-140">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-141">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-141">Az.Monitor</span></span>
* <span data-ttu-id="e0305-142">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="e0305-142">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="e0305-143">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="e0305-143">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="e0305-144">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="e0305-144">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="e0305-145">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="e0305-145">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="e0305-146">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="e0305-146">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="e0305-147">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="e0305-147">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="e0305-148">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="e0305-148">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="e0305-149">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="e0305-149">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-150">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-150">Az.Network</span></span>
* <span data-ttu-id="e0305-151">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="e0305-151">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="e0305-152">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="e0305-152">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="e0305-153">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="e0305-153">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="e0305-154">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="e0305-154">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="e0305-155">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="e0305-155">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="e0305-156">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="e0305-156">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="e0305-157">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="e0305-157">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="e0305-158">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="e0305-158">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="e0305-159">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="e0305-159">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="e0305-160">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="e0305-160">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="e0305-161">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="e0305-161">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="e0305-162">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="e0305-162">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="e0305-163">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="e0305-163">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="e0305-164">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="e0305-164">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="e0305-165">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-165">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="e0305-166">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-166">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-167">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-167">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-168">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="e0305-168">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="e0305-169">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="e0305-169">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-170">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-170">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-171">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="e0305-171">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-172">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-172">Az.Sql</span></span>
* <span data-ttu-id="e0305-173">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="e0305-173">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="e0305-174">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="e0305-174">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-175">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-175">Az.Storage</span></span>
* <span data-ttu-id="e0305-176">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="e0305-176">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="e0305-177">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e0305-177">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="e0305-178">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="e0305-178">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="e0305-179">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="e0305-179">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="e0305-180">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="e0305-180">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="e0305-181">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="e0305-181">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="e0305-182">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="e0305-182">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="e0305-183">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="e0305-183">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="e0305-184">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="e0305-184">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="e0305-185">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="e0305-185">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="e0305-186">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="e0305-186">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="e0305-187">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="e0305-187">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="e0305-188">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="e0305-188">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="e0305-189">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-189">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="e0305-190">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-190">General</span></span>
* <span data-ttu-id="e0305-191">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="e0305-191">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="e0305-192">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="e0305-192">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="e0305-193">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="e0305-193">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="e0305-194">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="e0305-194">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="e0305-195">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="e0305-195">Az.Billing</span></span>
  - <span data-ttu-id="e0305-196">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-196">Az.Compute</span></span>
  - <span data-ttu-id="e0305-197">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="e0305-197">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="e0305-198">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-198">Az.EventHub</span></span>
  - <span data-ttu-id="e0305-199">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-199">Az.IotHub</span></span>
  - <span data-ttu-id="e0305-200">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-200">Az.KeyVault</span></span>
  - <span data-ttu-id="e0305-201">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-201">Az.Monitor</span></span>
  - <span data-ttu-id="e0305-202">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-202">Az.Network</span></span>
  - <span data-ttu-id="e0305-203">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-203">Az.Resources</span></span>
  - <span data-ttu-id="e0305-204">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-204">Az.Storage</span></span>
  - <span data-ttu-id="e0305-205">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-205">Az.Websites</span></span>
* <span data-ttu-id="e0305-206">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-206">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="e0305-207">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="e0305-207">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="e0305-208">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="e0305-208">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="e0305-209">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-209">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-210">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-210">Az.Accounts</span></span>
* <span data-ttu-id="e0305-211">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="e0305-211">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-212">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-212">Az.Compute</span></span>
* <span data-ttu-id="e0305-213">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="e0305-213">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="e0305-214">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="e0305-214">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="e0305-215">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="e0305-215">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="e0305-216">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="e0305-216">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="e0305-217">[#11354]</span><span class="sxs-lookup"><span data-stu-id="e0305-217">[#11354]</span></span>
* <span data-ttu-id="e0305-218">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="e0305-218">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="e0305-219">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="e0305-219">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="e0305-220">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="e0305-220">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="e0305-221">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="e0305-221">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="e0305-222">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="e0305-222">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="e0305-223">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-223">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="e0305-224">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="e0305-224">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="e0305-225">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="e0305-225">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="e0305-226">[#11257]</span><span class="sxs-lookup"><span data-stu-id="e0305-226">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-227">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-227">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-228">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="e0305-228">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="e0305-229">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="e0305-229">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-230">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-230">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-231">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="e0305-231">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="e0305-232">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="e0305-232">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="e0305-233">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-233">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-234">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="e0305-234">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-235">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-235">Az.IotHub</span></span>
* <span data-ttu-id="e0305-236">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0305-236">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="e0305-237">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-237">New Cmdlets are:</span></span>
    - <span data-ttu-id="e0305-238">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="e0305-238">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="e0305-239">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="e0305-239">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-240">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-240">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-241">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="e0305-241">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-242">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-242">Az.Monitor</span></span>
* <span data-ttu-id="e0305-243">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="e0305-243">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-244">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-244">Az.Network</span></span>
* <span data-ttu-id="e0305-245">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="e0305-245">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="e0305-246">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="e0305-246">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="e0305-247">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="e0305-247">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="e0305-248">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="e0305-248">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="e0305-249">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="e0305-249">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="e0305-250">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="e0305-250">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-251">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-251">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-252">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="e0305-252">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-254">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-254">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="e0305-255">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="e0305-255">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="e0305-256">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="e0305-256">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="e0305-257">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="e0305-257">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="e0305-258">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="e0305-258">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="e0305-259">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="e0305-259">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-260">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-260">Az.Resources</span></span>
* <span data-ttu-id="e0305-261">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="e0305-261">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="e0305-262">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="e0305-262">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="e0305-263">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="e0305-263">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="e0305-264">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="e0305-264">Added example.</span></span>
* <span data-ttu-id="e0305-265">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="e0305-265">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="e0305-266">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="e0305-266">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-267">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-267">Az.Sql</span></span>
* <span data-ttu-id="e0305-268">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="e0305-268">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="e0305-269">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="e0305-269">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="e0305-270">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="e0305-270">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="e0305-271">Az.Support</span><span class="sxs-lookup"><span data-stu-id="e0305-271">Az.Support</span></span>
* <span data-ttu-id="e0305-272">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="e0305-272">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-273">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-273">Az.Websites</span></span>
* <span data-ttu-id="e0305-274">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="e0305-274">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="e0305-275">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="e0305-275">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="e0305-276">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="e0305-276">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="e0305-277">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="e0305-277">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="e0305-278">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="e0305-278">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="e0305-279">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-279">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-280">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-280">Az.Accounts</span></span>
* <span data-ttu-id="e0305-281">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="e0305-281">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="e0305-282">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="e0305-282">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="e0305-283">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="e0305-283">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="e0305-284">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-284">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-285">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="e0305-285">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="e0305-286">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="e0305-286">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="e0305-287">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="e0305-287">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="e0305-288">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="e0305-288">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-289">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-289">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-290">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="e0305-290">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-291">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-291">Az.IotHub</span></span>
* <span data-ttu-id="e0305-292">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-292">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="e0305-293">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-293">New Cmdlets are:</span></span>
    - <span data-ttu-id="e0305-294">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-294">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="e0305-295">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-295">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="e0305-296">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-296">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="e0305-297">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-297">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="e0305-298">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-298">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="e0305-299">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-299">New Cmdlets are:</span></span>
    - <span data-ttu-id="e0305-300">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="e0305-300">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="e0305-301">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="e0305-301">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="e0305-302">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="e0305-302">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="e0305-303">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="e0305-303">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="e0305-304">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-304">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="e0305-305">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-305">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="e0305-306">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-306">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="e0305-307">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-307">New Cmdlets are:</span></span>
    - <span data-ttu-id="e0305-308">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="e0305-308">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="e0305-309">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="e0305-309">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="e0305-310">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0305-310">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-311">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-311">Az.Monitor</span></span>
* <span data-ttu-id="e0305-312">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="e0305-312">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-313">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-313">Az.Network</span></span>
* <span data-ttu-id="e0305-314">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="e0305-314">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="e0305-315">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="e0305-315">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="e0305-316">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="e0305-316">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="e0305-317">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="e0305-317">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-318">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-318">Az.Resources</span></span>
* <span data-ttu-id="e0305-319">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="e0305-319">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="e0305-320">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="e0305-320">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="e0305-321">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="e0305-321">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="e0305-322">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="e0305-322">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="e0305-323">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="e0305-323">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="e0305-324">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="e0305-324">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="e0305-325">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="e0305-325">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="e0305-326">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="e0305-326">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="e0305-327">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="e0305-327">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="e0305-328">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="e0305-328">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="e0305-329">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="e0305-329">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="e0305-330">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="e0305-330">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="e0305-331">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="e0305-331">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="e0305-332">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="e0305-332">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-333">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-333">Az.Sql</span></span>
* <span data-ttu-id="e0305-334">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="e0305-334">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="e0305-335">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="e0305-335">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="e0305-336">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="e0305-336">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="e0305-337">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="e0305-337">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="e0305-338">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="e0305-338">Remove an LTR backup</span></span>
    - <span data-ttu-id="e0305-339">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="e0305-339">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="e0305-340">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="e0305-340">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="e0305-341">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-341">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="e0305-342">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-342">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-343">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-343">Az.Storage</span></span>
* <span data-ttu-id="e0305-344">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-344">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="e0305-345">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="e0305-345">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="e0305-346">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="e0305-346">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="e0305-347">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="e0305-347">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="e0305-348">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="e0305-348">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-349">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-349">Az.Websites</span></span>
* <span data-ttu-id="e0305-350">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="e0305-350">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="e0305-351">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="e0305-351">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="e0305-352">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="e0305-352">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="e0305-353">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="e0305-353">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="e0305-354">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="e0305-354">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="e0305-355">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-355">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="e0305-356">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="e0305-356">Highlights since the last major release</span></span>
* <span data-ttu-id="e0305-357">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="e0305-357">Updated client side telemetry.</span></span>
* <span data-ttu-id="e0305-358">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e0305-358">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="e0305-359">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="e0305-359">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-360">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-360">Az.Accounts</span></span>
* <span data-ttu-id="e0305-361">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="e0305-361">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-362">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-362">Az.Automation</span></span>
* <span data-ttu-id="e0305-363">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="e0305-363">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-364">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-364">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-365">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="e0305-365">Updated SDK to 7.0</span></span>
* <span data-ttu-id="e0305-366">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="e0305-366">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-367">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-367">Az.Compute</span></span>
* <span data-ttu-id="e0305-368">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="e0305-368">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="e0305-369">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-369">Az.FrontDoor</span></span>
* <span data-ttu-id="e0305-370">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="e0305-370">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-371">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-371">Az.IotHub</span></span>
* <span data-ttu-id="e0305-372">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="e0305-372">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="e0305-373">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-373">New Cmdlets are:</span></span>
    - <span data-ttu-id="e0305-374">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-374">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="e0305-375">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-375">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="e0305-376">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-376">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="e0305-377">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="e0305-377">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-378">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-378">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-379">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="e0305-379">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-380">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-380">Az.Monitor</span></span>
* <span data-ttu-id="e0305-381">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="e0305-381">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="e0305-382">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="e0305-382">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="e0305-383">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="e0305-383">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-384">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-384">Az.Network</span></span>
* <span data-ttu-id="e0305-385">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="e0305-385">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="e0305-386">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="e0305-386">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="e0305-387">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="e0305-387">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="e0305-388">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="e0305-388">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="e0305-389">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="e0305-389">No new cmdlets are added.</span></span> <span data-ttu-id="e0305-390">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="e0305-390">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-391">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-392">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="e0305-392">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-393">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-393">Az.Resources</span></span>
* <span data-ttu-id="e0305-394">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="e0305-394">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="e0305-395">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="e0305-395">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="e0305-396">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="e0305-396">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="e0305-397">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="e0305-397">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="e0305-398">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="e0305-398">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="e0305-399">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="e0305-399">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="e0305-400">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="e0305-400">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="e0305-401">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="e0305-401">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-402">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-402">Az.Sql</span></span>
* <span data-ttu-id="e0305-403">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="e0305-403">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="e0305-404">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="e0305-404">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="e0305-405">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="e0305-405">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="e0305-406">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="e0305-406">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="e0305-407">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="e0305-407">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="e0305-408">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="e0305-408">Az.StorageSync</span></span>
* <span data-ttu-id="e0305-409">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="e0305-409">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="e0305-410">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-410">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="e0305-411">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="e0305-411">Highlights since the last major release</span></span>
* <span data-ttu-id="e0305-412">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="e0305-412">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="e0305-413">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="e0305-413">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-414">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-414">Az.Accounts</span></span>
* <span data-ttu-id="e0305-415">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="e0305-415">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="e0305-416">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="e0305-416">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="e0305-417">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-417">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-418">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="e0305-418">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="e0305-419">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="e0305-419">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="e0305-420">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="e0305-420">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="e0305-421">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="e0305-421">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-422">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-422">Az.Compute</span></span>
* <span data-ttu-id="e0305-423">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="e0305-423">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="e0305-424">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="e0305-424">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="e0305-425">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-425">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="e0305-426">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-426">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="e0305-427">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="e0305-427">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-428">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-428">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-429">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="e0305-429">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="e0305-430">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="e0305-430">Az.DeploymentManager</span></span>
* <span data-ttu-id="e0305-431">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="e0305-431">Adds LIST operations for resources</span></span>
* <span data-ttu-id="e0305-432">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="e0305-432">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="e0305-433">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-433">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-434">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="e0305-434">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-435">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-435">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-436">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="e0305-436">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-437">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-437">Az.Network</span></span>
* <span data-ttu-id="e0305-438">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="e0305-438">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="e0305-439">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="e0305-439">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="e0305-440">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="e0305-440">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="e0305-441">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="e0305-441">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="e0305-442">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="e0305-442">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="e0305-443">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="e0305-443">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="e0305-444">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e0305-444">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="e0305-445">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="e0305-445">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="e0305-446">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-446">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-447">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-447">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="e0305-448">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-448">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="e0305-449">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="e0305-449">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="e0305-450">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="e0305-450">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-451">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-451">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-452">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="e0305-452">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="e0305-453">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="e0305-453">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="e0305-454">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="e0305-454">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="e0305-455">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="e0305-455">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-456">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-456">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-457">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="e0305-457">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="e0305-458">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="e0305-458">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-459">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-459">Az.Resources</span></span>
* <span data-ttu-id="e0305-460">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="e0305-460">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="e0305-461">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="e0305-461">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-462">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-462">Az.Sql</span></span>
<span data-ttu-id="e0305-463">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="e0305-463">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-464">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-464">Az.Storage</span></span>
* <span data-ttu-id="e0305-465">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e0305-465">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="e0305-466">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-466">New-AzStorageAccount</span></span>
* <span data-ttu-id="e0305-467">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="e0305-467">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="e0305-468">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="e0305-468">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-469">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-469">Az.Websites</span></span>
* <span data-ttu-id="e0305-470">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="e0305-470">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="e0305-471">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="e0305-471">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="e0305-472">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e0305-472">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-473">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-473">Az.Accounts</span></span>
* <span data-ttu-id="e0305-474">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="e0305-474">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-475">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-475">Az.Cdn</span></span>
* <span data-ttu-id="e0305-476">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="e0305-476">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-477">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-477">Az.Compute</span></span>
* <span data-ttu-id="e0305-478">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="e0305-478">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="e0305-479">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-479">Az.ContainerInstance</span></span>
* <span data-ttu-id="e0305-480">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-480">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="e0305-481">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="e0305-481">Az.DataBoxEdge</span></span>
* <span data-ttu-id="e0305-482">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="e0305-482">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="e0305-483">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-483">Get the Edge Storage Container</span></span>
* <span data-ttu-id="e0305-484">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="e0305-484">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="e0305-485">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-485">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="e0305-486">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="e0305-486">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="e0305-487">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-487">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="e0305-488">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="e0305-488">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="e0305-489">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-489">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="e0305-490">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="e0305-490">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="e0305-491">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-491">Get the Edge Storage Account</span></span>
* <span data-ttu-id="e0305-492">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="e0305-492">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="e0305-493">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-493">Create new Edge Storage Account</span></span>
* <span data-ttu-id="e0305-494">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="e0305-494">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="e0305-495">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="e0305-495">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="e0305-496">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="e0305-496">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="e0305-497">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="e0305-497">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="e0305-498">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="e0305-498">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="e0305-499">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="e0305-499">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-500">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-500">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-501">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="e0305-501">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="e0305-502">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="e0305-502">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="e0305-503">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="e0305-503">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="e0305-504">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="e0305-504">Az.DevTestLabs</span></span>
* <span data-ttu-id="e0305-505">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="e0305-505">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-506">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-506">Az.EventHub</span></span>
* <span data-ttu-id="e0305-507">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="e0305-507">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="e0305-508">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-508">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-509">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="e0305-509">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="e0305-510">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="e0305-510">Az.MachineLearning</span></span>
* <span data-ttu-id="e0305-511">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="e0305-511">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="e0305-512">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="e0305-512">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="e0305-513">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="e0305-513">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="e0305-514">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="e0305-514">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="e0305-515">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="e0305-515">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="e0305-516">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="e0305-516">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="e0305-517">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="e0305-517">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="e0305-518">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="e0305-518">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-519">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-519">Az.Network</span></span>
* <span data-ttu-id="e0305-520">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="e0305-520">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-521">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-521">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-522">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-522">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="e0305-523">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-523">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="e0305-524">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-524">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="e0305-525">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-525">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-526">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-526">Az.Resources</span></span>
* <span data-ttu-id="e0305-527">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="e0305-527">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-528">Az.Sql</span></span>
* <span data-ttu-id="e0305-529">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="e0305-529">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="e0305-530">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="e0305-530">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="e0305-531">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="e0305-531">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="e0305-532">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="e0305-532">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-533">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-533">Az.Storage</span></span>
* <span data-ttu-id="e0305-534">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="e0305-534">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="e0305-535">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-535">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="e0305-536">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="e0305-536">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="e0305-537">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-537">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="e0305-538">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-538">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="e0305-539">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-539">General</span></span>
* <span data-ttu-id="e0305-540">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="e0305-540">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-541">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-541">Az.Accounts</span></span>
* <span data-ttu-id="e0305-542">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="e0305-542">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="e0305-543">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="e0305-543">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="e0305-544">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e0305-544">Az.Batch</span></span>
* <span data-ttu-id="e0305-545">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="e0305-545">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-546">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-546">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-547">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="e0305-547">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="e0305-548">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-548">Az.FrontDoor</span></span>
* <span data-ttu-id="e0305-549">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="e0305-549">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="e0305-550">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="e0305-550">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="e0305-551">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="e0305-551">Az.HealthcareApis</span></span>
* <span data-ttu-id="e0305-552">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="e0305-552">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-553">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-553">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-554">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="e0305-554">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="e0305-555">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="e0305-555">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="e0305-556">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="e0305-556">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-557">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-557">Az.Monitor</span></span>
* <span data-ttu-id="e0305-558">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="e0305-558">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="e0305-559">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="e0305-559">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="e0305-560">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="e0305-560">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-561">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-561">Az.Network</span></span>
* <span data-ttu-id="e0305-562">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="e0305-562">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-563">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-563">Az.Resources</span></span>
* <span data-ttu-id="e0305-564">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="e0305-564">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="e0305-565">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="e0305-565">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-566">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-566">Az.Sql</span></span>
* <span data-ttu-id="e0305-567">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="e0305-567">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-568">Az.Storage</span></span>
* <span data-ttu-id="e0305-569">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="e0305-569">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="e0305-570">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="e0305-570">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="e0305-571">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="e0305-571">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="e0305-572">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="e0305-572">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="e0305-573">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="e0305-573">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="e0305-574">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="e0305-574">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="e0305-575">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="e0305-575">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="e0305-576">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="e0305-576">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="e0305-577">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="e0305-577">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="e0305-578">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="e0305-578">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="e0305-579">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="e0305-579">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="e0305-580">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="e0305-580">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="e0305-581">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="e0305-581">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="e0305-582">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-582">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="e0305-583">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="e0305-583">Highlights since the last major release</span></span>
* <span data-ttu-id="e0305-584">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="e0305-584">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="e0305-585">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="e0305-585">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-586">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-586">Az.Compute</span></span>
* <span data-ttu-id="e0305-587">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="e0305-587">VM Reapply feature</span></span>
    - <span data-ttu-id="e0305-588">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="e0305-588">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="e0305-589">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="e0305-589">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="e0305-590">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-590">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="e0305-591">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="e0305-591">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="e0305-592">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-592">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="e0305-593">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="e0305-593">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="e0305-594">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="e0305-594">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="e0305-595">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="e0305-595">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="e0305-596">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="e0305-596">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="e0305-597">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-597">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="e0305-598">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="e0305-598">Az.DataBoxEdge</span></span>
* <span data-ttu-id="e0305-599">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="e0305-599">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="e0305-600">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="e0305-600">Get the Order</span></span>
* <span data-ttu-id="e0305-601">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="e0305-601">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="e0305-602">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="e0305-602">Create new Order</span></span>
* <span data-ttu-id="e0305-603">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="e0305-603">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="e0305-604">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="e0305-604">Remove the Order</span></span>
* <span data-ttu-id="e0305-605">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="e0305-605">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="e0305-606">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="e0305-606">Now creates Local Share</span></span>
* <span data-ttu-id="e0305-607">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="e0305-607">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="e0305-608">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="e0305-608">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="e0305-609">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="e0305-609">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="e0305-610">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0305-610">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="e0305-611">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="e0305-611">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="e0305-612">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="e0305-612">Gets the information about Triggers</span></span>
* <span data-ttu-id="e0305-613">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="e0305-613">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="e0305-614">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="e0305-614">Create new Triggers</span></span>
* <span data-ttu-id="e0305-615">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="e0305-615">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="e0305-616">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="e0305-616">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-617">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-618">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="e0305-618">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="e0305-619">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="e0305-619">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-620">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-620">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-621">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="e0305-621">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-622">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-622">Az.EventHub</span></span>
* <span data-ttu-id="e0305-623">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="e0305-623">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="e0305-624">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-624">Az.FrontDoor</span></span>
* <span data-ttu-id="e0305-625">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="e0305-625">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="e0305-626">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="e0305-626">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="e0305-627">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="e0305-627">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="e0305-628">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="e0305-628">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-629">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-629">Az.Network</span></span>
* <span data-ttu-id="e0305-630">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="e0305-630">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="e0305-631">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="e0305-631">Az.PrivateDns</span></span>
* <span data-ttu-id="e0305-632">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="e0305-632">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-633">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-633">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-634">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="e0305-634">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="e0305-635">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="e0305-635">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="e0305-636">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="e0305-636">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="e0305-637">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="e0305-637">Az.RedisCache</span></span>
* <span data-ttu-id="e0305-638">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="e0305-638">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="e0305-639">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="e0305-639">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="e0305-640">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="e0305-640">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-641">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-641">Az.Resources</span></span>
- <span data-ttu-id="e0305-642">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="e0305-642">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="e0305-643">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="e0305-643">Updated create policy definition help example</span></span>
- <span data-ttu-id="e0305-644">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="e0305-644">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="e0305-645">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="e0305-645">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="e0305-646">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="e0305-646">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-647">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-647">Az.Sql</span></span>
* <span data-ttu-id="e0305-648">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="e0305-648">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="e0305-649">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="e0305-649">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="e0305-650">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-650">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="e0305-651">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-651">General</span></span>
* <span data-ttu-id="e0305-652">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="e0305-652">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-653">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-653">Az.Accounts</span></span>
* <span data-ttu-id="e0305-654">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="e0305-654">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="e0305-655">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="e0305-655">Az.Advisor</span></span>
* <span data-ttu-id="e0305-656">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="e0305-656">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="e0305-657">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e0305-657">Az.Batch</span></span>
* <span data-ttu-id="e0305-658">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="e0305-658">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="e0305-659">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="e0305-659">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="e0305-660">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="e0305-660">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="e0305-661">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="e0305-661">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="e0305-662">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="e0305-662">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="e0305-663">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="e0305-663">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="e0305-664">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="e0305-664">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="e0305-665">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="e0305-665">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="e0305-666">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="e0305-666">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="e0305-667">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="e0305-667">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="e0305-668">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="e0305-668">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="e0305-669">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="e0305-669">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="e0305-670">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="e0305-670">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="e0305-671">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="e0305-671">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="e0305-672">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="e0305-672">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="e0305-673">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="e0305-673">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="e0305-674">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="e0305-674">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="e0305-675">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="e0305-675">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="e0305-676">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="e0305-676">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="e0305-677">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="e0305-677">This operation is no longer supported.</span></span>
* <span data-ttu-id="e0305-678">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="e0305-678">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="e0305-679">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="e0305-679">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="e0305-680">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="e0305-680">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="e0305-681">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="e0305-681">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="e0305-682">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="e0305-682">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="e0305-683">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="e0305-683">New non-verified images are also now returned.</span></span> <span data-ttu-id="e0305-684">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="e0305-684">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="e0305-685">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="e0305-685">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="e0305-686">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="e0305-686">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="e0305-687">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="e0305-687">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="e0305-688">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="e0305-688">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="e0305-689">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="e0305-689">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="e0305-690">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="e0305-690">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="e0305-691">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="e0305-691">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="e0305-692">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="e0305-692">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="e0305-693">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="e0305-693">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-694">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-694">Az.Cdn</span></span>
* <span data-ttu-id="e0305-695">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="e0305-695">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="e0305-696">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="e0305-696">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-697">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-697">Az.Compute</span></span>
* <span data-ttu-id="e0305-698">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="e0305-698">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="e0305-699">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="e0305-699">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="e0305-700">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="e0305-700">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="e0305-701">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-701">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="e0305-702">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-702">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="e0305-703">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="e0305-703">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="e0305-704">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-704">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="e0305-705">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="e0305-705">Breaking changes</span></span>
    - <span data-ttu-id="e0305-706">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="e0305-706">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="e0305-707">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="e0305-707">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-708">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-708">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-709">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="e0305-709">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-710">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-710">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-711">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="e0305-711">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="e0305-712">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="e0305-712">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="e0305-713">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="e0305-713">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="e0305-714">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="e0305-714">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="e0305-715">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="e0305-715">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="e0305-716">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="e0305-716">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="e0305-717">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-717">Az.FrontDoor</span></span>
* <span data-ttu-id="e0305-718">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="e0305-718">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="e0305-719">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-719">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-720">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="e0305-720">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="e0305-721">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="e0305-721">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="e0305-722">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="e0305-722">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="e0305-723">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-723">Removed five cmdlets:</span></span>
    - <span data-ttu-id="e0305-724">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="e0305-724">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="e0305-725">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="e0305-725">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="e0305-726">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="e0305-726">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="e0305-727">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="e0305-727">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="e0305-728">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="e0305-728">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="e0305-729">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-729">Added three cmdlets:</span></span>
    - <span data-ttu-id="e0305-730">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="e0305-730">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="e0305-731">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="e0305-731">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="e0305-732">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="e0305-732">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="e0305-733">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="e0305-733">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="e0305-734">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="e0305-734">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="e0305-735">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="e0305-735">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="e0305-736">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-736">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="e0305-737">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="e0305-737">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="e0305-738">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="e0305-738">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="e0305-739">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="e0305-739">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="e0305-740">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="e0305-740">Added some scenario test cases.</span></span>
* <span data-ttu-id="e0305-741">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="e0305-741">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-742">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-742">Az.IotHub</span></span>
* <span data-ttu-id="e0305-743">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="e0305-743">Breaking changes:</span></span>
    - <span data-ttu-id="e0305-744">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="e0305-744">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="e0305-745">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="e0305-745">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="e0305-746">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="e0305-746">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="e0305-747">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="e0305-747">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="e0305-748">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="e0305-748">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="e0305-749">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="e0305-749">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="e0305-750">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="e0305-750">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="e0305-751">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="e0305-751">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="e0305-752">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="e0305-752">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="e0305-753">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="e0305-753">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="e0305-754">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="e0305-754">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="e0305-755">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="e0305-755">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-756">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-756">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-757">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-757">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-758">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-758">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="e0305-759">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-759">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="e0305-760">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-760">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-761">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-761">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-762">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-762">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-763">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-763">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-764">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-764">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-765">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="e0305-765">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-766">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-766">Az.Resources</span></span>
* <span data-ttu-id="e0305-767">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="e0305-767">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-768">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-768">Az.Network</span></span>
* <span data-ttu-id="e0305-769">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="e0305-769">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="e0305-770">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="e0305-770">Updated cmdlet:</span></span>
        - <span data-ttu-id="e0305-771">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-771">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-772">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-772">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-773">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-773">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-774">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-774">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-775">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-775">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="e0305-776">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="e0305-776">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="e0305-777">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e0305-777">New cmdlet:</span></span>
        - <span data-ttu-id="e0305-778">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="e0305-778">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="e0305-779">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="e0305-779">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="e0305-780">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-780">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="e0305-781">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-781">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="e0305-782">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="e0305-782">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="e0305-783">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="e0305-783">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="e0305-784">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-784">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="e0305-785">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="e0305-785">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="e0305-786">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-786">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-787">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="e0305-787">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="e0305-788">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="e0305-788">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="e0305-789">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="e0305-789">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="e0305-790">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="e0305-790">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="e0305-791">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="e0305-791">Set-AzVirtualHub</span></span>
* <span data-ttu-id="e0305-792">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="e0305-792">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="e0305-793">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="e0305-793">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="e0305-794">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="e0305-794">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="e0305-795">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="e0305-795">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="e0305-796">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="e0305-796">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="e0305-797">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="e0305-797">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="e0305-798">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-798">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="e0305-799">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-799">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-800">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-800">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="e0305-801">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="e0305-801">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="e0305-802">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="e0305-802">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="e0305-803">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="e0305-803">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="e0305-804">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="e0305-804">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="e0305-805">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="e0305-805">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="e0305-806">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="e0305-806">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="e0305-807">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="e0305-807">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="e0305-808">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-808">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-809">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="e0305-809">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="e0305-810">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="e0305-810">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="e0305-811">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="e0305-811">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="e0305-812">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="e0305-812">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="e0305-813">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="e0305-813">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="e0305-814">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-814">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="e0305-815">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="e0305-815">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="e0305-816">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="e0305-816">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="e0305-817">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="e0305-817">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="e0305-818">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="e0305-818">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="e0305-819">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="e0305-819">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="e0305-820">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="e0305-820">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="e0305-821">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="e0305-821">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="e0305-822">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="e0305-822">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="e0305-823">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e0305-823">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="e0305-824">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="e0305-824">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="e0305-825">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-825">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="e0305-826">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-826">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-827">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-827">New-AzIpGroup</span></span>
        - <span data-ttu-id="e0305-828">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-828">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="e0305-829">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-829">Get-AzIpGroup</span></span>
        - <span data-ttu-id="e0305-830">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-830">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-831">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-831">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-832">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="e0305-832">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-833">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-833">Az.Sql</span></span>
* <span data-ttu-id="e0305-834">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="e0305-834">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="e0305-835">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="e0305-835">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="e0305-836">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="e0305-836">Removed deprecated aliases:</span></span>
* <span data-ttu-id="e0305-837">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="e0305-837">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="e0305-838">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="e0305-838">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="e0305-839">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-839">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="e0305-840">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="e0305-840">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="e0305-841">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="e0305-841">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="e0305-842">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="e0305-842">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-843">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-843">Az.Storage</span></span>
* <span data-ttu-id="e0305-844">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e0305-844">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="e0305-845">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-845">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="e0305-846">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-846">Set-AzStorageAccount</span></span>
* <span data-ttu-id="e0305-847">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="e0305-847">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="e0305-848">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="e0305-848">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="e0305-849">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="e0305-849">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="e0305-850">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-850">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="e0305-851">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-851">General</span></span>
* <span data-ttu-id="e0305-852">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="e0305-852">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-853">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-853">Az.Accounts</span></span>
* <span data-ttu-id="e0305-854">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="e0305-854">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="e0305-855">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-855">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-856">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="e0305-856">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="e0305-857">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="e0305-857">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-858">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-858">Az.Automation</span></span>
* <span data-ttu-id="e0305-859">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="e0305-859">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="e0305-860">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e0305-860">Az.Batch</span></span>
* <span data-ttu-id="e0305-861">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="e0305-861">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-862">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-862">Az.Compute</span></span>
* <span data-ttu-id="e0305-863">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-863">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="e0305-864">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="e0305-864">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="e0305-865">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="e0305-865">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="e0305-866">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="e0305-866">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-867">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-867">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-868">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="e0305-868">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="e0305-869">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="e0305-869">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="e0305-870">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="e0305-870">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-871">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-871">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-872">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="e0305-872">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="e0305-873">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="e0305-873">Az.HealthcareApis</span></span>
* <span data-ttu-id="e0305-874">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="e0305-874">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="e0305-875">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="e0305-875">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="e0305-876">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="e0305-876">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="e0305-877">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="e0305-877">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-878">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-878">Az.IotHub</span></span>
* <span data-ttu-id="e0305-879">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="e0305-879">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="e0305-880">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="e0305-880">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-881">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-881">Az.Monitor</span></span>
* <span data-ttu-id="e0305-882">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="e0305-882">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="e0305-883">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="e0305-883">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="e0305-884">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="e0305-884">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="e0305-885">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e0305-885">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-886">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-886">Az.Network</span></span>
* <span data-ttu-id="e0305-887">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="e0305-887">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="e0305-888">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="e0305-888">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="e0305-889">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-889">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-890">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-890">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="e0305-891">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-891">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="e0305-892">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="e0305-892">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="e0305-893">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="e0305-893">Updated cmdlets:</span></span>
        - <span data-ttu-id="e0305-894">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-894">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="e0305-895">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-895">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="e0305-896">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-896">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="e0305-897">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="e0305-897">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="e0305-898">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="e0305-898">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="e0305-899">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="e0305-899">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="e0305-900">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="e0305-900">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="e0305-901">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="e0305-901">Az.RedisCache</span></span>
* <span data-ttu-id="e0305-902">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="e0305-902">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-903">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-903">Az.Sql</span></span>
* <span data-ttu-id="e0305-904">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="e0305-904">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-905">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-905">Az.Storage</span></span>
* <span data-ttu-id="e0305-906">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="e0305-906">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="e0305-907">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="e0305-907">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="e0305-908">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="e0305-908">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="e0305-909">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="e0305-909">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="e0305-910">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-910">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="e0305-911">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="e0305-911">Az.StorageSync</span></span>
* <span data-ttu-id="e0305-912">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="e0305-912">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-913">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-913">Az.Websites</span></span>
* <span data-ttu-id="e0305-914">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="e0305-914">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="e0305-915">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-915">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="e0305-916">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-916">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-917">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="e0305-917">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="e0305-918">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="e0305-918">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="e0305-919">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="e0305-919">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-920">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-920">Az.Automation</span></span>
* <span data-ttu-id="e0305-921">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="e0305-921">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="e0305-922">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="e0305-922">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="e0305-923">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="e0305-923">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-924">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-924">Az.Compute</span></span>
* <span data-ttu-id="e0305-925">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-925">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="e0305-926">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-926">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="e0305-927">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="e0305-927">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="e0305-928">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="e0305-928">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="e0305-929">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="e0305-929">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="e0305-930">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="e0305-930">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="e0305-931">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="e0305-931">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="e0305-932">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="e0305-932">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="e0305-933">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="e0305-933">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-934">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-934">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-935">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="e0305-935">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="e0305-936">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="e0305-936">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="e0305-937">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-937">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-938">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="e0305-938">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-939">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-939">Az.IotHub</span></span>
* <span data-ttu-id="e0305-940">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="e0305-940">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="e0305-941">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="e0305-941">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="e0305-942">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="e0305-942">New cmdlets are:</span></span>
    - <span data-ttu-id="e0305-943">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="e0305-943">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="e0305-944">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="e0305-944">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="e0305-945">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="e0305-945">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="e0305-946">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="e0305-946">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-947">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-947">Az.Monitor</span></span>
* <span data-ttu-id="e0305-948">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="e0305-948">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="e0305-949">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="e0305-949">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="e0305-950">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="e0305-950">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="e0305-951">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="e0305-951">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="e0305-952">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="e0305-952">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="e0305-953">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="e0305-953">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="e0305-954">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="e0305-954">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="e0305-955">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="e0305-955">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="e0305-956">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="e0305-956">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="e0305-957">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="e0305-957">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="e0305-958">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="e0305-958">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="e0305-959">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="e0305-959">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="e0305-960">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="e0305-960">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="e0305-961">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="e0305-961">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="e0305-962">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="e0305-962">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="e0305-963">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="e0305-963">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="e0305-964">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="e0305-964">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="e0305-965">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-965">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="e0305-966">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="e0305-966">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="e0305-967">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-967">Overall improved help files</span></span>
* <span data-ttu-id="e0305-968">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="e0305-968">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-969">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-969">Az.Network</span></span>
* <span data-ttu-id="e0305-970">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="e0305-970">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="e0305-971">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="e0305-971">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="e0305-972">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="e0305-972">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="e0305-973">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="e0305-973">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="e0305-974">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="e0305-974">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="e0305-975">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="e0305-975">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="e0305-976">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="e0305-976">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="e0305-977">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="e0305-977">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="e0305-978">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-978">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="e0305-979">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="e0305-979">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="e0305-980">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="e0305-980">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="e0305-981">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="e0305-981">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="e0305-982">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-982">New cmdlets</span></span>
        - <span data-ttu-id="e0305-983">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="e0305-983">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="e0305-984">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-984">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="e0305-985">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="e0305-985">Updated cmdlet:</span></span>
        - <span data-ttu-id="e0305-986">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="e0305-986">New-VpnSite</span></span>
        - <span data-ttu-id="e0305-987">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="e0305-987">Update-VpnSite</span></span>
        - <span data-ttu-id="e0305-988">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-988">New-VpnConnection</span></span>
        - <span data-ttu-id="e0305-989">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-989">Update-VpnConnection</span></span>
* <span data-ttu-id="e0305-990">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="e0305-990">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-991">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-991">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-992">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="e0305-992">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="e0305-993">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="e0305-993">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-994">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-994">Az.Resources</span></span>
* <span data-ttu-id="e0305-995">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="e0305-995">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-996">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-996">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-997">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="e0305-997">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="e0305-998">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="e0305-998">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="e0305-999">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="e0305-999">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="e0305-1000">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="e0305-1000">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="e0305-1001">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="e0305-1001">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="e0305-1002">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="e0305-1002">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="e0305-1003">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="e0305-1003">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="e0305-1004">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="e0305-1004">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="e0305-1005">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="e0305-1005">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="e0305-1006">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="e0305-1006">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="e0305-1007">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="e0305-1007">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="e0305-1008">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="e0305-1008">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="e0305-1009">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="e0305-1009">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="e0305-1010">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="e0305-1010">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="e0305-1011">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="e0305-1011">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="e0305-1012">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="e0305-1012">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="e0305-1013">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="e0305-1013">Az.SignalR</span></span>
* <span data-ttu-id="e0305-1014">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="e0305-1014">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1015">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1015">Az.Sql</span></span>
* <span data-ttu-id="e0305-1016">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="e0305-1016">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="e0305-1017">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="e0305-1017">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="e0305-1018">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1018">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="e0305-1019">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e0305-1019">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="e0305-1020">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="e0305-1020">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1021">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1021">Az.Storage</span></span>
* <span data-ttu-id="e0305-1022">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="e0305-1022">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="e0305-1023">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="e0305-1023">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="e0305-1024">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1024">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="e0305-1025">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1025">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="e0305-1026">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="e0305-1026">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="e0305-1027">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1027">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="e0305-1028">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="e0305-1028">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="e0305-1029">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="e0305-1029">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="e0305-1030">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="e0305-1030">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="e0305-1031">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="e0305-1031">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="e0305-1032">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="e0305-1032">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1033">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1033">Az.Websites</span></span>
* <span data-ttu-id="e0305-1034">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="e0305-1034">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="e0305-1035">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="e0305-1035">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="e0305-1036">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="e0305-1036">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="e0305-1037">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1037">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="e0305-1038">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-1038">General</span></span>
* <span data-ttu-id="e0305-1039">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="e0305-1039">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-1040">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1040">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1041">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="e0305-1041">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="e0305-1042">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="e0305-1042">Az.Aks</span></span>
* <span data-ttu-id="e0305-1043">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="e0305-1043">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="e0305-1044">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="e0305-1044">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="e0305-1045">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-1045">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-1046">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="e0305-1046">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="e0305-1047">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="e0305-1047">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="e0305-1048">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="e0305-1048">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="e0305-1049">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="e0305-1049">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="e0305-1050">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="e0305-1050">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="e0305-1051">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e0305-1051">Az.Batch</span></span>
* <span data-ttu-id="e0305-1052">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="e0305-1052">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-1053">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-1053">Az.Cdn</span></span>
* <span data-ttu-id="e0305-1054">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="e0305-1054">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1055">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1055">Az.Compute</span></span>
* <span data-ttu-id="e0305-1056">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1056">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="e0305-1057">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-1057">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="e0305-1058">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="e0305-1058">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="e0305-1059">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="e0305-1059">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="e0305-1060">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="e0305-1060">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="e0305-1061">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="e0305-1061">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="e0305-1062">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="e0305-1062">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="e0305-1063">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="e0305-1063">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1064">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1064">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1065">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="e0305-1065">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="e0305-1066">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="e0305-1066">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="e0305-1067">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="e0305-1067">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="e0305-1068">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="e0305-1068">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-1069">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-1069">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-1070">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="e0305-1070">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-1071">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1071">Az.EventHub</span></span>
* <span data-ttu-id="e0305-1072">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-1072">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="e0305-1073">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="e0305-1073">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="e0305-1074">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="e0305-1074">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="e0305-1075">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="e0305-1075">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="e0305-1076">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="e0305-1076">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="e0305-1077">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="e0305-1077">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-1078">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-1078">Az.Monitor</span></span>
* <span data-ttu-id="e0305-1079">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-1079">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1080">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1080">Az.Network</span></span>
* <span data-ttu-id="e0305-1081">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="e0305-1081">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="e0305-1082">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="e0305-1082">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="e0305-1083">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="e0305-1083">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="e0305-1084">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="e0305-1084">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="e0305-1085">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="e0305-1085">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="e0305-1086">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="e0305-1086">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="e0305-1087">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="e0305-1087">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-1088">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1088">Az.OperationalInsights</span></span>
* <span data-ttu-id="e0305-1089">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="e0305-1089">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="e0305-1090">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="e0305-1090">Added example</span></span>
    - <span data-ttu-id="e0305-1091">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="e0305-1091">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="e0305-1092">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="e0305-1092">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="e0305-1093">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="e0305-1093">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1094">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1094">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1095">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1095">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1096">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1096">Az.Resources</span></span>
* <span data-ttu-id="e0305-1097">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="e0305-1097">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="e0305-1098">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="e0305-1098">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="e0305-1099">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="e0305-1099">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="e0305-1100">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-1100">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e0305-1101">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e0305-1101">Az.ServiceBus</span></span>
* <span data-ttu-id="e0305-1102">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-1102">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="e0305-1103">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="e0305-1103">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="e0305-1104">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="e0305-1104">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-1105">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-1105">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-1106">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="e0305-1106">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="e0305-1107">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="e0305-1107">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="e0305-1108">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="e0305-1108">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="e0305-1109">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="e0305-1109">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="e0305-1110">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="e0305-1110">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="e0305-1111">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="e0305-1111">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1112">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1112">Az.Sql</span></span>
* <span data-ttu-id="e0305-1113">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="e0305-1113">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1114">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1114">Az.Storage</span></span>
* <span data-ttu-id="e0305-1115">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="e0305-1115">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="e0305-1116">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="e0305-1116">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="e0305-1117">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1117">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="e0305-1118">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="e0305-1118">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="e0305-1119">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="e0305-1119">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="e0305-1120">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="e0305-1120">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1121">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1121">Az.Websites</span></span>
* <span data-ttu-id="e0305-1122">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="e0305-1122">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="e0305-1123">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1123">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1124">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1124">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1125">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="e0305-1125">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="e0305-1126">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1126">Az.ApplicationInsights</span></span>
* <span data-ttu-id="e0305-1127">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="e0305-1127">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1128">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1128">Az.Automation</span></span>
* <span data-ttu-id="e0305-1129">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="e0305-1129">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-1130">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1130">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-1131">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="e0305-1131">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1132">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1132">Az.Compute</span></span>
* <span data-ttu-id="e0305-1133">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="e0305-1133">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="e0305-1134">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="e0305-1134">Az.ContainerRegistry</span></span>
* <span data-ttu-id="e0305-1135">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="e0305-1135">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="e0305-1136">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="e0305-1136">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1137">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1137">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1138">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e0305-1138">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="e0305-1139">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="e0305-1139">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-1140">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1140">Az.EventHub</span></span>
* <span data-ttu-id="e0305-1141">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="e0305-1141">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="e0305-1142">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="e0305-1142">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-1143">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-1143">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-1144">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="e0305-1144">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e0305-1145">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1145">Az.LogicApp</span></span>
* <span data-ttu-id="e0305-1146">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="e0305-1146">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="e0305-1147">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="e0305-1147">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="e0305-1148">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1148">Az.ManagedServices</span></span>
* <span data-ttu-id="e0305-1149">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="e0305-1149">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1150">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1150">Az.Network</span></span>
* <span data-ttu-id="e0305-1151">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="e0305-1151">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="e0305-1152">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1152">New cmdlets</span></span>
        - <span data-ttu-id="e0305-1153">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="e0305-1153">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="e0305-1154">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-1154">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="e0305-1155">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1155">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-1156">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1156">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-1157">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1157">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-1158">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1158">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="e0305-1159">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="e0305-1159">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="e0305-1160">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-1160">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="e0305-1161">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="e0305-1161">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="e0305-1162">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1162">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="e0305-1163">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="e0305-1163">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="e0305-1164">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="e0305-1164">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="e0305-1165">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="e0305-1165">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="e0305-1166">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="e0305-1166">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="e0305-1167">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="e0305-1167">Updated cmdlets</span></span>
        - <span data-ttu-id="e0305-1168">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1168">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="e0305-1169">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1169">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="e0305-1170">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1170">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="e0305-1171">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1171">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="e0305-1172">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1172">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="e0305-1173">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="e0305-1173">Updated cmdlet:</span></span>
        - <span data-ttu-id="e0305-1174">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1174">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="e0305-1175">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1175">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="e0305-1176">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1176">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="e0305-1177">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="e0305-1177">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="e0305-1178">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="e0305-1178">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="e0305-1179">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="e0305-1179">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-1180">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1180">Az.OperationalInsights</span></span>
* <span data-ttu-id="e0305-1181">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="e0305-1181">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="e0305-1182">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="e0305-1182">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1183">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1183">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1184">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1184">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="e0305-1185">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1185">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="e0305-1186">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1186">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="e0305-1187">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1187">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="e0305-1188">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1188">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="e0305-1189">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1189">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="e0305-1190">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1190">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="e0305-1191">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1191">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="e0305-1192">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1192">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="e0305-1193">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="e0305-1193">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1194">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1194">Az.Resources</span></span>
- <span data-ttu-id="e0305-1195">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="e0305-1195">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="e0305-1196">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="e0305-1196">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e0305-1197">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e0305-1197">Az.ServiceBus</span></span>
* <span data-ttu-id="e0305-1198">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="e0305-1198">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="e0305-1199">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="e0305-1199">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1200">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1200">Az.Sql</span></span>
* <span data-ttu-id="e0305-1201">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="e0305-1201">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="e0305-1202">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="e0305-1202">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="e0305-1203">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="e0305-1203">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1204">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1204">Az.Storage</span></span>
* <span data-ttu-id="e0305-1205">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="e0305-1205">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="e0305-1206">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="e0305-1206">Az.StorageSync</span></span>
* <span data-ttu-id="e0305-1207">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="e0305-1207">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="e0305-1208">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="e0305-1208">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1209">Az.Websites</span></span>
* <span data-ttu-id="e0305-1210">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1210">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="e0305-1211">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1211">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="e0305-1212">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1212">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="e0305-1213">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1213">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1214">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1214">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1215">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="e0305-1215">Add support for profile cmdlets</span></span>
* <span data-ttu-id="e0305-1216">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="e0305-1216">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="e0305-1217">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="e0305-1217">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="e0305-1218">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="e0305-1218">Az.Advisor</span></span>
* <span data-ttu-id="e0305-1219">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="e0305-1219">GA release of Az.Advisor</span></span>
* <span data-ttu-id="e0305-1220">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="e0305-1220">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="e0305-1221">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-1221">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-1222">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="e0305-1222">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="e0305-1223">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="e0305-1223">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="e0305-1224">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="e0305-1224">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="e0305-1225">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="e0305-1225">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="e0305-1226">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="e0305-1226">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="e0305-1227">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="e0305-1227">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="e0305-1228">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="e0305-1228">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1229">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1229">Az.Automation</span></span>
* <span data-ttu-id="e0305-1230">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="e0305-1230">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1231">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1231">Az.Compute</span></span>
* <span data-ttu-id="e0305-1232">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1232">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1233">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1234">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="e0305-1234">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="e0305-1235">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="e0305-1235">Az.EventGrid</span></span>
* <span data-ttu-id="e0305-1236">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="e0305-1236">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-1237">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1237">Az.IotHub</span></span>
* <span data-ttu-id="e0305-1238">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="e0305-1238">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1239">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1239">Az.Network</span></span>
* <span data-ttu-id="e0305-1240">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="e0305-1240">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="e0305-1241">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="e0305-1241">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-1242">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1242">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-1243">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="e0305-1243">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="e0305-1244">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="e0305-1244">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-1245">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1245">Az.OperationalInsights</span></span>
* <span data-ttu-id="e0305-1246">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="e0305-1246">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1247">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1248">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="e0305-1248">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1249">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1249">Az.Resources</span></span>
    - <span data-ttu-id="e0305-1250">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="e0305-1250">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="e0305-1251">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="e0305-1251">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="e0305-1252">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="e0305-1252">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="e0305-1253">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="e0305-1253">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e0305-1254">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e0305-1254">Az.ServiceBus</span></span>
* <span data-ttu-id="e0305-1255">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="e0305-1255">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1256">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1256">Az.Sql</span></span>
* <span data-ttu-id="e0305-1257">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="e0305-1257">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="e0305-1258">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1258">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="e0305-1259">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="e0305-1259">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="e0305-1260">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="e0305-1260">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="e0305-1261">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="e0305-1261">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="e0305-1262">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="e0305-1262">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="e0305-1263">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="e0305-1263">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="e0305-1264">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="e0305-1264">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="e0305-1265">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="e0305-1265">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1266">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1266">Az.Storage</span></span>
* <span data-ttu-id="e0305-1267">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e0305-1267">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="e0305-1268">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="e0305-1268">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="e0305-1269">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="e0305-1269">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="e0305-1270">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="e0305-1270">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="e0305-1271">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1271">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="e0305-1272">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1272">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="e0305-1273">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1273">Set-AzStorageAccount</span></span>
* <span data-ttu-id="e0305-1274">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="e0305-1274">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="e0305-1275">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="e0305-1275">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="e0305-1276">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="e0305-1276">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="e0305-1277">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="e0305-1277">Az.StorageSync</span></span>
* <span data-ttu-id="e0305-1278">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="e0305-1278">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="e0305-1279">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1279">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1280">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1280">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1281">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="e0305-1281">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="e0305-1282">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="e0305-1282">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="e0305-1283">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="e0305-1283">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="e0305-1284">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="e0305-1284">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="e0305-1285">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="e0305-1285">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1286">Az.Compute</span></span>
* <span data-ttu-id="e0305-1287">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="e0305-1287">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="e0305-1288">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="e0305-1288">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="e0305-1289">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="e0305-1289">Az.Dns</span></span>
* <span data-ttu-id="e0305-1290">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="e0305-1290">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="e0305-1291">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="e0305-1291">Az.EventGrid</span></span>
* <span data-ttu-id="e0305-1292">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="e0305-1292">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="e0305-1293">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-1293">New cmdlets:</span></span>
    - <span data-ttu-id="e0305-1294">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="e0305-1294">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="e0305-1295">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="e0305-1295">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="e0305-1296">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="e0305-1296">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="e0305-1297">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-1297">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="e0305-1298">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="e0305-1298">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="e0305-1299">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="e0305-1299">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="e0305-1300">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="e0305-1300">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="e0305-1301">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="e0305-1301">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="e0305-1302">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="e0305-1302">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="e0305-1303">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="e0305-1303">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="e0305-1304">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="e0305-1304">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="e0305-1305">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="e0305-1305">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="e0305-1306">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="e0305-1306">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="e0305-1307">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="e0305-1307">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="e0305-1308">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="e0305-1308">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="e0305-1309">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="e0305-1309">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="e0305-1310">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="e0305-1310">Updated cmdlets:</span></span>
    - <span data-ttu-id="e0305-1311">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="e0305-1311">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="e0305-1312">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1312">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="e0305-1313">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1313">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="e0305-1314">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="e0305-1314">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="e0305-1315">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="e0305-1315">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="e0305-1316">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="e0305-1316">Event subscription expiration date,</span></span>
            - <span data-ttu-id="e0305-1317">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="e0305-1317">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="e0305-1318">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="e0305-1318">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="e0305-1319">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="e0305-1319">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="e0305-1320">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="e0305-1320">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="e0305-1321">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="e0305-1321">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="e0305-1322">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="e0305-1322">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="e0305-1323">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1323">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="e0305-1324">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1324">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="e0305-1325">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-1325">Az.FrontDoor</span></span>
* <span data-ttu-id="e0305-1326">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="e0305-1326">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="e0305-1327">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="e0305-1327">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="e0305-1328">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="e0305-1328">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="e0305-1329">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="e0305-1329">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1330">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1330">Az.Network</span></span>
* <span data-ttu-id="e0305-1331">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="e0305-1331">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="e0305-1332">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1332">New cmdlets</span></span>
        - <span data-ttu-id="e0305-1333">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="e0305-1333">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="e0305-1334">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="e0305-1334">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="e0305-1335">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1335">New cmdlets</span></span>
        - <span data-ttu-id="e0305-1336">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="e0305-1336">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="e0305-1337">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-1337">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="e0305-1338">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1338">New cmdlets</span></span>
        - <span data-ttu-id="e0305-1339">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-1339">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="e0305-1340">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-1340">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="e0305-1341">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="e0305-1341">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="e0305-1342">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1342">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="e0305-1343">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1343">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="e0305-1344">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="e0305-1344">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="e0305-1345">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1345">New cmdlets</span></span>
        - <span data-ttu-id="e0305-1346">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="e0305-1346">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="e0305-1347">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="e0305-1347">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="e0305-1348">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="e0305-1348">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="e0305-1349">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1349">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="e0305-1350">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="e0305-1350">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="e0305-1351">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="e0305-1351">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="e0305-1352">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="e0305-1352">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="e0305-1353">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="e0305-1353">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="e0305-1354">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="e0305-1354">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="e0305-1355">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="e0305-1355">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="e0305-1356">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1356">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="e0305-1357">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="e0305-1357">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="e0305-1358">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1358">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="e0305-1359">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="e0305-1359">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="e0305-1360">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1360">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="e0305-1361">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1361">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="e0305-1362">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="e0305-1362">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="e0305-1363">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="e0305-1363">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="e0305-1364">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="e0305-1364">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="e0305-1365">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="e0305-1365">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="e0305-1366">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="e0305-1366">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="e0305-1367">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="e0305-1367">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="e0305-1368">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="e0305-1368">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="e0305-1369">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="e0305-1369">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="e0305-1370">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1370">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="e0305-1371">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1371">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="e0305-1372">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1372">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-1373">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1373">Az.OperationalInsights</span></span>
* <span data-ttu-id="e0305-1374">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="e0305-1374">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1375">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1375">Az.Resources</span></span>
* <span data-ttu-id="e0305-1376">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="e0305-1376">Support for additional Template Export options</span></span>
    - <span data-ttu-id="e0305-1377">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-1377">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="e0305-1378">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-1378">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="e0305-1379">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="e0305-1379">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-1380">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-1380">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-1381">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="e0305-1381">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1382">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1382">Az.Sql</span></span>
* <span data-ttu-id="e0305-1383">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="e0305-1383">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="e0305-1384">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="e0305-1384">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="e0305-1385">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="e0305-1385">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="e0305-1386">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="e0305-1386">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="e0305-1387">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="e0305-1387">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="e0305-1388">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="e0305-1388">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="e0305-1389">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="e0305-1389">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="e0305-1390">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="e0305-1390">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1391">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1391">Az.Storage</span></span>
* <span data-ttu-id="e0305-1392">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e0305-1392">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="e0305-1393">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1393">New-AzStorageAccount</span></span>
* <span data-ttu-id="e0305-1394">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="e0305-1394">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="e0305-1395">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1395">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1396">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1396">Az.Websites</span></span>
* <span data-ttu-id="e0305-1397">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="e0305-1397">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="e0305-1398">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="e0305-1398">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="e0305-1399">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1399">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="e0305-1400">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-1400">Az.Cdn</span></span>
* <span data-ttu-id="e0305-1401">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="e0305-1401">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1402">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1402">Az.Compute</span></span>
* <span data-ttu-id="e0305-1403">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="e0305-1403">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="e0305-1404">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="e0305-1404">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-1405">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1405">Az.EventHub</span></span>
* <span data-ttu-id="e0305-1406">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="e0305-1406">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="e0305-1407">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="e0305-1407">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1408">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1408">Az.Network</span></span>
* <span data-ttu-id="e0305-1409">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1409">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="e0305-1410">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="e0305-1410">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-1411">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1411">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-1412">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="e0305-1412">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1413">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1413">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1414">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="e0305-1414">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e0305-1415">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e0305-1415">Az.ServiceBus</span></span>
* <span data-ttu-id="e0305-1416">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="e0305-1416">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-1417">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-1417">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-1418">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="e0305-1418">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="e0305-1419">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e0305-1419">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1420">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1420">Az.Sql</span></span>
* <span data-ttu-id="e0305-1421">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="e0305-1421">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="e0305-1422">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1422">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="e0305-1423">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="e0305-1423">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="e0305-1424">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="e0305-1424">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1425">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1425">Az.Websites</span></span>
* <span data-ttu-id="e0305-1426">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="e0305-1426">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="e0305-1427">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1427">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="e0305-1428">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-1428">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-1429">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="e0305-1429">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="e0305-1430">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="e0305-1430">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="e0305-1431">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="e0305-1431">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="e0305-1432">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="e0305-1432">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="e0305-1433">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1433">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="e0305-1434">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e0305-1434">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="e0305-1435">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="e0305-1435">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="e0305-1436">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="e0305-1436">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="e0305-1437">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-1437">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="e0305-1438">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="e0305-1438">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="e0305-1439">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="e0305-1439">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="e0305-1440">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="e0305-1440">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="e0305-1441">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="e0305-1441">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="e0305-1442">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="e0305-1442">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="e0305-1443">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="e0305-1443">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="e0305-1444">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="e0305-1444">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="e0305-1445">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="e0305-1445">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="e0305-1446">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="e0305-1446">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="e0305-1447">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="e0305-1447">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="e0305-1448">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="e0305-1448">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="e0305-1449">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="e0305-1449">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="e0305-1450">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="e0305-1450">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="e0305-1451">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="e0305-1451">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="e0305-1452">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-1452">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="e0305-1453">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="e0305-1453">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="e0305-1454">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="e0305-1454">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="e0305-1455">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="e0305-1455">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="e0305-1456">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="e0305-1456">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="e0305-1457">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="e0305-1457">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="e0305-1458">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="e0305-1458">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="e0305-1459">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="e0305-1459">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="e0305-1460">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="e0305-1460">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="e0305-1461">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="e0305-1461">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="e0305-1462">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="e0305-1462">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="e0305-1463">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="e0305-1463">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="e0305-1464">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="e0305-1464">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="e0305-1465">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="e0305-1465">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="e0305-1466">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="e0305-1466">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="e0305-1467">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="e0305-1467">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="e0305-1468">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="e0305-1468">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="e0305-1469">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="e0305-1469">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="e0305-1470">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="e0305-1470">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="e0305-1471">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="e0305-1471">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="e0305-1472">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="e0305-1472">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="e0305-1473">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="e0305-1473">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="e0305-1474">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="e0305-1474">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="e0305-1475">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="e0305-1475">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="e0305-1476">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="e0305-1476">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="e0305-1477">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="e0305-1477">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="e0305-1478">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="e0305-1478">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="e0305-1479">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="e0305-1479">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="e0305-1480">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="e0305-1480">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="e0305-1481">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="e0305-1481">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="e0305-1482">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="e0305-1482">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="e0305-1483">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="e0305-1483">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="e0305-1484">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="e0305-1484">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="e0305-1485">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="e0305-1485">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="e0305-1486">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="e0305-1486">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="e0305-1487">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="e0305-1487">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="e0305-1488">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="e0305-1488">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="e0305-1489">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="e0305-1489">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="e0305-1490">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="e0305-1490">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="e0305-1491">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="e0305-1491">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="e0305-1492">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="e0305-1492">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="e0305-1493">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="e0305-1493">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="e0305-1494">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="e0305-1494">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="e0305-1495">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="e0305-1495">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="e0305-1496">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="e0305-1496">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="e0305-1497">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="e0305-1497">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="e0305-1498">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="e0305-1498">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="e0305-1499">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="e0305-1499">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="e0305-1500">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="e0305-1500">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="e0305-1501">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="e0305-1501">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="e0305-1502">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="e0305-1502">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="e0305-1503">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="e0305-1503">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="e0305-1504">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="e0305-1504">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="e0305-1505">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="e0305-1505">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1506">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1506">Az.Automation</span></span>
* <span data-ttu-id="e0305-1507">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="e0305-1507">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="e0305-1508">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="e0305-1508">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="e0305-1509">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="e0305-1509">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="e0305-1510">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="e0305-1510">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="e0305-1511">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="e0305-1511">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="e0305-1512">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="e0305-1512">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="e0305-1513">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="e0305-1513">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1514">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1514">Az.Compute</span></span>
* <span data-ttu-id="e0305-1515">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="e0305-1515">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="e0305-1516">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="e0305-1516">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-1517">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-1517">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-1518">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1518">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-1519">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-1519">Az.Monitor</span></span>
* <span data-ttu-id="e0305-1520">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-1520">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1521">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1521">Az.Network</span></span>
* <span data-ttu-id="e0305-1522">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="e0305-1522">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="e0305-1523">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="e0305-1523">Updated cmdlet:</span></span>
        - <span data-ttu-id="e0305-1524">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="e0305-1524">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="e0305-1525">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e0305-1525">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1526">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1526">Az.Resources</span></span>
* <span data-ttu-id="e0305-1527">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="e0305-1527">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1528">Az.Sql</span></span>
* <span data-ttu-id="e0305-1529">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="e0305-1529">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="e0305-1530">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1530">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1531">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1531">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1532">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="e0305-1532">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-1533">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1533">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-1534">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="e0305-1534">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="e0305-1535">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="e0305-1535">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1536">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1536">Az.Compute</span></span>
* <span data-ttu-id="e0305-1537">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="e0305-1537">Proximity placement group feature.</span></span>
    - <span data-ttu-id="e0305-1538">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-1538">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="e0305-1539">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1539">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="e0305-1540">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="e0305-1540">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="e0305-1541">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="e0305-1541">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="e0305-1542">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-1542">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="e0305-1543">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="e0305-1543">Breaking changes</span></span>
    - <span data-ttu-id="e0305-1544">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="e0305-1544">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="e0305-1545">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="e0305-1545">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="e0305-1546">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="e0305-1546">Az.DeploymentManager</span></span>
* <span data-ttu-id="e0305-1547">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1547">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="e0305-1548">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="e0305-1548">Az.Dns</span></span>
* <span data-ttu-id="e0305-1549">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="e0305-1549">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="e0305-1550">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="e0305-1550">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="e0305-1551">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="e0305-1551">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="e0305-1552">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-1552">Az.FrontDoor</span></span>
* <span data-ttu-id="e0305-1553">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="e0305-1553">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="e0305-1554">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="e0305-1554">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="e0305-1555">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-1555">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-1556">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-1556">Removed two cmdlets:</span></span>
    - <span data-ttu-id="e0305-1557">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="e0305-1557">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="e0305-1558">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="e0305-1558">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="e0305-1559">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="e0305-1559">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="e0305-1560">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="e0305-1560">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="e0305-1561">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="e0305-1561">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="e0305-1562">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="e0305-1562">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-1563">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-1563">Az.Monitor</span></span>
* <span data-ttu-id="e0305-1564">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="e0305-1564">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="e0305-1565">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="e0305-1565">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="e0305-1566">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-1566">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="e0305-1567">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="e0305-1567">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="e0305-1568">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="e0305-1568">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="e0305-1569">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="e0305-1569">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="e0305-1570">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="e0305-1570">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="e0305-1571">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="e0305-1571">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="e0305-1572">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="e0305-1572">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="e0305-1573">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="e0305-1573">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="e0305-1574">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="e0305-1574">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="e0305-1575">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="e0305-1575">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="e0305-1576">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="e0305-1576">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="e0305-1577">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="e0305-1577">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1578">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1578">Az.Network</span></span>
* <span data-ttu-id="e0305-1579">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="e0305-1579">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="e0305-1580">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1580">New cmdlets</span></span>
        - <span data-ttu-id="e0305-1581">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1581">New-AzNatGateway</span></span>
        - <span data-ttu-id="e0305-1582">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1582">Get-AzNatGateway</span></span>
        - <span data-ttu-id="e0305-1583">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1583">Set-AzNatGateway</span></span>
        - <span data-ttu-id="e0305-1584">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-1584">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="e0305-1585">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="e0305-1585">Updated cmdlets</span></span>
        - <span data-ttu-id="e0305-1586">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="e0305-1586">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="e0305-1587">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="e0305-1587">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="e0305-1588">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1588">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="e0305-1589">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1589">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="e0305-1590">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="e0305-1590">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-1591">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1591">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-1592">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="e0305-1592">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="e0305-1593">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="e0305-1593">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="e0305-1594">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="e0305-1594">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1595">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1595">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1596">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="e0305-1596">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="e0305-1597">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="e0305-1597">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="e0305-1598">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="e0305-1598">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="e0305-1599">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-1599">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="e0305-1600">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1600">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="e0305-1601">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="e0305-1601">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="e0305-1602">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="e0305-1602">Az.Relay</span></span>
* <span data-ttu-id="e0305-1603">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="e0305-1603">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e0305-1604">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e0305-1604">Az.ServiceBus</span></span>
* <span data-ttu-id="e0305-1605">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="e0305-1605">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1606">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1606">Az.Storage</span></span>
* <span data-ttu-id="e0305-1607">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="e0305-1607">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="e0305-1608">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="e0305-1608">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="e0305-1609">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="e0305-1609">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="e0305-1610">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1610">New-AzStorageAccount</span></span>
* <span data-ttu-id="e0305-1611">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="e0305-1611">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="e0305-1612">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1612">New-AzStorageAccount</span></span>
    - <span data-ttu-id="e0305-1613">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1613">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="e0305-1614">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1614">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1615">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1615">Az.Websites</span></span>
* <span data-ttu-id="e0305-1616">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1616">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="e0305-1617">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="e0305-1617">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="e0305-1618">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1618">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="e0305-1619">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="e0305-1619">Highlights since the last major release</span></span>
* <span data-ttu-id="e0305-1620">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="e0305-1620">General availability of `Az` module</span></span>
* <span data-ttu-id="e0305-1621">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="e0305-1621">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="e0305-1622">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="e0305-1622">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="e0305-1623">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1623">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="e0305-1624">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="e0305-1624">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="e0305-1625">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1625">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="e0305-1626">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="e0305-1626">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-1627">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1627">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1628">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="e0305-1628">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="e0305-1629">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e0305-1629">Az.Batch</span></span>
* <span data-ttu-id="e0305-1630">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1630">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-1631">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-1631">Az.Cdn</span></span>
* <span data-ttu-id="e0305-1632">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1632">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-1633">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1633">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-1634">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1634">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1635">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1635">Az.Compute</span></span>
* <span data-ttu-id="e0305-1636">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="e0305-1636">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="e0305-1637">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1637">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="e0305-1638">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="e0305-1638">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1639">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1639">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1640">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="e0305-1640">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-1641">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-1641">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-1642">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1642">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="e0305-1643">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="e0305-1643">Az.EventGrid</span></span>
* <span data-ttu-id="e0305-1644">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="e0305-1644">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-1645">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1645">Az.EventHub</span></span>
* <span data-ttu-id="e0305-1646">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="e0305-1646">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="e0305-1647">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="e0305-1647">Az.HDInsight</span></span>
* <span data-ttu-id="e0305-1648">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1648">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-1649">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1649">Az.IotHub</span></span>
* <span data-ttu-id="e0305-1650">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1650">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-1651">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-1651">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-1652">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1652">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="e0305-1653">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="e0305-1653">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="e0305-1654">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="e0305-1654">Az.MachineLearning</span></span>
* <span data-ttu-id="e0305-1655">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1655">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="e0305-1656">Az.Media</span><span class="sxs-lookup"><span data-stu-id="e0305-1656">Az.Media</span></span>
* <span data-ttu-id="e0305-1657">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1657">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-1658">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-1658">Az.Monitor</span></span>
  * <span data-ttu-id="e0305-1659">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="e0305-1659">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="e0305-1660">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="e0305-1660">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="e0305-1661">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="e0305-1661">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="e0305-1662">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="e0305-1662">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="e0305-1663">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="e0305-1663">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="e0305-1664">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="e0305-1664">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="e0305-1665">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="e0305-1665">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1666">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1666">Az.Network</span></span>
* <span data-ttu-id="e0305-1667">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1667">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="e0305-1668">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="e0305-1668">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="e0305-1669">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="e0305-1669">Az.NotificationHubs</span></span>
* <span data-ttu-id="e0305-1670">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1670">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-1671">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1671">Az.OperationalInsights</span></span>
* <span data-ttu-id="e0305-1672">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1672">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="e0305-1673">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="e0305-1673">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="e0305-1674">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1674">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1675">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1675">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1676">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1676">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="e0305-1677">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1677">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="e0305-1678">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="e0305-1678">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="e0305-1679">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="e0305-1679">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="e0305-1680">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="e0305-1680">Az.RedisCache</span></span>
* <span data-ttu-id="e0305-1681">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1681">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1682">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1682">Az.Resources</span></span>
* <span data-ttu-id="e0305-1683">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="e0305-1683">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1684">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1684">Az.Sql</span></span>
* <span data-ttu-id="e0305-1685">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="e0305-1685">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="e0305-1686">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1686">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="e0305-1687">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="e0305-1687">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="e0305-1688">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="e0305-1688">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="e0305-1689">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="e0305-1689">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="e0305-1690">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="e0305-1690">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="e0305-1691">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="e0305-1691">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1692">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1692">Az.Websites</span></span>
* <span data-ttu-id="e0305-1693">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="e0305-1693">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="e0305-1694">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="e0305-1694">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="e0305-1695">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="e0305-1695">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="e0305-1696">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="e0305-1696">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="e0305-1697">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1697">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="e0305-1698">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="e0305-1698">Highlights since the last major release</span></span>
* <span data-ttu-id="e0305-1699">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="e0305-1699">General availability of `Az` module</span></span>
* <span data-ttu-id="e0305-1700">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="e0305-1700">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="e0305-1701">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="e0305-1701">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="e0305-1702">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1702">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="e0305-1703">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="e0305-1703">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="e0305-1704">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1704">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="e0305-1705">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="e0305-1705">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="e0305-1706">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1706">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1707">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="e0305-1707">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="e0305-1708">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1708">Az.AnalysisServices</span></span>
* <span data-ttu-id="e0305-1709">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="e0305-1709">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="e0305-1710">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="e0305-1710">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1711">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1711">Az.Automation</span></span>
* <span data-ttu-id="e0305-1712">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="e0305-1712">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="e0305-1713">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="e0305-1713">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="e0305-1714">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1714">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1715">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1715">Az.Compute</span></span>
* <span data-ttu-id="e0305-1716">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-1716">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="e0305-1717">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="e0305-1717">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="e0305-1718">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-1718">Az.ContainerInstance</span></span>
* <span data-ttu-id="e0305-1719">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="e0305-1719">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1720">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1720">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1721">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="e0305-1721">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="e0305-1722">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e0305-1722">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1723">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1723">Az.Resources</span></span>
* <span data-ttu-id="e0305-1724">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="e0305-1724">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="e0305-1725">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="e0305-1725">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="e0305-1726">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="e0305-1726">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="e0305-1727">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="e0305-1727">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="e0305-1728">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="e0305-1728">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="e0305-1729">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="e0305-1729">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1730">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1730">Az.Sql</span></span>
* <span data-ttu-id="e0305-1731">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="e0305-1731">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1732">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1732">Az.Storage</span></span>
* <span data-ttu-id="e0305-1733">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1733">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="e0305-1734">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="e0305-1734">New-AzStorageContext</span></span>
* <span data-ttu-id="e0305-1735">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="e0305-1735">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="e0305-1736">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="e0305-1736">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="e0305-1737">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="e0305-1737">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="e0305-1738">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1738">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="e0305-1739">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1739">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="e0305-1740">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="e0305-1740">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="e0305-1741">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1741">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="e0305-1742">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1742">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="e0305-1743">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1743">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="e0305-1744">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="e0305-1744">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="e0305-1745">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1745">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="e0305-1746">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="e0305-1746">Highlights since the last major release</span></span>
* <span data-ttu-id="e0305-1747">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="e0305-1747">General availability of `Az` module</span></span>
* <span data-ttu-id="e0305-1748">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="e0305-1748">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="e0305-1749">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="e0305-1749">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="e0305-1750">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1750">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="e0305-1751">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="e0305-1751">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="e0305-1752">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1752">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="e0305-1753">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="e0305-1753">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1754">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1754">Az.Automation</span></span>
* <span data-ttu-id="e0305-1755">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="e0305-1755">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="e0305-1756">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="e0305-1756">Dynamic grouping</span></span>
    * <span data-ttu-id="e0305-1757">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="e0305-1757">Pre-Post script</span></span>
    * <span data-ttu-id="e0305-1758">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="e0305-1758">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1759">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1759">Az.Compute</span></span>
* <span data-ttu-id="e0305-1760">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="e0305-1760">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="e0305-1761">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="e0305-1761">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-1762">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-1762">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-1763">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-1763">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1764">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1764">Az.Network</span></span>
* <span data-ttu-id="e0305-1765">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="e0305-1765">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="e0305-1766">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="e0305-1766">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1767">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1767">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1768">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="e0305-1768">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="e0305-1769">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="e0305-1769">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1770">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1770">Az.Resources</span></span>
* <span data-ttu-id="e0305-1771">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-1771">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="e0305-1772">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="e0305-1772">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1773">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1773">Az.Sql</span></span>
* <span data-ttu-id="e0305-1774">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="e0305-1774">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1775">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1775">Az.Storage</span></span>
* <span data-ttu-id="e0305-1776">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e0305-1776">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="e0305-1777">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1777">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="e0305-1778">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1778">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="e0305-1779">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1779">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="e0305-1780">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="e0305-1780">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="e0305-1781">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="e0305-1781">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="e0305-1782">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="e0305-1782">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1783">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1783">Az.Websites</span></span>
* <span data-ttu-id="e0305-1784">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="e0305-1784">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="e0305-1785">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1785">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1786">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1786">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1787">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="e0305-1787">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="e0305-1788">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1788">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1789">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1789">Az.Automation</span></span>
* <span data-ttu-id="e0305-1790">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1790">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="e0305-1791">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="e0305-1791">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="e0305-1792">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="e0305-1792">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-1793">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-1793">Az.Cdn</span></span>
* <span data-ttu-id="e0305-1794">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="e0305-1794">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1795">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1795">Az.Compute</span></span>
* <span data-ttu-id="e0305-1796">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="e0305-1796">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1797">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1797">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1798">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="e0305-1798">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e0305-1799">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1799">Az.LogicApp</span></span>
* <span data-ttu-id="e0305-1800">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="e0305-1800">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1801">Az.Network</span></span>
* <span data-ttu-id="e0305-1802">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1802">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1803">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1803">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1804">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-1804">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="e0305-1805">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="e0305-1805">SDK Update</span></span>
* <span data-ttu-id="e0305-1806">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="e0305-1806">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="e0305-1807">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="e0305-1807">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1808">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1808">Az.Resources</span></span>
* <span data-ttu-id="e0305-1809">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="e0305-1809">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="e0305-1810">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="e0305-1810">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="e0305-1811">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="e0305-1811">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="e0305-1812">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="e0305-1812">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="e0305-1813">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="e0305-1813">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="e0305-1814">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="e0305-1814">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1815">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1815">Az.Sql</span></span>
* <span data-ttu-id="e0305-1816">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="e0305-1816">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="e0305-1817">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="e0305-1817">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1818">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1818">Az.Storage</span></span>
* <span data-ttu-id="e0305-1819">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-1819">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="e0305-1820">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1820">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="e0305-1821">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1821">Az.AnalysisServices</span></span>
* <span data-ttu-id="e0305-1822">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="e0305-1822">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1823">Az.Automation</span></span>
* <span data-ttu-id="e0305-1824">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1824">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="e0305-1825">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1825">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="e0305-1826">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1826">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-1827">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1827">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-1828">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="e0305-1828">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1829">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1829">Az.Compute</span></span>
* <span data-ttu-id="e0305-1830">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="e0305-1830">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="e0305-1831">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="e0305-1831">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="e0305-1832">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="e0305-1832">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="e0305-1833">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="e0305-1833">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-1834">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-1834">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-1835">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="e0305-1835">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e0305-1836">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1836">Az.EventHub</span></span>
* <span data-ttu-id="e0305-1837">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="e0305-1837">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-1838">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-1838">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-1839">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="e0305-1839">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e0305-1840">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1840">Az.LogicApp</span></span>
* <span data-ttu-id="e0305-1841">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="e0305-1841">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="e0305-1842">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="e0305-1842">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="e0305-1843">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="e0305-1843">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="e0305-1844">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e0305-1844">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="e0305-1845">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e0305-1845">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="e0305-1846">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e0305-1846">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="e0305-1847">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e0305-1847">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="e0305-1848">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="e0305-1848">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="e0305-1849">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1849">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="e0305-1850">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1850">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="e0305-1851">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1851">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="e0305-1852">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-1852">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="e0305-1853">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e0305-1853">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e0305-1854">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-1854">Az.Monitor</span></span>
* <span data-ttu-id="e0305-1855">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="e0305-1855">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1856">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1856">Az.Network</span></span>
* <span data-ttu-id="e0305-1857">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="e0305-1857">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-1858">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-1858">Az.OperationalInsights</span></span>
* <span data-ttu-id="e0305-1859">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="e0305-1859">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="e0305-1860">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0305-1860">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="e0305-1861">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="e0305-1861">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1862">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1862">Az.Resources</span></span>
* <span data-ttu-id="e0305-1863">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="e0305-1863">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="e0305-1864">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="e0305-1864">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="e0305-1865">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="e0305-1865">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="e0305-1866">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="e0305-1866">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1867">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1867">Az.Sql</span></span>
* <span data-ttu-id="e0305-1868">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="e0305-1868">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="e0305-1869">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="e0305-1869">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1870">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1870">Az.Websites</span></span>
* <span data-ttu-id="e0305-1871">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="e0305-1871">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="e0305-1872">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1872">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1873">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1873">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1874">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="e0305-1874">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="e0305-1875">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1875">Az.AnalysisServices</span></span>
<span data-ttu-id="e0305-1876">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="e0305-1876">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1877">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1877">Az.Compute</span></span>
* <span data-ttu-id="e0305-1878">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="e0305-1878">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="e0305-1879">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="e0305-1879">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="e0305-1880">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="e0305-1880">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1881">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1881">Az.RecoveryServices</span></span>
<span data-ttu-id="e0305-1882">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="e0305-1882">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1883">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1883">Az.Resources</span></span>
* <span data-ttu-id="e0305-1884">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="e0305-1884">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="e0305-1885">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="e0305-1885">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="e0305-1886">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="e0305-1886">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="e0305-1887">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="e0305-1887">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1888">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1888">Az.Sql</span></span>
* <span data-ttu-id="e0305-1889">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0305-1889">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="e0305-1890">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="e0305-1890">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="e0305-1891">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="e0305-1891">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="e0305-1892">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1892">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1893">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1893">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1894">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="e0305-1894">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="e0305-1895">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1895">Az.AnalysisServices</span></span>
* <span data-ttu-id="e0305-1896">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="e0305-1896">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-1897">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-1897">Az.RecoveryServices</span></span>
* <span data-ttu-id="e0305-1898">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="e0305-1898">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="e0305-1899">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1899">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1900">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1900">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1901">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="e0305-1901">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="e0305-1902">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1902">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e0305-1903">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="e0305-1903">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="e0305-1904">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="e0305-1904">Az.Aks</span></span>
* <span data-ttu-id="e0305-1905">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1905">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e0305-1906">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-1906">Az.Automation</span></span>
* <span data-ttu-id="e0305-1907">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="e0305-1907">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="e0305-1908">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1908">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e0305-1909">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e0305-1909">Az.Cdn</span></span>
* <span data-ttu-id="e0305-1910">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1910">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1911">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1911">Az.Compute</span></span>
* <span data-ttu-id="e0305-1912">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="e0305-1912">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="e0305-1913">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="e0305-1913">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="e0305-1914">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="e0305-1914">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="e0305-1915">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="e0305-1915">Az.ContainerRegistry</span></span>
* <span data-ttu-id="e0305-1916">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1916">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e0305-1917">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e0305-1917">Az.DataFactory</span></span>
* <span data-ttu-id="e0305-1918">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="e0305-1918">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-1919">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-1919">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-1920">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="e0305-1920">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="e0305-1921">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="e0305-1921">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="e0305-1922">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1922">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-1923">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1923">Az.IotHub</span></span>
* <span data-ttu-id="e0305-1924">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="e0305-1924">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e0305-1925">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-1925">Az.KeyVault</span></span>
* <span data-ttu-id="e0305-1926">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1926">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-1927">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-1927">Az.Network</span></span>
* <span data-ttu-id="e0305-1928">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1928">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1929">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1929">Az.Resources</span></span>
* <span data-ttu-id="e0305-1930">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="e0305-1930">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="e0305-1931">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="e0305-1931">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="e0305-1932">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="e0305-1932">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="e0305-1933">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="e0305-1933">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="e0305-1934">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="e0305-1934">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="e0305-1935">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="e0305-1935">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="e0305-1936">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="e0305-1936">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-1937">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-1937">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-1938">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="e0305-1938">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="e0305-1939">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="e0305-1939">Fix some error messages.</span></span>
* <span data-ttu-id="e0305-1940">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="e0305-1940">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="e0305-1941">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="e0305-1941">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="e0305-1942">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="e0305-1942">Az.SignalR</span></span>
* <span data-ttu-id="e0305-1943">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1943">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1944">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1944">Az.Sql</span></span>
* <span data-ttu-id="e0305-1945">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1945">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e0305-1946">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="e0305-1946">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="e0305-1947">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="e0305-1947">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="e0305-1948">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="e0305-1948">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1949">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1949">Az.Storage</span></span>
* <span data-ttu-id="e0305-1950">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1950">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e0305-1951">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="e0305-1951">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="e0305-1952">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="e0305-1952">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="e0305-1953">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="e0305-1953">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="e0305-1954">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="e0305-1954">Az.TrafficManager</span></span>
* <span data-ttu-id="e0305-1955">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1955">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-1956">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-1956">Az.Websites</span></span>
* <span data-ttu-id="e0305-1957">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="e0305-1957">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e0305-1958">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="e0305-1958">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="e0305-1959">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="e0305-1959">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="e0305-1960">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e0305-1960">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e0305-1961">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1961">Az.Accounts</span></span>
* <span data-ttu-id="e0305-1962">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="e0305-1962">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-1963">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-1963">Az.Compute</span></span>
* <span data-ttu-id="e0305-1964">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="e0305-1964">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="e0305-1965">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="e0305-1965">Updated the description of ID in help files</span></span>
* <span data-ttu-id="e0305-1966">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1966">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-1967">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-1967">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-1968">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="e0305-1968">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="e0305-1969">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="e0305-1969">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="e0305-1970">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="e0305-1970">Az.EventGrid</span></span>
* <span data-ttu-id="e0305-1971">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="e0305-1971">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="e0305-1972">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="e0305-1972">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="e0305-1973">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="e0305-1973">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="e0305-1974">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="e0305-1974">Event Time-To-Live,</span></span>
        - <span data-ttu-id="e0305-1975">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="e0305-1975">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="e0305-1976">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="e0305-1976">Dead letter endpoint.</span></span>
    - <span data-ttu-id="e0305-1977">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="e0305-1977">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="e0305-1978">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="e0305-1978">Event Time-To-Live,</span></span>
        - <span data-ttu-id="e0305-1979">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="e0305-1979">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="e0305-1980">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="e0305-1980">Dead letter endpoint.</span></span>
* <span data-ttu-id="e0305-1981">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="e0305-1981">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="e0305-1982">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="e0305-1982">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e0305-1983">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1983">Az.IotHub</span></span>
* <span data-ttu-id="e0305-1984">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="e0305-1984">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e0305-1985">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e0305-1985">Az.LogicApp</span></span>
* <span data-ttu-id="e0305-1986">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="e0305-1986">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-1987">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-1987">Az.Resources</span></span>
* <span data-ttu-id="e0305-1988">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="e0305-1988">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="e0305-1989">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="e0305-1989">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="e0305-1990">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="e0305-1990">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="e0305-1991">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="e0305-1991">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="e0305-1992">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="e0305-1992">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="e0305-1993">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="e0305-1993">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="e0305-1994">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="e0305-1994">Az.SignalR</span></span>
* <span data-ttu-id="e0305-1995">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-1995">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-1996">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-1996">Az.Sql</span></span>
* <span data-ttu-id="e0305-1997">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="e0305-1997">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e0305-1998">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-1998">Az.Storage</span></span>
* <span data-ttu-id="e0305-1999">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="e0305-1999">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="e0305-2000">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="e0305-2000">New-AzStorageContext</span></span>
* <span data-ttu-id="e0305-2001">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="e0305-2001">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="e0305-2002">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="e0305-2002">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-2003">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-2003">Az.Websites</span></span>
* <span data-ttu-id="e0305-2004">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="e0305-2004">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="e0305-2005">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-2005">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="e0305-2006">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2006">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="e0305-2007">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-2007">General</span></span>

- <span data-ttu-id="e0305-2008">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="e0305-2008">General Availability of Az Module</span></span>
- <span data-ttu-id="e0305-2009">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="e0305-2009">Online help for each module</span></span>
- <span data-ttu-id="e0305-2010">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="e0305-2010">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="e0305-2011">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="e0305-2011">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="e0305-2012">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-2012">Az.Accounts</span></span>
- <span data-ttu-id="e0305-2013">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e0305-2013">Changed from Az.Profile</span></span>
- <span data-ttu-id="e0305-2014">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="e0305-2014">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="e0305-2015">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-2015">Az.ApiManagement</span></span>
- <span data-ttu-id="e0305-2016">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="e0305-2016">Fixes for #7002</span></span>
- <span data-ttu-id="e0305-2017">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2017">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="e0305-2018">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e0305-2018">Az.Batch</span></span>
- <span data-ttu-id="e0305-2019">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="e0305-2019">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="e0305-2020">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="e0305-2020">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="e0305-2021">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2021">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="e0305-2022">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="e0305-2022">Az.Billing</span></span>
- <span data-ttu-id="e0305-2023">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2023">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="e0305-2024">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="e0305-2024">Az.CognitivServices</span></span>
- <span data-ttu-id="e0305-2025">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-2025">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="e0305-2026">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="e0305-2026">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="e0305-2027">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-2027">Az.ContainerInstance</span></span>
- <span data-ttu-id="e0305-2028">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="e0305-2028">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="e0305-2029">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="e0305-2029">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="e0305-2030">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2030">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="e0305-2031">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-2031">Az.DataLakeStore</span></span>
- <span data-ttu-id="e0305-2032">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2032">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="e0305-2033">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e0305-2033">Az.Monitor</span></span>
- <span data-ttu-id="e0305-2034">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2034">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="e0305-2035">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e0305-2035">Az.KeyVault</span></span>
- <span data-ttu-id="e0305-2036">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="e0305-2036">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="e0305-2037">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="e0305-2037">Az.MachineLearning</span></span>
- <span data-ttu-id="e0305-2038">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="e0305-2038">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="e0305-2039">Az.Media</span><span class="sxs-lookup"><span data-stu-id="e0305-2039">Az.Media</span></span>
- <span data-ttu-id="e0305-2040">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="e0305-2040">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="e0305-2041">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-2041">Az.Network</span></span>
<span data-ttu-id="e0305-2042">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="e0305-2042">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="e0305-2043">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="e0305-2043">New cmdlets added:</span></span>
        - <span data-ttu-id="e0305-2044">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2044">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e0305-2045">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2045">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e0305-2046">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2046">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e0305-2047">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2047">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e0305-2048">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2048">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e0305-2049">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="e0305-2049">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="e0305-2050">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2050">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="e0305-2051">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0305-2051">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="e0305-2052">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e0305-2052">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="e0305-2053">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="e0305-2053">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="e0305-2054">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="e0305-2054">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="e0305-2055">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="e0305-2055">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="e0305-2056">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-2056">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="e0305-2057">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-2057">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="e0305-2058">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="e0305-2058">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="e0305-2059">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="e0305-2059">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="e0305-2060">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="e0305-2060">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="e0305-2061">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="e0305-2061">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="e0305-2062">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="e0305-2062">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="e0305-2063">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="e0305-2063">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="e0305-2064">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2064">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="e0305-2065">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-2065">Az.OperationalInsights</span></span>
- <span data-ttu-id="e0305-2066">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2066">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="e0305-2067">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e0305-2067">Az.Profile</span></span>
- <span data-ttu-id="e0305-2068">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e0305-2068">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-2069">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-2069">Az.RecoveryServices</span></span>
- <span data-ttu-id="e0305-2070">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2070">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="e0305-2071">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-2071">Az.Resources</span></span>
- <span data-ttu-id="e0305-2072">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2072">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="e0305-2073">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-2073">Az.ServiceFabric</span></span>
- <span data-ttu-id="e0305-2074">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="e0305-2074">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="e0305-2075">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2075">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="e0305-2076">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="e0305-2076">Az.SIgnalR</span></span>
- <span data-ttu-id="e0305-2077">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="e0305-2077">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="e0305-2078">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-2078">Az.Sql</span></span>
- <span data-ttu-id="e0305-2079">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="e0305-2079">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="e0305-2080">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="e0305-2080">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="e0305-2081">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2081">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="e0305-2082">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-2082">Az.Storage</span></span>
- <span data-ttu-id="e0305-2083">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2083">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="e0305-2084">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-2084">Az.Websites</span></span>
- <span data-ttu-id="e0305-2085">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="e0305-2085">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="e0305-2086">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2086">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="e0305-2087">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-2087">General</span></span>

* <span data-ttu-id="e0305-2088">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="e0305-2088">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="e0305-2089">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-2089">Az.Compute</span></span>

* <span data-ttu-id="e0305-2090">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="e0305-2090">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="e0305-2091">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-2091">Az.DataLakeStore</span></span>

* <span data-ttu-id="e0305-2092">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="e0305-2092">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="e0305-2093">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e0305-2093">Az.FrontDoor</span></span>

* <span data-ttu-id="e0305-2094">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="e0305-2094">Fixed some broken links</span></span>
    - <span data-ttu-id="e0305-2095">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="e0305-2095">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="e0305-2096">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="e0305-2096">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="e0305-2097">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e0305-2097">Az.RecoveryServices</span></span>

* <span data-ttu-id="e0305-2098">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-2098">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="e0305-2099">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="e0305-2099">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="e0305-2100">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-2100">Az.Resources</span></span>

* <span data-ttu-id="e0305-2101">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="e0305-2101">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="e0305-2102">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="e0305-2102">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="e0305-2103">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-2103">Az.Sql</span></span>

* <span data-ttu-id="e0305-2104">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="e0305-2104">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="e0305-2105">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="e0305-2105">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="e0305-2106">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="e0305-2106">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="e0305-2107">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-2107">Az.Storage</span></span>

* <span data-ttu-id="e0305-2108">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e0305-2108">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="e0305-2109">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="e0305-2109">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="e0305-2110">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="e0305-2110">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="e0305-2111">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="e0305-2111">Support Static Website configuration</span></span>
    - <span data-ttu-id="e0305-2112">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="e0305-2112">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="e0305-2113">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="e0305-2113">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="e0305-2114">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-2114">Az.Websites</span></span>

* <span data-ttu-id="e0305-2115">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="e0305-2115">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="e0305-2116">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="e0305-2116">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="e0305-2117">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-2117">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="e0305-2118">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2118">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="e0305-2119">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e0305-2119">Az.ApiManagement</span></span>
* <span data-ttu-id="e0305-2120">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="e0305-2120">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="e0305-2121">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e0305-2121">Az.Automation</span></span>
* <span data-ttu-id="e0305-2122">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="e0305-2122">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="e0305-2123">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="e0305-2123">Added Update Management cmdlets</span></span>
* <span data-ttu-id="e0305-2124">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="e0305-2124">Added Source Control cmdlets</span></span>
* <span data-ttu-id="e0305-2125">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="e0305-2125">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="e0305-2126">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="e0305-2126">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="e0305-2127">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-2127">Az.Compute</span></span>
* <span data-ttu-id="e0305-2128">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="e0305-2128">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="e0305-2129">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="e0305-2129">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="e0305-2130">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-2130">Az.ContainerInstance</span></span>
* <span data-ttu-id="e0305-2131">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="e0305-2131">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="e0305-2132">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="e0305-2132">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="e0305-2133">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="e0305-2133">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="e0305-2134">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-2134">Az.Network</span></span>
* <span data-ttu-id="e0305-2135">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="e0305-2135">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="e0305-2136">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="e0305-2136">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="e0305-2137">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="e0305-2137">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="e0305-2138">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="e0305-2138">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="e0305-2139">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="e0305-2139">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="e0305-2140">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="e0305-2140">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="e0305-2141">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="e0305-2141">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="e0305-2142">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="e0305-2142">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="e0305-2143">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="e0305-2143">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="e0305-2144">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="e0305-2144">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="e0305-2145">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="e0305-2145">Az.Relay</span></span>
* <span data-ttu-id="e0305-2146">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="e0305-2146">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="e0305-2147">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-2147">Az.Resources</span></span>
* <span data-ttu-id="e0305-2148">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="e0305-2148">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="e0305-2149">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="e0305-2149">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="e0305-2150">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="e0305-2150">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="e0305-2151">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-2151">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-2152">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="e0305-2152">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="e0305-2153">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-2153">Az.Sql</span></span>
* <span data-ttu-id="e0305-2154">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-2154">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="e0305-2155">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-2155">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e0305-2156">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-2156">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e0305-2157">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-2157">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e0305-2158">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e0305-2158">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e0305-2159">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e0305-2159">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="e0305-2160">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e0305-2160">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="e0305-2161">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e0305-2161">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="e0305-2162">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e0305-2162">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="e0305-2163">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="e0305-2163">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="e0305-2164">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e0305-2164">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="e0305-2165">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="e0305-2165">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="e0305-2166">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="e0305-2166">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="e0305-2167">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="e0305-2167">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="e0305-2168">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="e0305-2168">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="e0305-2169">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="e0305-2169">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="e0305-2170">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="e0305-2170">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="e0305-2171">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2171">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="e0305-2172">Geral</span><span class="sxs-lookup"><span data-stu-id="e0305-2172">General</span></span>
* <span data-ttu-id="e0305-2173">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="e0305-2173">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="e0305-2174">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e0305-2174">Az.Profile</span></span>
* <span data-ttu-id="e0305-2175">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="e0305-2175">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="e0305-2176">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="e0305-2176">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="e0305-2177">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="e0305-2177">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="e0305-2178">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="e0305-2178">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="e0305-2179">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="e0305-2179">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="e0305-2180">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="e0305-2180">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="e0305-2181">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="e0305-2181">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-2182">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-2182">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-2183">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="e0305-2183">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-2184">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-2184">Az.Compute</span></span>
* <span data-ttu-id="e0305-2185">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="e0305-2185">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="e0305-2186">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="e0305-2186">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="e0305-2187">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="e0305-2187">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-2188">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-2188">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-2189">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="e0305-2189">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="e0305-2190">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="e0305-2190">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="e0305-2191">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="e0305-2191">Az.Insights</span></span>
* <span data-ttu-id="e0305-2192">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="e0305-2192">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="e0305-2193">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="e0305-2193">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="e0305-2194">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="e0305-2194">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="e0305-2195">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="e0305-2195">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-2196">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-2196">Az.Network</span></span>
* <span data-ttu-id="e0305-2197">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="e0305-2197">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="e0305-2198">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="e0305-2198">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="e0305-2199">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="e0305-2199">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="e0305-2200">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="e0305-2200">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="e0305-2201">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="e0305-2201">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="e0305-2202">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="e0305-2202">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="e0305-2203">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="e0305-2203">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e0305-2204">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e0305-2204">Az.PolicyInsights</span></span>
* <span data-ttu-id="e0305-2205">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="e0305-2205">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-2206">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-2206">Az.Resources</span></span>
* <span data-ttu-id="e0305-2207">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="e0305-2207">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="e0305-2208">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="e0305-2208">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e0305-2209">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e0305-2209">Az.ServiceBus</span></span>
* <span data-ttu-id="e0305-2210">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="e0305-2210">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e0305-2211">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e0305-2211">Az.ServiceFabric</span></span>
* <span data-ttu-id="e0305-2212">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="e0305-2212">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="e0305-2213">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="e0305-2213">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="e0305-2214">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="e0305-2214">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="e0305-2215">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="e0305-2215">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="e0305-2216">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="e0305-2216">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="e0305-2217">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2217">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="e0305-2218">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e0305-2218">Az.Profile</span></span>
* <span data-ttu-id="e0305-2219">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="e0305-2219">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="e0305-2220">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="e0305-2220">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-2221">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-2221">Az.Compute</span></span>
* <span data-ttu-id="e0305-2222">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="e0305-2222">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="e0305-2223">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="e0305-2223">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e0305-2224">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e0305-2224">Az.DataLakeStore</span></span>
* <span data-ttu-id="e0305-2225">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="e0305-2225">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="e0305-2226">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-2226">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="e0305-2227">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="e0305-2227">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="e0305-2228">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="e0305-2228">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="e0305-2229">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="e0305-2229">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-2230">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-2230">Az.Network</span></span>
* <span data-ttu-id="e0305-2231">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="e0305-2231">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="e0305-2232">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="e0305-2232">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-2233">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-2233">Az.Resources</span></span>
* <span data-ttu-id="e0305-2234">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="e0305-2234">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="e0305-2235">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="e0305-2235">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="e0305-2236">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2236">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="e0305-2237">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="e0305-2237">Azure.Storage</span></span>
* <span data-ttu-id="e0305-2238">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="e0305-2238">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="e0305-2239">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="e0305-2239">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="e0305-2240">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="e0305-2240">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="e0305-2241">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="e0305-2241">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="e0305-2242">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="e0305-2242">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e0305-2243">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e0305-2243">Az.CognitiveServices</span></span>
* <span data-ttu-id="e0305-2244">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="e0305-2244">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e0305-2245">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e0305-2245">Az.Compute</span></span>
* <span data-ttu-id="e0305-2246">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="e0305-2246">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="e0305-2247">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="e0305-2247">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="e0305-2248">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="e0305-2248">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="e0305-2249">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="e0305-2249">Az.DataFactoryV2</span></span>
* <span data-ttu-id="e0305-2250">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="e0305-2250">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e0305-2251">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e0305-2251">Az.Network</span></span>
* <span data-ttu-id="e0305-2252">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="e0305-2252">Added NetworkProfile functionality.</span></span> <span data-ttu-id="e0305-2253">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="e0305-2253">new cmdlets added</span></span>
    - <span data-ttu-id="e0305-2254">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e0305-2254">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="e0305-2255">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e0305-2255">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="e0305-2256">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e0305-2256">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="e0305-2257">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e0305-2257">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="e0305-2258">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-2258">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="e0305-2259">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-2259">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="e0305-2260">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="e0305-2260">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="e0305-2261">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="e0305-2261">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="e0305-2262">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="e0305-2262">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="e0305-2263">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="e0305-2263">Az.RedisCache</span></span>
* <span data-ttu-id="e0305-2264">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="e0305-2264">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="e0305-2265">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="e0305-2265">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="e0305-2266">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e0305-2266">Az.Resources</span></span>
* <span data-ttu-id="e0305-2267">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="e0305-2267">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="e0305-2268">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="e0305-2268">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="e0305-2269">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e0305-2269">Az.Sql</span></span>
* <span data-ttu-id="e0305-2270">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="e0305-2270">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e0305-2271">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e0305-2271">Az.Websites</span></span>
* <span data-ttu-id="e0305-2272">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="e0305-2272">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="e0305-2273">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="e0305-2273">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="e0305-2274">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e0305-2274">0.2.0 - September 2018</span></span>
 <span data-ttu-id="e0305-2275">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="e0305-2275">Initial Release</span></span>
