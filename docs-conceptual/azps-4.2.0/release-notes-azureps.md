---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: a9ec7589ab155553da29612096a607d82a078321
ms.sourcegitcommit: 5523170e571fbd1dc93bd0fa4223aba3b324d3b0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/25/2020
ms.locfileid: "85363703"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="8d30d-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="8d30d-103">Azure PowerShell release notes</span></span>

## <a name="430---june-2020"></a><span data-ttu-id="8d30d-104">4.3.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-104">4.3.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-105">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-106">Suporte para a deteção da definição do ambiente por predefinição e adição de ambiente através de "Add-AzEnvironment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-106">Supported discovering environment setting by default and adding environment via 'Add-AzEnvironment'</span></span>
* <span data-ttu-id="8d30d-107">Atualizar assemblagens pré-carregadas [#12024], [#11976]</span><span class="sxs-lookup"><span data-stu-id="8d30d-107">Update preloaded assemblies [#12024], [#11976]</span></span>
* <span data-ttu-id="8d30d-108">Atualização da assemblagem Azure.Core</span><span class="sxs-lookup"><span data-stu-id="8d30d-108">Updated Azure.Core assembly</span></span>
* <span data-ttu-id="8d30d-109">Correção de um problema que pode provocar a falha de "Connect-AzAccount" numa execução de múltiplos threads [#11201]</span><span class="sxs-lookup"><span data-stu-id="8d30d-109">Fixed an issue that may cause 'Connect-AzAccount' to fail in multi-threaded execution [#11201]</span></span>

#### <a name="azaks"></a><span data-ttu-id="8d30d-110">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8d30d-110">Az.Aks</span></span>
* <span data-ttu-id="8d30d-111">Substituição da utilização da [API AccessProfile](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) antiga por chamadas para as APIs [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) e [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials)</span><span class="sxs-lookup"><span data-stu-id="8d30d-111">Replaced usage of old [AccessProfile API](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) with calls to [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) and [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials) APIs</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-112">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-112">Az.Batch</span></span>
* <span data-ttu-id="8d30d-113">Atualização da versão do SDK de Az.Batch para utilizar "Microsoft.Azure.Management.Batch" para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-113">Updated Az.Batch to use 'Microsoft.Azure.Management.Batch' SDK version to 11.0.0</span></span>
* <span data-ttu-id="8d30d-114">Adição da capacidade de definir a Identidade BatchAccount no cmdlet "New-AzBatchAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-114">Added the ability to set the BatchAccount Identity in the 'New-AzBatchAccount' cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-115">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-115">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-116">Suporte para a apresentação das capacidades da conta.</span><span class="sxs-lookup"><span data-stu-id="8d30d-116">Supported displaying account capabilities.</span></span>
* <span data-ttu-id="8d30d-117">Suporte para a modificação de PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="8d30d-117">Supported modifying PublicNetworkAccess.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-118">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-118">Az.Compute</span></span>
* <span data-ttu-id="8d30d-119">Adição do parâmetro SimulateEviction aos cmdlets Set-AzVM e Set-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="8d30d-119">Added SimulateEviction parameter to Set-AzVM and Set-AzVmssVM cmdlets.</span></span>
* <span data-ttu-id="8d30d-120">Adição de "Premium_LRS" ao mecanismo de preenchimento de argumentos do parâmetro StorageAccountType para o cmdlet New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="8d30d-120">Added 'Premium_LRS' to the argument completer of StorageAccountType parameter for New-AzGalleryImageVersion cmdlet.</span></span>
* <span data-ttu-id="8d30d-121">Adição de subestados a VMCustomScriptExtension [#11297]</span><span class="sxs-lookup"><span data-stu-id="8d30d-121">Added Substatuses to VMCustomScriptExtension [#11297]</span></span>
* <span data-ttu-id="8d30d-122">Adição de "Delete" ao mecanismo de preenchimento de argumentos do parâmetro EvictionPolicy para os cmdlets New-AzVM e New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="8d30d-122">Added 'Delete' to the argument completer of EvictionPolicy parameter for New-AzVM and New-AzVMConfig cmdlets.</span></span>
* <span data-ttu-id="8d30d-123">Correção do nome da nova Extensão de VM para SAP</span><span class="sxs-lookup"><span data-stu-id="8d30d-123">Fixed name of new VM Extension for SAP</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-124">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-125">Atualização da versão do SDK de .Net do ADF para 4.9.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-125">Updated ADF .Net SDK version to 4.9.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-126">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-126">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-127">Adição de parâmetros de Identidade Gerida aos cmdlets "New-AzEventHubNamespace" e "Set-AzEventHubNamespace"</span><span class="sxs-lookup"><span data-stu-id="8d30d-127">Added Managed Identity parameters to 'New-AzEventHubNamespace' and 'Set-AzEventHubNamespace' cmdlets</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="8d30d-128">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="8d30d-128">Az.Functions</span></span>
* <span data-ttu-id="8d30d-129">Adição de suporte para a criação de aplicações de funções do PowerShell 7.0 e de Java 11</span><span class="sxs-lookup"><span data-stu-id="8d30d-129">Added support to create PowerShell 7.0 and Java 11 function apps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-130">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-130">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-131">Suporte para listagem de anfitriões e reinício de anfitriões específicos do cluster HDInsight.</span><span class="sxs-lookup"><span data-stu-id="8d30d-131">Supported listing hosts and restart specific hosts of the HDInsight cluster.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8d30d-132">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8d30d-132">Az.HealthcareApis</span></span>
* <span data-ttu-id="8d30d-133">Atualização da versão do SDK para 1.1.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-133">Updated the SDK version to 1.1.0</span></span>
* <span data-ttu-id="8d30d-134">Adição de suporte para as definições de Exportação e a Identidade Gerida</span><span class="sxs-lookup"><span data-stu-id="8d30d-134">Added support for Export settings and Managed Identity</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-135">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-136">Correção do parâmetro de objeto de entrada para "Set-AzActivityLogAlert"</span><span class="sxs-lookup"><span data-stu-id="8d30d-136">Fixed input object parameter for 'Set-AzActivityLogAlert'</span></span>
* <span data-ttu-id="8d30d-137">Correção do parâmetro "InputObject" para "Set-AzActionGroup" [#10868]</span><span class="sxs-lookup"><span data-stu-id="8d30d-137">Fixed 'InputObject' parameter for 'Set-AzActionGroup' [#10868]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-138">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-138">Az.Network</span></span>
* <span data-ttu-id="8d30d-139">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="8d30d-139">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="8d30d-140">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-140">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="8d30d-141">"New-AzFirewallPolicyDnsSetting"</span><span class="sxs-lookup"><span data-stu-id="8d30d-141">'New-AzFirewallPolicyDnsSetting'</span></span>
    - <span data-ttu-id="8d30d-142">Suporte para FQDN de Destino nas Regras de Rede para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-142">Support for Destination FQDN in Network Rules for Firewall Policy</span></span>
* <span data-ttu-id="8d30d-143">Adição de suporte para operações de conjuntos de endereços back-end</span><span class="sxs-lookup"><span data-stu-id="8d30d-143">Added support for backend address pool operations</span></span>
    - <span data-ttu-id="8d30d-144">"New-AzLoadBalancerBackendAddressConfig"</span><span class="sxs-lookup"><span data-stu-id="8d30d-144">'New-AzLoadBalancerBackendAddressConfig'</span></span>
    - <span data-ttu-id="8d30d-145">"New-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="8d30d-145">'New-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="8d30d-146">"Set-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="8d30d-146">'Set-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="8d30d-147">"Remove-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="8d30d-147">'Remove-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="8d30d-148">"Get-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="8d30d-148">'Get-AzLoadBalancerBackendAddressPool'</span></span>
* <span data-ttu-id="8d30d-149">Adição de validação de nomes para "New-AzIpGroup"</span><span class="sxs-lookup"><span data-stu-id="8d30d-149">Added name validation for 'New-AzIpGroup'</span></span>
* <span data-ttu-id="8d30d-150">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-150">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="8d30d-151">"New-AzFirewallPolicyThreatIntelWhitelist"</span><span class="sxs-lookup"><span data-stu-id="8d30d-151">'New-AzFirewallPolicyThreatIntelWhitelist'</span></span>
* <span data-ttu-id="8d30d-152">Foram atualizados os seguintes comandos para a funcionalidade: Definição/remoção de servidores DNS personalizados no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="8d30d-152">Updated below commands for feature: Custom dns servers set/remove on VirtualWan P2SVpnGateway.</span></span>
    - <span data-ttu-id="8d30d-153">Atualização de New-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="8d30d-153">Updated New-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
    - <span data-ttu-id="8d30d-154">Atualização de Update-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="8d30d-154">Updated Update-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
* <span data-ttu-id="8d30d-155">Atualização de "Update-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-155">Updated 'Update-AzVpnGateway'</span></span>
    - <span data-ttu-id="8d30d-156">Adição do parâmetro opcional "-BgpPeeringAddress" para os clientes especificarem os respetivos bgps personalizados a definir no VpnGateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-156">Added optional parameter '-BgpPeeringAddress' for customers to specify their custom bgps to set on VpnGateway.</span></span>
* <span data-ttu-id="8d30d-157">Adição de novo cmdlet para suportar a reposição do estado de encaminhamento de um recurso VirtualHub:</span><span class="sxs-lookup"><span data-stu-id="8d30d-157">Added new cmdlet to support resetting the routing state of a VirtualHub resource:</span></span>
    - <span data-ttu-id="8d30d-158">"Reset-AzHubRouter"</span><span class="sxs-lookup"><span data-stu-id="8d30d-158">'Reset-AzHubRouter'</span></span>
* <span data-ttu-id="8d30d-159">Atualização dos elementos indicados abaixo com base na alteração recente de Swagger para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-159">Updated below things based on recent swagger change for Firewall Policy</span></span>
    - <span data-ttu-id="8d30d-160">Alteração de nomes para RuleGroup, RuleCollectionGroup e RuleType</span><span class="sxs-lookup"><span data-stu-id="8d30d-160">Changes names for RuleGroup, RuleCollectionGroup and RuleType</span></span>
    - <span data-ttu-id="8d30d-161">Adição de suporte para Coleções de Regras de NAT da Política de Firewall para suportar várias Coleções de Regras de NAT</span><span class="sxs-lookup"><span data-stu-id="8d30d-161">Added support for Firewall Policy NAT Rule Collections to support multiple NAT Rule Collection</span></span>
* <span data-ttu-id="8d30d-162">[Alteração Interruptiva] Adição do parâmetro obrigatório "SourceIpGroup" para "New-AzFirewallPolicyApplicationRule" e "New-AzFirewallPolicyNetworkRule".</span><span class="sxs-lookup"><span data-stu-id="8d30d-162">[Breaking Change] Added mandatory parameter 'SourceIpGroup' for 'New-AzFirewallPolicyApplicationRule' and 'New-AzFirewallPolicyNetworkRule'.</span></span>
* <span data-ttu-id="8d30d-163">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d30d-163">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="8d30d-164">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d30d-164">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="8d30d-165">[Alteração Interruptiva] Remoção de parâmetros obrigatórios: "TranslatedAddress", "TranslatedPort" para "New-AzFirewallPolicyNatRuleCollection".</span><span class="sxs-lookup"><span data-stu-id="8d30d-165">[Breaking Change] Removed mandatory parameters: 'TranslatedAddress', 'TranslatedPort' for 'New-AzFirewallPolicyNatRuleCollection'.</span></span>
* <span data-ttu-id="8d30d-166">Adição de novos cmdlets para suportar PrivateLink no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-166">Added new cmdlets to support PrivateLink On Application Gateway</span></span>
    - <span data-ttu-id="8d30d-167">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-167">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="8d30d-168">"Get-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-168">'Get-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="8d30d-169">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-169">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="8d30d-170">"Set-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-170">'Set-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="8d30d-171">"Remove-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-171">'Remove-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="8d30d-172">"New-AzApplicationGatewayPrivateLinkIpConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-172">'New-AzApplicationGatewayPrivateLinkIpConfiguration'</span></span>
* <span data-ttu-id="8d30d-173">Adição de novos cmdlets para o recurso subordinado HubRouteTables de VirtualHub.</span><span class="sxs-lookup"><span data-stu-id="8d30d-173">Added new cmdlets for HubRouteTables child resource of VirtualHub.</span></span>
    - <span data-ttu-id="8d30d-174">"New-AzVHubRoute"</span><span class="sxs-lookup"><span data-stu-id="8d30d-174">'New-AzVHubRoute'</span></span>
    - <span data-ttu-id="8d30d-175">"New-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="8d30d-175">'New-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="8d30d-176">"Get-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="8d30d-176">'Get-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="8d30d-177">"Update-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="8d30d-177">'Update-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="8d30d-178">"Remove-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="8d30d-178">'Remove-AzVHubRouteTable'</span></span>
* <span data-ttu-id="8d30d-179">Atualização dos cmdlets existentes para suportar o parâmetro de entrada opcional RoutingConfiguration para encaminhamento personalizado em VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="8d30d-179">Updated existing cmdlets to support optional RoutingConfiguration input parameter for custom routing in VirtualWan.</span></span>
    - <span data-ttu-id="8d30d-180">"New-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-180">'New-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="8d30d-181">"Set-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-181">'Set-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="8d30d-182">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-182">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="8d30d-183">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-183">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="8d30d-184">"New-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-184">'New-AzVpnConnection'</span></span>
    - <span data-ttu-id="8d30d-185">"Update-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-185">'Update-AzVpnConnection'</span></span>
    - <span data-ttu-id="8d30d-186">"New-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-186">'New-AzP2sVpnGateway'</span></span>
    - <span data-ttu-id="8d30d-187">"Update-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-187">'Update-AzP2sVpnGateway'</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-188">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-188">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-189">Correção do erro PSWorkspace não implementa IOperationalInsightsWorkspace [#12135]</span><span class="sxs-lookup"><span data-stu-id="8d30d-189">Fixed bug PSWorkspace doesn't implement IOperationalInsightsWorkspace [#12135]</span></span>
* <span data-ttu-id="8d30d-190">Adição de "pergb2018" ao conjunto de valores válidos do parâmetro "Sku" em "Set-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="8d30d-190">Added 'pergb2018' to valid value set of parameter 'Sku' in 'Set-AzOperationalInsightsWorkspace'</span></span> 
* <span data-ttu-id="8d30d-191">Adição do alias "FunctionParameters" para o parâmetro "FunctionParameter" a</span><span class="sxs-lookup"><span data-stu-id="8d30d-191">Added alias 'FunctionParameters' for parameter 'FunctionParameter' to</span></span>
    - <span data-ttu-id="8d30d-192">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="8d30d-192">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="8d30d-193">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="8d30d-193">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-194">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-194">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-195">Adição de suporte no Azure Backup para a obtenção de itens de MAB.</span><span class="sxs-lookup"><span data-stu-id="8d30d-195">Azure Backup added support for fetching MAB items.</span></span>
* <span data-ttu-id="8d30d-196">Suporte do Azure Site Recovery para o tipo de disco "StandardSSD_LRS"</span><span class="sxs-lookup"><span data-stu-id="8d30d-196">Azure Site Recovery supports disk type 'StandardSSD_LRS'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-197">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-197">Az.Resources</span></span>
* <span data-ttu-id="8d30d-198">Adição de "UsageLocation", "GivenName", "Surname", "AccountEnabled", "MailNickname", "Mail" em "PSADUser" [#10526] [#10497]</span><span class="sxs-lookup"><span data-stu-id="8d30d-198">Added 'UsageLocation', 'GivenName', 'Surname', 'AccountEnabled', 'MailNickname', 'Mail' on 'PSADUser' [#10526] [#10497]</span></span>
* <span data-ttu-id="8d30d-199">Correção do problema em que "-Mail" não funciona em "Get-AzADUser" [#11981]</span><span class="sxs-lookup"><span data-stu-id="8d30d-199">Fixed issue that '-Mail' doesn't work on 'Get-AzADUser' [#11981]</span></span>
* <span data-ttu-id="8d30d-200">Adição do parâmetro "-ExcludeChangeType" a "Get-AzDeploymentWhatIfResult" e "Get-AzResourceGroupDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="8d30d-200">Added '-ExcludeChangeType' parameter to 'Get-AzDeploymentWhatIfResult' and 'Get-AzResourceGroupDeploymentWhatIfResult'</span></span>
* <span data-ttu-id="8d30d-201">Adição do parâmetro "-WhatIfExcludeChangeType" a "New-AzDeployment" e "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-201">Added '-WhatIfExcludeChangeType' parameter to 'New-AzDeployment' and 'New-AzResourceGroupDeployment'</span></span>
* <span data-ttu-id="8d30d-202">Atualização de cmdlets "Test-Az\*Deployment" para apresentação de mensagens de erro melhores</span><span class="sxs-lookup"><span data-stu-id="8d30d-202">Updated 'Test-Az\*Deployment' cmdlets to show better error messages</span></span>
* <span data-ttu-id="8d30d-203">Correção da mensagem de ajuda para o parâmetro "-Name" de criação de implementação e cmdlets What-If</span><span class="sxs-lookup"><span data-stu-id="8d30d-203">Fixed help message for '-Name' parameter of deployment create and What-If cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-204">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-204">Az.Sql</span></span>
* <span data-ttu-id="8d30d-205">Adição de suporte para o principal de serviço para o cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="8d30d-205">Added support for service principal for Set SQL Server Azure Active Directory Admin cmdlet</span></span>
* <span data-ttu-id="8d30d-206">Correção de problema de sincronização em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-206">Fixed sync issue in Data Classification cmdlets.</span></span>
* <span data-ttu-id="8d30d-207">Suporte para a pesquisa de utilizador por correio em "Set-AzSqlServerActiveDirectoryAdministrator" [#12192]</span><span class="sxs-lookup"><span data-stu-id="8d30d-207">Supported searching user by mail on 'Set-AzSqlServerActiveDirectoryAdministrator' [#12192]</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-208">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-208">Az.Storage</span></span>
* <span data-ttu-id="8d30d-209">Suporte para a criação de Conta de armazenamento com RequireInfrastructureEncryption</span><span class="sxs-lookup"><span data-stu-id="8d30d-209">Supported create Storage account with RequireInfrastructureEncryption</span></span>
    -  <span data-ttu-id="8d30d-210">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-210">'New-AzStorageAccount'</span></span>
* <span data-ttu-id="8d30d-211">Mudança da lógica de carregamento de Azure.Core para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-211">Moved the logic of loading Azure.Core to Az.Accounts</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-212">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-212">Az.Websites</span></span>
* <span data-ttu-id="8d30d-213">Adição de salvaguarda para eliminar a aplicação Web criada em caso de falha do restauro em "Restore-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="8d30d-213">Added safeguard to delete created webapp if restore failed in 'Restore-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8d30d-214">Adição de "SourceWebApp.Location" para "New-AzWebApp" e "New-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="8d30d-214">Added 'SourceWebApp.Location' for 'New-AzWebApp' and 'New-AzWebAppSlot'</span></span>
* <span data-ttu-id="8d30d-215">Correção do erro que impedia a alteração de definições de Contentor em "Set-AzWebApp" e "Set-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="8d30d-215">Fixed bug that prevented changing Container settings in 'Set-AzWebApp' and 'Set-AzWebAppSlot'</span></span>
* <span data-ttu-id="8d30d-216">Correção do erro para obter SiteConfig quando -Name não é fornecido para Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-216">Fixed bug to get SiteConfig when -Name is not given for Get-AzWebApp</span></span>
* <span data-ttu-id="8d30d-217">Adição de suporte para a criação de ASP para Aplicações Linux</span><span class="sxs-lookup"><span data-stu-id="8d30d-217">Added a support to create ASP for Linux Apps</span></span>
* <span data-ttu-id="8d30d-218">Adição de exceções para clonagem entre grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="8d30d-218">Added exceptions for clone across resource groups</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="8d30d-219">4.2.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-219">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-220">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-220">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-221">Correção de um problema que fazia com que o Az ignorasse registos nas tarefas da Automatização do Azure ou do PowerShell [#11492]</span><span class="sxs-lookup"><span data-stu-id="8d30d-221">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d30d-222">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-222">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d30d-223">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="8d30d-223">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-224">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-224">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-225">Atualização da versão de assemblagem dos cmdlets de gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="8d30d-225">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="8d30d-226">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8d30d-226">Az.Billing</span></span>
* <span data-ttu-id="8d30d-227">Atualização da versão de assemblagem dos cmdlets de consumo</span><span class="sxs-lookup"><span data-stu-id="8d30d-227">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-228">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-228">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-229">Suporte para o controlo de PrivateEndpoint e PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="8d30d-229">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-230">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-230">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-231">Atualização da versão de assemblagem dos cmdlets V2 de fábrica de dados</span><span class="sxs-lookup"><span data-stu-id="8d30d-231">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="8d30d-232">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-232">Az.DataShare</span></span>
* <span data-ttu-id="8d30d-233">Disponibilidade geral do módulo "Az.DataShare"</span><span class="sxs-lookup"><span data-stu-id="8d30d-233">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="8d30d-234">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="8d30d-234">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="8d30d-235">Disponibilidade geral do módulo "Az.DesktopVirtualization"</span><span class="sxs-lookup"><span data-stu-id="8d30d-235">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-236">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-236">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-237">Atualização do SDK para a versão 0.21.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-237">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="8d30d-238">Adição de parâmetros opcionais a</span><span class="sxs-lookup"><span data-stu-id="8d30d-238">Added optional parameters to</span></span> 
    - <span data-ttu-id="8d30d-239">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="8d30d-239">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="8d30d-240">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="8d30d-240">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-241">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-241">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-242">Correção do exemplo 3 de "Start-AzPolicyComplianceScan"</span><span class="sxs-lookup"><span data-stu-id="8d30d-242">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8d30d-243">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8d30d-243">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8d30d-244">Atualização da versão de assemblagem dos cmdlets do PowerBI</span><span class="sxs-lookup"><span data-stu-id="8d30d-244">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="8d30d-245">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="8d30d-245">Az.PrivateDns</span></span>
* <span data-ttu-id="8d30d-246">Correção da formatação da cadeia de saída verbosa de Remove-AzPrivateDnsRecordSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-246">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-247">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-248">Suporte do Azure Site Recovery para a criação de um plano de recuperação para replicação zona a zona a partir de uma entrada xml.</span><span class="sxs-lookup"><span data-stu-id="8d30d-248">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="8d30d-249">Atualização da versão de assemblagem dos cmdlets do SiteRecovery e Backup</span><span class="sxs-lookup"><span data-stu-id="8d30d-249">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-250">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-250">Az.Resources</span></span>
* <span data-ttu-id="8d30d-251">Adição do parâmetro Tail aos cmdlets Get-AzDeploymentScriptLog e Save-AzDeploymentScriptLog</span><span class="sxs-lookup"><span data-stu-id="8d30d-251">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="8d30d-252">Formatação da propriedade Output e apresentação da mesma na saída do cmdlet Get-AzDeploymentScript</span><span class="sxs-lookup"><span data-stu-id="8d30d-252">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="8d30d-253">Mudança de nome do parâmetro -DeploymentScriptInputObject para -DeploymentScriptObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-253">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="8d30d-254">Correção do nome em falta do ficheiro/destino nas mensagens de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="8d30d-254">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="8d30d-255">Atualização da versão de assemblagem dos cmdlets de gestor de recursos e de etiquetas</span><span class="sxs-lookup"><span data-stu-id="8d30d-255">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-256">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-256">Az.Sql</span></span>
* <span data-ttu-id="8d30d-257">Adição de UsePrivateLinkConnection a "New-AzSqlSyncGroup", "Update-AzSqlSyncGroup", "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="8d30d-257">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="8d30d-258">Adição de SyncMemberAzureDatabaseResourceId a "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="8d30d-258">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="8d30d-259">Adição do suporte de pesquisa de Utilizador convidado ao cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="8d30d-259">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-260">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-260">Az.Storage</span></span>
* <span data-ttu-id="8d30d-261">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="8d30d-261">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="8d30d-262">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-262">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="8d30d-263">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="8d30d-263">Highlights since the last release</span></span>
* <span data-ttu-id="8d30d-264">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="8d30d-264">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="8d30d-265">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="8d30d-265">General availability of Az.Functions</span></span> 
* <span data-ttu-id="8d30d-266">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="8d30d-266">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-267">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-267">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-268">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="8d30d-268">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="8d30d-269">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="8d30d-269">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="8d30d-270">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8d30d-270">Az.Aks</span></span>
* <span data-ttu-id="8d30d-271">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="8d30d-271">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="8d30d-272">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="8d30d-272">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="8d30d-273">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="8d30d-273">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-274">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-274">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-275">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="8d30d-275">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="8d30d-276">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="8d30d-276">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="8d30d-277">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="8d30d-277">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="8d30d-278">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="8d30d-278">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="8d30d-279">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="8d30d-279">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="8d30d-280">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="8d30d-280">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="8d30d-281">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="8d30d-281">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="8d30d-282">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="8d30d-282">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="8d30d-283">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="8d30d-283">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="8d30d-284">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="8d30d-284">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="8d30d-285">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="8d30d-285">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="8d30d-286">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="8d30d-286">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="8d30d-287">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="8d30d-287">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="8d30d-288">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="8d30d-288">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="8d30d-289">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="8d30d-289">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="8d30d-290">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="8d30d-290">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="8d30d-291">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-291">Az.ApplicationInsights</span></span>
* <span data-ttu-id="8d30d-292">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="8d30d-292">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="8d30d-293">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="8d30d-293">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="8d30d-294">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="8d30d-294">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-295">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-295">Az.Batch</span></span>
* <span data-ttu-id="8d30d-296">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="8d30d-296">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="8d30d-297">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="8d30d-297">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="8d30d-298">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="8d30d-298">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="8d30d-299">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="8d30d-299">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="8d30d-300">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="8d30d-300">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="8d30d-301">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="8d30d-301">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="8d30d-302">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="8d30d-302">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="8d30d-303">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="8d30d-303">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="8d30d-304">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="8d30d-304">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-305">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-305">Az.Compute</span></span>
* <span data-ttu-id="8d30d-306">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="8d30d-306">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="8d30d-307">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-307">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="8d30d-308">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8d30d-308">Breaking changes</span></span>
    - <span data-ttu-id="8d30d-309">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="8d30d-309">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="8d30d-310">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="8d30d-310">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="8d30d-311">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="8d30d-311">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="8d30d-312">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="8d30d-312">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="8d30d-313">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="8d30d-313">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="8d30d-314">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="8d30d-314">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="8d30d-315">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="8d30d-315">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-316">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-316">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-317">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="8d30d-317">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-318">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-318">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-319">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="8d30d-319">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="8d30d-320">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="8d30d-320">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="8d30d-321">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="8d30d-321">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="8d30d-322">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="8d30d-322">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="8d30d-323">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="8d30d-323">Az.Functions</span></span>
* <span data-ttu-id="8d30d-324">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="8d30d-324">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-325">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-325">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-326">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="8d30d-326">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8d30d-327">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8d30d-327">Az.HealthcareApis</span></span>
* <span data-ttu-id="8d30d-328">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="8d30d-328">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-329">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-329">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-330">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="8d30d-330">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="8d30d-331">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="8d30d-331">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="8d30d-332">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="8d30d-332">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="8d30d-333">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="8d30d-333">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="8d30d-334">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="8d30d-334">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="8d30d-335">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-335">New cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-336">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-336">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="8d30d-337">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-337">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="8d30d-338">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-338">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="8d30d-339">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-339">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="8d30d-340">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="8d30d-340">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="8d30d-341">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-341">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-342">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-342">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-343">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="8d30d-343">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="8d30d-344">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="8d30d-344">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="8d30d-345">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="8d30d-345">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="8d30d-346">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="8d30d-346">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="8d30d-347">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="8d30d-347">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="8d30d-348">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="8d30d-348">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="8d30d-349">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="8d30d-349">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-350">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-350">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-351">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="8d30d-351">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="8d30d-352">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="8d30d-352">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="8d30d-353">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="8d30d-353">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="8d30d-354">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="8d30d-354">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="8d30d-355">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="8d30d-355">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="8d30d-356">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="8d30d-356">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="8d30d-357">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="8d30d-357">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-358">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-358">Az.Network</span></span>
* <span data-ttu-id="8d30d-359">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="8d30d-359">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="8d30d-360">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="8d30d-360">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="8d30d-361">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="8d30d-361">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="8d30d-362">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="8d30d-362">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="8d30d-363">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="8d30d-363">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="8d30d-364">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-364">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-365">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="8d30d-365">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="8d30d-366">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="8d30d-366">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="8d30d-367">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="8d30d-367">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="8d30d-368">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="8d30d-368">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="8d30d-369">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="8d30d-369">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="8d30d-370">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-370">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="8d30d-371">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8d30d-371">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="8d30d-372">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="8d30d-372">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="8d30d-373">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="8d30d-373">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="8d30d-374">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="8d30d-374">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="8d30d-375">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="8d30d-375">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="8d30d-376">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="8d30d-376">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="8d30d-377">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="8d30d-377">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="8d30d-378">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="8d30d-378">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="8d30d-379">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="8d30d-379">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="8d30d-380">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="8d30d-380">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="8d30d-381">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="8d30d-381">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="8d30d-382">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-382">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d30d-383">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-383">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-384">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-384">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-385">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="8d30d-385">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="8d30d-386">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="8d30d-386">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="8d30d-387">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="8d30d-387">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="8d30d-388">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="8d30d-388">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="8d30d-389">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="8d30d-389">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="8d30d-390">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="8d30d-390">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="8d30d-391">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="8d30d-391">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="8d30d-392">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="8d30d-392">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-393">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-393">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-394">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-394">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="8d30d-395">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="8d30d-395">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="8d30d-396">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-396">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="8d30d-397">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="8d30d-397">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="8d30d-398">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="8d30d-398">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-399">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-399">Az.Resources</span></span>
* <span data-ttu-id="8d30d-400">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="8d30d-400">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="8d30d-401">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="8d30d-401">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="8d30d-402">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="8d30d-402">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="8d30d-403">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="8d30d-403">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="8d30d-404">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="8d30d-404">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="8d30d-405">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="8d30d-405">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="8d30d-406">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="8d30d-406">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="8d30d-407">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="8d30d-407">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="8d30d-408">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="8d30d-408">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="8d30d-409">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="8d30d-409">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="8d30d-410">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="8d30d-410">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="8d30d-411">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="8d30d-411">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="8d30d-412">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="8d30d-412">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="8d30d-413">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="8d30d-413">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="8d30d-414">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="8d30d-414">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="8d30d-415">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="8d30d-415">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="8d30d-416">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-416">'New-AzDeployment'</span></span>
    - <span data-ttu-id="8d30d-417">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-417">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="8d30d-418">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-418">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8d30d-419">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-419">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-420">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-420">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-421">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="8d30d-421">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-422">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-422">Az.Sql</span></span>
* <span data-ttu-id="8d30d-423">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="8d30d-423">Enhance performance of:</span></span>
    - <span data-ttu-id="8d30d-424">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="8d30d-424">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="8d30d-425">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="8d30d-425">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="8d30d-426">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="8d30d-426">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="8d30d-427">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="8d30d-427">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="8d30d-428">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="8d30d-428">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="8d30d-429">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="8d30d-429">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="8d30d-430">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="8d30d-430">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="8d30d-431">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="8d30d-431">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="8d30d-432">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="8d30d-432">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="8d30d-433">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="8d30d-433">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-434">Az.Storage</span></span>
* <span data-ttu-id="8d30d-435">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-435">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="8d30d-436">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="8d30d-436">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="8d30d-437">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-437">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="8d30d-438">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="8d30d-438">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="8d30d-439">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="8d30d-439">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="8d30d-440">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="8d30d-440">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="8d30d-441">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-441">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="8d30d-442">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-442">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="8d30d-443">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="8d30d-443">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="8d30d-444">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="8d30d-444">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="8d30d-445">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="8d30d-445">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="8d30d-446">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="8d30d-446">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="8d30d-447">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="8d30d-447">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="8d30d-448">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-448">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="8d30d-449">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-449">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="8d30d-450">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-450">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="8d30d-451">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-451">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="8d30d-452">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="8d30d-452">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="8d30d-453">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="8d30d-453">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="8d30d-454">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="8d30d-454">Supported failover Storage account</span></span>
    - <span data-ttu-id="8d30d-455">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="8d30d-455">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="8d30d-456">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="8d30d-456">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="8d30d-457">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="8d30d-457">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="8d30d-458">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="8d30d-458">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="8d30d-459">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="8d30d-459">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="8d30d-460">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="8d30d-460">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="8d30d-461">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="8d30d-461">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="8d30d-462">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="8d30d-462">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="8d30d-463">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="8d30d-463">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="8d30d-464">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="8d30d-464">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="8d30d-465">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="8d30d-465">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="8d30d-466">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="8d30d-466">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="8d30d-467">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="8d30d-467">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="8d30d-468">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="8d30d-468">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="8d30d-469">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="8d30d-469">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="8d30d-470">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="8d30d-470">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="8d30d-471">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="8d30d-471">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="8d30d-472">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="8d30d-472">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="8d30d-473">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="8d30d-473">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8d30d-474">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8d30d-474">Az.TrafficManager</span></span>
* <span data-ttu-id="8d30d-475">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="8d30d-475">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-476">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-476">Az.Websites</span></span>
* <span data-ttu-id="8d30d-477">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="8d30d-477">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="8d30d-478">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-478">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="8d30d-479">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="8d30d-479">Highlights since the last release</span></span>
* <span data-ttu-id="8d30d-480">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="8d30d-480">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-481">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-481">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-482">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="8d30d-482">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-483">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-483">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-484">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="8d30d-484">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="8d30d-485">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="8d30d-485">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-486">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-486">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-487">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="8d30d-487">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-488">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-488">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-489">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="8d30d-489">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-490">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-490">Az.Compute</span></span>
* <span data-ttu-id="8d30d-491">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="8d30d-491">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="8d30d-492">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="8d30d-492">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-493">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-493">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-494">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-494">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-495">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="8d30d-495">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="8d30d-496">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="8d30d-496">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="8d30d-497">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-497">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="8d30d-498">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-498">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-499">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="8d30d-499">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="8d30d-500">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="8d30d-500">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="8d30d-501">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="8d30d-501">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="8d30d-502">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-502">New cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-503">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-503">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="8d30d-504">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-504">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="8d30d-505">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-505">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="8d30d-506">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-506">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="8d30d-507">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-507">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-508">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-508">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-509">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="8d30d-509">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="8d30d-510">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="8d30d-510">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="8d30d-511">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="8d30d-511">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="8d30d-512">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="8d30d-512">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="8d30d-513">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="8d30d-513">Az.Maintenance</span></span>
* <span data-ttu-id="8d30d-514">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-514">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-515">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-515">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-516">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="8d30d-516">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="8d30d-517">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="8d30d-517">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="8d30d-518">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="8d30d-518">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="8d30d-519">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="8d30d-519">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="8d30d-520">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="8d30d-520">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="8d30d-521">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="8d30d-521">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="8d30d-522">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="8d30d-522">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="8d30d-523">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="8d30d-523">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-524">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-524">Az.Network</span></span>
* <span data-ttu-id="8d30d-525">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="8d30d-525">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="8d30d-526">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-526">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="8d30d-527">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-527">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="8d30d-528">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-528">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="8d30d-529">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-529">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="8d30d-530">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="8d30d-530">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="8d30d-531">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-531">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="8d30d-532">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="8d30d-532">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="8d30d-533">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="8d30d-533">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="8d30d-534">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="8d30d-534">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="8d30d-535">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="8d30d-535">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="8d30d-536">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="8d30d-536">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="8d30d-537">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="8d30d-537">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="8d30d-538">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="8d30d-538">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="8d30d-539">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-539">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="8d30d-540">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-540">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-541">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-541">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-542">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="8d30d-542">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="8d30d-543">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="8d30d-543">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-544">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-544">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-545">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="8d30d-545">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-546">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-546">Az.Sql</span></span>
* <span data-ttu-id="8d30d-547">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="8d30d-547">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="8d30d-548">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="8d30d-548">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-549">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-549">Az.Storage</span></span>
* <span data-ttu-id="8d30d-550">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="8d30d-550">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="8d30d-551">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-551">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="8d30d-552">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-552">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="8d30d-553">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-553">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="8d30d-554">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="8d30d-554">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="8d30d-555">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="8d30d-555">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="8d30d-556">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="8d30d-556">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="8d30d-557">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="8d30d-557">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="8d30d-558">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="8d30d-558">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="8d30d-559">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="8d30d-559">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="8d30d-560">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="8d30d-560">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="8d30d-561">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="8d30d-561">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="8d30d-562">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="8d30d-562">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="8d30d-563">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-563">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="8d30d-564">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-564">General</span></span>
* <span data-ttu-id="8d30d-565">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="8d30d-565">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="8d30d-566">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="8d30d-566">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="8d30d-567">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="8d30d-567">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="8d30d-568">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="8d30d-568">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="8d30d-569">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8d30d-569">Az.Billing</span></span>
  - <span data-ttu-id="8d30d-570">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-570">Az.Compute</span></span>
  - <span data-ttu-id="8d30d-571">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8d30d-571">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="8d30d-572">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-572">Az.EventHub</span></span>
  - <span data-ttu-id="8d30d-573">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-573">Az.IotHub</span></span>
  - <span data-ttu-id="8d30d-574">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-574">Az.KeyVault</span></span>
  - <span data-ttu-id="8d30d-575">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-575">Az.Monitor</span></span>
  - <span data-ttu-id="8d30d-576">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-576">Az.Network</span></span>
  - <span data-ttu-id="8d30d-577">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-577">Az.Resources</span></span>
  - <span data-ttu-id="8d30d-578">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-578">Az.Storage</span></span>
  - <span data-ttu-id="8d30d-579">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-579">Az.Websites</span></span>
* <span data-ttu-id="8d30d-580">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-580">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="8d30d-581">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8d30d-581">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="8d30d-582">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="8d30d-582">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="8d30d-583">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-583">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-584">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-584">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-585">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="8d30d-585">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-586">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-586">Az.Compute</span></span>
* <span data-ttu-id="8d30d-587">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="8d30d-587">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="8d30d-588">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="8d30d-588">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="8d30d-589">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="8d30d-589">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="8d30d-590">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="8d30d-590">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="8d30d-591">[#11354]</span><span class="sxs-lookup"><span data-stu-id="8d30d-591">[#11354]</span></span>
* <span data-ttu-id="8d30d-592">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="8d30d-592">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="8d30d-593">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8d30d-593">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="8d30d-594">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8d30d-594">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="8d30d-595">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8d30d-595">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="8d30d-596">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8d30d-596">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="8d30d-597">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-597">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="8d30d-598">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="8d30d-598">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="8d30d-599">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-599">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="8d30d-600">[#11257]</span><span class="sxs-lookup"><span data-stu-id="8d30d-600">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-601">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-601">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-602">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-602">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="8d30d-603">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="8d30d-603">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-604">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-604">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-605">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="8d30d-605">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="8d30d-606">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="8d30d-606">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-607">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-607">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-608">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="8d30d-608">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-609">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-609">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-610">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d30d-610">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="8d30d-611">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-611">New Cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-612">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="8d30d-612">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="8d30d-613">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="8d30d-613">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-614">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-614">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-615">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="8d30d-615">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-616">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-616">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-617">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="8d30d-617">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-618">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-618">Az.Network</span></span>
* <span data-ttu-id="8d30d-619">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="8d30d-619">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="8d30d-620">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-620">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="8d30d-621">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="8d30d-621">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="8d30d-622">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="8d30d-622">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="8d30d-623">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="8d30d-623">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="8d30d-624">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="8d30d-624">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-625">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-625">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-626">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="8d30d-626">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-627">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-627">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-628">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-628">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="8d30d-629">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="8d30d-629">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="8d30d-630">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-630">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="8d30d-631">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="8d30d-631">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="8d30d-632">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-632">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="8d30d-633">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="8d30d-633">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-634">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-634">Az.Resources</span></span>
* <span data-ttu-id="8d30d-635">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="8d30d-635">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="8d30d-636">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="8d30d-636">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="8d30d-637">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="8d30d-637">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="8d30d-638">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-638">Added example.</span></span>
* <span data-ttu-id="8d30d-639">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="8d30d-639">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="8d30d-640">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="8d30d-640">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-641">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-641">Az.Sql</span></span>
* <span data-ttu-id="8d30d-642">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="8d30d-642">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="8d30d-643">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="8d30d-643">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="8d30d-644">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-644">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="8d30d-645">Az.Support</span><span class="sxs-lookup"><span data-stu-id="8d30d-645">Az.Support</span></span>
* <span data-ttu-id="8d30d-646">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="8d30d-646">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-647">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-647">Az.Websites</span></span>
* <span data-ttu-id="8d30d-648">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="8d30d-648">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="8d30d-649">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8d30d-649">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="8d30d-650">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8d30d-650">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="8d30d-651">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8d30d-651">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="8d30d-652">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8d30d-652">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="8d30d-653">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-653">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-654">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-654">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-655">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="8d30d-655">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="8d30d-656">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="8d30d-656">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="8d30d-657">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="8d30d-657">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-658">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-658">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-659">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="8d30d-659">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="8d30d-660">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="8d30d-660">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="8d30d-661">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="8d30d-661">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="8d30d-662">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="8d30d-662">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-663">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-663">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-664">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="8d30d-664">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-665">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-665">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-666">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-666">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="8d30d-667">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-667">New Cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-668">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-668">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8d30d-669">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-669">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8d30d-670">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-670">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8d30d-671">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-671">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="8d30d-672">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-672">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="8d30d-673">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-673">New Cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-674">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8d30d-674">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="8d30d-675">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8d30d-675">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="8d30d-676">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8d30d-676">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="8d30d-677">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8d30d-677">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="8d30d-678">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-678">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="8d30d-679">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-679">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="8d30d-680">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-680">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="8d30d-681">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-681">New Cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-682">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="8d30d-682">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="8d30d-683">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="8d30d-683">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="8d30d-684">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d30d-684">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-685">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-685">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-686">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="8d30d-686">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-687">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-687">Az.Network</span></span>
* <span data-ttu-id="8d30d-688">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-688">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="8d30d-689">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="8d30d-689">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="8d30d-690">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="8d30d-690">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="8d30d-691">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-691">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-692">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-692">Az.Resources</span></span>
* <span data-ttu-id="8d30d-693">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-693">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="8d30d-694">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="8d30d-694">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="8d30d-695">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="8d30d-695">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="8d30d-696">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="8d30d-696">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="8d30d-697">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="8d30d-697">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="8d30d-698">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="8d30d-698">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="8d30d-699">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="8d30d-699">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="8d30d-700">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8d30d-700">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="8d30d-701">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8d30d-701">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="8d30d-702">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8d30d-702">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="8d30d-703">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8d30d-703">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="8d30d-704">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="8d30d-704">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="8d30d-705">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8d30d-705">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="8d30d-706">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-706">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-707">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-707">Az.Sql</span></span>
* <span data-ttu-id="8d30d-708">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-708">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="8d30d-709">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="8d30d-709">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="8d30d-710">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="8d30d-710">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="8d30d-711">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="8d30d-711">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="8d30d-712">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="8d30d-712">Remove an LTR backup</span></span>
    - <span data-ttu-id="8d30d-713">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="8d30d-713">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="8d30d-714">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="8d30d-714">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="8d30d-715">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-715">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="8d30d-716">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-716">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-717">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-717">Az.Storage</span></span>
* <span data-ttu-id="8d30d-718">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-718">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="8d30d-719">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="8d30d-719">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="8d30d-720">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="8d30d-720">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="8d30d-721">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="8d30d-721">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="8d30d-722">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="8d30d-722">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-723">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-723">Az.Websites</span></span>
* <span data-ttu-id="8d30d-724">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="8d30d-724">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="8d30d-725">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="8d30d-725">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="8d30d-726">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="8d30d-726">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="8d30d-727">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="8d30d-727">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="8d30d-728">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="8d30d-728">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="8d30d-729">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-729">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d30d-730">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8d30d-730">Highlights since the last major release</span></span>
* <span data-ttu-id="8d30d-731">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-731">Updated client side telemetry.</span></span>
* <span data-ttu-id="8d30d-732">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-732">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="8d30d-733">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d30d-733">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-734">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-734">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-735">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="8d30d-735">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-736">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-736">Az.Automation</span></span>
* <span data-ttu-id="8d30d-737">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8d30d-737">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-738">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-738">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-739">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-739">Updated SDK to 7.0</span></span>
* <span data-ttu-id="8d30d-740">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="8d30d-740">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-741">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-741">Az.Compute</span></span>
* <span data-ttu-id="8d30d-742">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="8d30d-742">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-743">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-743">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-744">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="8d30d-744">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-745">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-745">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-746">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8d30d-746">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="8d30d-747">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-747">New Cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-748">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-748">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8d30d-749">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-749">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8d30d-750">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-750">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8d30d-751">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8d30d-751">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-752">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-752">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-753">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="8d30d-753">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-754">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-754">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-755">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="8d30d-755">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="8d30d-756">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="8d30d-756">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="8d30d-757">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="8d30d-757">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-758">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-758">Az.Network</span></span>
* <span data-ttu-id="8d30d-759">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="8d30d-759">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="8d30d-760">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="8d30d-760">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="8d30d-761">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="8d30d-761">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="8d30d-762">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="8d30d-762">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="8d30d-763">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8d30d-763">No new cmdlets are added.</span></span> <span data-ttu-id="8d30d-764">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="8d30d-764">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-765">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-765">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-766">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="8d30d-766">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-767">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-767">Az.Resources</span></span>
* <span data-ttu-id="8d30d-768">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="8d30d-768">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="8d30d-769">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="8d30d-769">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="8d30d-770">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="8d30d-770">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="8d30d-771">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="8d30d-771">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="8d30d-772">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="8d30d-772">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="8d30d-773">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="8d30d-773">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="8d30d-774">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="8d30d-774">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="8d30d-775">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="8d30d-775">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-776">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-776">Az.Sql</span></span>
* <span data-ttu-id="8d30d-777">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-777">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="8d30d-778">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="8d30d-778">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="8d30d-779">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="8d30d-779">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="8d30d-780">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8d30d-780">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="8d30d-781">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="8d30d-781">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d30d-782">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d30d-782">Az.StorageSync</span></span>
* <span data-ttu-id="8d30d-783">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="8d30d-783">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="8d30d-784">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-784">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d30d-785">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8d30d-785">Highlights since the last major release</span></span>
* <span data-ttu-id="8d30d-786">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="8d30d-786">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="8d30d-787">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="8d30d-787">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-788">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-788">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-789">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="8d30d-789">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="8d30d-790">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="8d30d-790">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-791">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-791">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-792">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="8d30d-792">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="8d30d-793">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="8d30d-793">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="8d30d-794">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="8d30d-794">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="8d30d-795">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="8d30d-795">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-796">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-796">Az.Compute</span></span>
* <span data-ttu-id="8d30d-797">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="8d30d-797">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="8d30d-798">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-798">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="8d30d-799">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-799">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="8d30d-800">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-800">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="8d30d-801">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="8d30d-801">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-802">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-802">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-803">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-803">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8d30d-804">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8d30d-804">Az.DeploymentManager</span></span>
* <span data-ttu-id="8d30d-805">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="8d30d-805">Adds LIST operations for resources</span></span>
* <span data-ttu-id="8d30d-806">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-806">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-807">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-807">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-808">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="8d30d-808">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-809">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-809">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-810">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="8d30d-810">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-811">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-811">Az.Network</span></span>
* <span data-ttu-id="8d30d-812">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="8d30d-812">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="8d30d-813">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="8d30d-813">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="8d30d-814">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-814">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8d30d-815">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="8d30d-815">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="8d30d-816">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-816">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="8d30d-817">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="8d30d-817">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="8d30d-818">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8d30d-818">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="8d30d-819">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-819">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="8d30d-820">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-820">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-821">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-821">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="8d30d-822">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-822">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="8d30d-823">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-823">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="8d30d-824">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="8d30d-824">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-825">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-825">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-826">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="8d30d-826">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="8d30d-827">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="8d30d-827">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="8d30d-828">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="8d30d-828">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="8d30d-829">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="8d30d-829">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-830">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-830">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-831">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-831">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="8d30d-832">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="8d30d-832">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-833">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-833">Az.Resources</span></span>
* <span data-ttu-id="8d30d-834">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="8d30d-834">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="8d30d-835">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="8d30d-835">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-836">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-836">Az.Sql</span></span>
<span data-ttu-id="8d30d-837">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="8d30d-837">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-838">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-838">Az.Storage</span></span>
* <span data-ttu-id="8d30d-839">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-839">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="8d30d-840">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-840">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d30d-841">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="8d30d-841">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="8d30d-842">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8d30d-842">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-843">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-843">Az.Websites</span></span>
* <span data-ttu-id="8d30d-844">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="8d30d-844">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="8d30d-845">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="8d30d-845">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="8d30d-846">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="8d30d-846">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-847">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-847">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-848">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="8d30d-848">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-849">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-849">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-850">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d30d-850">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-851">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-851">Az.Compute</span></span>
* <span data-ttu-id="8d30d-852">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="8d30d-852">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="8d30d-853">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-853">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d30d-854">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-854">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="8d30d-855">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8d30d-855">Az.DataBoxEdge</span></span>
* <span data-ttu-id="8d30d-856">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-856">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8d30d-857">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-857">Get the Edge Storage Container</span></span>
* <span data-ttu-id="8d30d-858">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-858">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8d30d-859">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-859">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="8d30d-860">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-860">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8d30d-861">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-861">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="8d30d-862">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-862">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8d30d-863">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-863">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="8d30d-864">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-864">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8d30d-865">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-865">Get the Edge Storage Account</span></span>
* <span data-ttu-id="8d30d-866">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-866">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8d30d-867">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-867">Create new Edge Storage Account</span></span>
* <span data-ttu-id="8d30d-868">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8d30d-868">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8d30d-869">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8d30d-869">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="8d30d-870">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="8d30d-870">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="8d30d-871">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="8d30d-871">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="8d30d-872">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="8d30d-872">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="8d30d-873">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="8d30d-873">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-874">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-874">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-875">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="8d30d-875">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="8d30d-876">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-876">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="8d30d-877">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-877">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="8d30d-878">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="8d30d-878">Az.DevTestLabs</span></span>
* <span data-ttu-id="8d30d-879">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="8d30d-879">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-880">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-880">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-881">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="8d30d-881">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-882">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-882">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-883">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="8d30d-883">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8d30d-884">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d30d-884">Az.MachineLearning</span></span>
* <span data-ttu-id="8d30d-885">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="8d30d-885">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="8d30d-886">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8d30d-886">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="8d30d-887">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-887">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="8d30d-888">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8d30d-888">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="8d30d-889">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8d30d-889">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="8d30d-890">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8d30d-890">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="8d30d-891">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="8d30d-891">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="8d30d-892">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="8d30d-892">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-893">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-893">Az.Network</span></span>
* <span data-ttu-id="8d30d-894">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="8d30d-894">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-895">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-895">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-896">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-896">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="8d30d-897">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-897">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="8d30d-898">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-898">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="8d30d-899">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-899">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-900">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-900">Az.Resources</span></span>
* <span data-ttu-id="8d30d-901">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="8d30d-901">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-902">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-902">Az.Sql</span></span>
* <span data-ttu-id="8d30d-903">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="8d30d-903">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="8d30d-904">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="8d30d-904">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="8d30d-905">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8d30d-905">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="8d30d-906">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="8d30d-906">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-907">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-907">Az.Storage</span></span>
* <span data-ttu-id="8d30d-908">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="8d30d-908">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="8d30d-909">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-909">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="8d30d-910">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="8d30d-910">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="8d30d-911">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-911">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="8d30d-912">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-912">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="8d30d-913">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-913">General</span></span>
* <span data-ttu-id="8d30d-914">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="8d30d-914">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-915">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-915">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-916">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-916">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="8d30d-917">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-917">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-918">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-918">Az.Batch</span></span>
* <span data-ttu-id="8d30d-919">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="8d30d-919">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-920">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-920">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-921">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-921">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-922">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-922">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-923">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="8d30d-923">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="8d30d-924">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="8d30d-924">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8d30d-925">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8d30d-925">Az.HealthcareApis</span></span>
* <span data-ttu-id="8d30d-926">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="8d30d-926">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-927">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-927">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-928">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="8d30d-928">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="8d30d-929">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="8d30d-929">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="8d30d-930">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="8d30d-930">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-931">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-931">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-932">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="8d30d-932">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="8d30d-933">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="8d30d-933">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="8d30d-934">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="8d30d-934">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-935">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-935">Az.Network</span></span>
* <span data-ttu-id="8d30d-936">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="8d30d-936">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-937">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-937">Az.Resources</span></span>
* <span data-ttu-id="8d30d-938">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-938">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="8d30d-939">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-939">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-940">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-940">Az.Sql</span></span>
* <span data-ttu-id="8d30d-941">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="8d30d-941">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-942">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-942">Az.Storage</span></span>
* <span data-ttu-id="8d30d-943">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="8d30d-943">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="8d30d-944">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="8d30d-944">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="8d30d-945">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8d30d-945">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="8d30d-946">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="8d30d-946">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="8d30d-947">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="8d30d-947">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="8d30d-948">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="8d30d-948">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="8d30d-949">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="8d30d-949">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="8d30d-950">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-950">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="8d30d-951">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-951">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="8d30d-952">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="8d30d-952">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="8d30d-953">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="8d30d-953">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="8d30d-954">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="8d30d-954">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="8d30d-955">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="8d30d-955">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="8d30d-956">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-956">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d30d-957">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8d30d-957">Highlights since the last major release</span></span>
* <span data-ttu-id="8d30d-958">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="8d30d-958">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="8d30d-959">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="8d30d-959">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-960">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-960">Az.Compute</span></span>
* <span data-ttu-id="8d30d-961">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="8d30d-961">VM Reapply feature</span></span>
    - <span data-ttu-id="8d30d-962">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d30d-962">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="8d30d-963">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="8d30d-963">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="8d30d-964">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-964">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="8d30d-965">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d30d-965">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="8d30d-966">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-966">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="8d30d-967">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="8d30d-967">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="8d30d-968">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="8d30d-968">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="8d30d-969">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="8d30d-969">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="8d30d-970">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="8d30d-970">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="8d30d-971">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-971">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="8d30d-972">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8d30d-972">Az.DataBoxEdge</span></span>
* <span data-ttu-id="8d30d-973">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="8d30d-973">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8d30d-974">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="8d30d-974">Get the Order</span></span>
* <span data-ttu-id="8d30d-975">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="8d30d-975">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8d30d-976">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="8d30d-976">Create new Order</span></span>
* <span data-ttu-id="8d30d-977">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="8d30d-977">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8d30d-978">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="8d30d-978">Remove the Order</span></span>
* <span data-ttu-id="8d30d-979">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="8d30d-979">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="8d30d-980">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="8d30d-980">Now creates Local Share</span></span>
* <span data-ttu-id="8d30d-981">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="8d30d-981">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="8d30d-982">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="8d30d-982">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="8d30d-983">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="8d30d-983">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="8d30d-984">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="8d30d-984">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="8d30d-985">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="8d30d-985">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8d30d-986">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="8d30d-986">Gets the information about Triggers</span></span>
* <span data-ttu-id="8d30d-987">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="8d30d-987">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8d30d-988">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="8d30d-988">Create new Triggers</span></span>
* <span data-ttu-id="8d30d-989">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="8d30d-989">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8d30d-990">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="8d30d-990">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-991">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-991">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-992">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-992">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="8d30d-993">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-993">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-994">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-994">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-995">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="8d30d-995">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-996">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-996">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-997">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="8d30d-997">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-998">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-998">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-999">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-999">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="8d30d-1000">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-1000">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="8d30d-1001">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="8d30d-1001">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="8d30d-1002">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-1002">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1003">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1003">Az.Network</span></span>
* <span data-ttu-id="8d30d-1004">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1004">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="8d30d-1005">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="8d30d-1005">Az.PrivateDns</span></span>
* <span data-ttu-id="8d30d-1006">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1006">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1007">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1007">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1008">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1008">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="8d30d-1009">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1009">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="8d30d-1010">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1010">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d30d-1011">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d30d-1011">Az.RedisCache</span></span>
* <span data-ttu-id="8d30d-1012">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1012">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="8d30d-1013">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1013">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="8d30d-1014">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1014">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1015">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1015">Az.Resources</span></span>
- <span data-ttu-id="8d30d-1016">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1016">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="8d30d-1017">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="8d30d-1017">Updated create policy definition help example</span></span>
- <span data-ttu-id="8d30d-1018">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1018">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="8d30d-1019">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1019">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="8d30d-1020">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1020">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1021">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1021">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1022">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1022">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="8d30d-1023">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="8d30d-1023">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="8d30d-1024">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1024">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="8d30d-1025">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-1025">General</span></span>
* <span data-ttu-id="8d30d-1026">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1026">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1027">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1027">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1028">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1028">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8d30d-1029">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1029">Az.Advisor</span></span>
* <span data-ttu-id="8d30d-1030">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1030">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-1031">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-1031">Az.Batch</span></span>
* <span data-ttu-id="8d30d-1032">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1032">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="8d30d-1033">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1033">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="8d30d-1034">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1034">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="8d30d-1035">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1035">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="8d30d-1036">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1036">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="8d30d-1037">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1037">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="8d30d-1038">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1038">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="8d30d-1039">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1039">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="8d30d-1040">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1040">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="8d30d-1041">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1041">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="8d30d-1042">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1042">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="8d30d-1043">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1043">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="8d30d-1044">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1044">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="8d30d-1045">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1045">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="8d30d-1046">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1046">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="8d30d-1047">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1047">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="8d30d-1048">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1048">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="8d30d-1049">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1049">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="8d30d-1050">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1050">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="8d30d-1051">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1051">This operation is no longer supported.</span></span>
* <span data-ttu-id="8d30d-1052">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1052">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="8d30d-1053">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1053">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="8d30d-1054">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1054">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="8d30d-1055">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1055">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="8d30d-1056">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1056">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="8d30d-1057">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1057">New non-verified images are also now returned.</span></span> <span data-ttu-id="8d30d-1058">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1058">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="8d30d-1059">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1059">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="8d30d-1060">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1060">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="8d30d-1061">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1061">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="8d30d-1062">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1062">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="8d30d-1063">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1063">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="8d30d-1064">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1064">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="8d30d-1065">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1065">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="8d30d-1066">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="8d30d-1066">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="8d30d-1067">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="8d30d-1067">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-1068">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-1068">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-1069">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1069">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="8d30d-1070">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1070">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1071">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1071">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1072">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="8d30d-1072">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="8d30d-1073">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-1073">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="8d30d-1074">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="8d30d-1074">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="8d30d-1075">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1075">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8d30d-1076">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1076">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="8d30d-1077">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="8d30d-1077">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="8d30d-1078">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-1078">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="8d30d-1079">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1079">Breaking changes</span></span>
    - <span data-ttu-id="8d30d-1080">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="8d30d-1080">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="8d30d-1081">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="8d30d-1081">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-1082">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-1082">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-1083">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1083">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-1084">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-1084">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-1085">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="8d30d-1085">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="8d30d-1086">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1086">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="8d30d-1087">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="8d30d-1087">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="8d30d-1088">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="8d30d-1088">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="8d30d-1089">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="8d30d-1089">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="8d30d-1090">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="8d30d-1090">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-1091">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1091">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-1092">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="8d30d-1092">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-1093">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-1093">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-1094">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1094">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="8d30d-1095">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1095">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="8d30d-1096">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1096">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="8d30d-1097">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1097">Removed five cmdlets:</span></span>
    - <span data-ttu-id="8d30d-1098">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8d30d-1098">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8d30d-1099">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8d30d-1099">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8d30d-1100">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8d30d-1100">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8d30d-1101">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d30d-1101">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="8d30d-1102">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d30d-1102">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="8d30d-1103">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1103">Added three cmdlets:</span></span>
    - <span data-ttu-id="8d30d-1104">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1104">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="8d30d-1105">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1105">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="8d30d-1106">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1106">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="8d30d-1107">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1107">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="8d30d-1108">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1108">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="8d30d-1109">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1109">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="8d30d-1110">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1110">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="8d30d-1111">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1111">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="8d30d-1112">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1112">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="8d30d-1113">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1113">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="8d30d-1114">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1114">Added some scenario test cases.</span></span>
* <span data-ttu-id="8d30d-1115">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1115">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-1116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1116">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-1117">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1117">Breaking changes:</span></span>
    - <span data-ttu-id="8d30d-1118">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1118">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8d30d-1119">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1119">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8d30d-1120">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1120">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8d30d-1121">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1121">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8d30d-1122">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1122">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="8d30d-1123">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1123">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="8d30d-1124">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1124">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="8d30d-1125">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1125">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="8d30d-1126">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1126">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8d30d-1127">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1127">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8d30d-1128">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1128">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8d30d-1129">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1129">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1130">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1130">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1131">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1131">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1132">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1132">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="8d30d-1133">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1133">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="8d30d-1134">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1134">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1135">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1135">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1136">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1136">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1137">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1137">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1138">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1138">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1139">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="8d30d-1139">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1140">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1140">Az.Resources</span></span>
* <span data-ttu-id="8d30d-1141">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="8d30d-1141">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1142">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1142">Az.Network</span></span>
* <span data-ttu-id="8d30d-1143">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1143">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="8d30d-1144">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1144">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d30d-1145">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1145">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1146">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1146">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1147">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1147">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1148">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1148">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1149">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1149">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8d30d-1150">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1150">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="8d30d-1151">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1151">New cmdlet:</span></span>
        - <span data-ttu-id="8d30d-1152">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="8d30d-1152">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="8d30d-1153">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1153">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="8d30d-1154">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1154">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="8d30d-1155">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1155">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="8d30d-1156">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1156">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="8d30d-1157">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1157">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="8d30d-1158">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-1158">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="8d30d-1159">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1159">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="8d30d-1160">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1160">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-1161">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1161">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="8d30d-1162">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-1162">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8d30d-1163">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-1163">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8d30d-1164">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-1164">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8d30d-1165">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1165">Set-AzVirtualHub</span></span>
* <span data-ttu-id="8d30d-1166">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="8d30d-1166">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="8d30d-1167">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1167">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8d30d-1168">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="8d30d-1168">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="8d30d-1169">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="8d30d-1169">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="8d30d-1170">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1170">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="8d30d-1171">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1171">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="8d30d-1172">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1172">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="8d30d-1173">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1173">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-1174">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1174">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="8d30d-1175">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1175">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8d30d-1176">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8d30d-1176">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8d30d-1177">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8d30d-1177">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8d30d-1178">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8d30d-1178">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8d30d-1179">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8d30d-1179">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8d30d-1180">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8d30d-1180">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="8d30d-1181">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="8d30d-1181">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="8d30d-1182">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1182">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-1183">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="8d30d-1183">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="8d30d-1184">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="8d30d-1184">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="8d30d-1185">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="8d30d-1185">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="8d30d-1186">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="8d30d-1186">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="8d30d-1187">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1187">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="8d30d-1188">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-1188">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="8d30d-1189">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1189">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8d30d-1190">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1190">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="8d30d-1191">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1191">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="8d30d-1192">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="8d30d-1192">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="8d30d-1193">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="8d30d-1193">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="8d30d-1194">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1194">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8d30d-1195">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="8d30d-1195">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="8d30d-1196">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="8d30d-1196">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="8d30d-1197">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1197">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="8d30d-1198">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-1198">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="8d30d-1199">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1199">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="8d30d-1200">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1200">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-1201">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1201">New-AzIpGroup</span></span>
        - <span data-ttu-id="8d30d-1202">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1202">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="8d30d-1203">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1203">Get-AzIpGroup</span></span>
        - <span data-ttu-id="8d30d-1204">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1204">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-1205">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1205">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-1206">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1206">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1207">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1207">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1208">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1208">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="8d30d-1209">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1209">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="8d30d-1210">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1210">Removed deprecated aliases:</span></span>
* <span data-ttu-id="8d30d-1211">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1211">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="8d30d-1212">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1212">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="8d30d-1213">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1213">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8d30d-1214">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="8d30d-1214">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="8d30d-1215">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="8d30d-1215">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="8d30d-1216">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1216">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1217">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1217">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1218">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-1218">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="8d30d-1219">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1219">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8d30d-1220">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1220">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8d30d-1221">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="8d30d-1221">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="8d30d-1222">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d30d-1222">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="8d30d-1223">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d30d-1223">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="8d30d-1224">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1224">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="8d30d-1225">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-1225">General</span></span>
* <span data-ttu-id="8d30d-1226">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1226">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1227">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1227">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1228">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1228">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-1229">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1229">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-1230">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-1230">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="8d30d-1231">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="8d30d-1231">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-1232">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1232">Az.Automation</span></span>
* <span data-ttu-id="8d30d-1233">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1233">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-1234">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-1234">Az.Batch</span></span>
* <span data-ttu-id="8d30d-1235">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1235">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1236">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1236">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1237">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-1237">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="8d30d-1238">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-1238">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="8d30d-1239">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1239">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="8d30d-1240">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1240">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-1241">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-1241">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-1242">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1242">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="8d30d-1243">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1243">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="8d30d-1244">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1244">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-1245">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-1245">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-1246">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="8d30d-1246">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8d30d-1247">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8d30d-1247">Az.HealthcareApis</span></span>
* <span data-ttu-id="8d30d-1248">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1248">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="8d30d-1249">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="8d30d-1249">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="8d30d-1250">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="8d30d-1250">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="8d30d-1251">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1251">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-1252">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1252">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-1253">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="8d30d-1253">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="8d30d-1254">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="8d30d-1254">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-1255">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1255">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-1256">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="8d30d-1256">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="8d30d-1257">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1257">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="8d30d-1258">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="8d30d-1258">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="8d30d-1259">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1259">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1260">Az.Network</span></span>
* <span data-ttu-id="8d30d-1261">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1261">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="8d30d-1262">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8d30d-1262">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="8d30d-1263">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1263">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-1264">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1264">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="8d30d-1265">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1265">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8d30d-1266">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="8d30d-1266">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="8d30d-1267">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1267">Updated cmdlets:</span></span>
        - <span data-ttu-id="8d30d-1268">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1268">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8d30d-1269">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1269">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8d30d-1270">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1270">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8d30d-1271">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="8d30d-1271">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="8d30d-1272">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="8d30d-1272">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="8d30d-1273">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1273">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="8d30d-1274">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1274">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d30d-1275">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d30d-1275">Az.RedisCache</span></span>
* <span data-ttu-id="8d30d-1276">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1276">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1277">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1278">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="8d30d-1278">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1279">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1279">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1280">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1280">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="8d30d-1281">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="8d30d-1281">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="8d30d-1282">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="8d30d-1282">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="8d30d-1283">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="8d30d-1283">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="8d30d-1284">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1284">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d30d-1285">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d30d-1285">Az.StorageSync</span></span>
* <span data-ttu-id="8d30d-1286">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1286">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1287">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1287">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1288">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="8d30d-1288">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="8d30d-1289">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1289">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-1290">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1290">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-1291">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1291">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="8d30d-1292">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1292">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="8d30d-1293">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1293">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-1294">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1294">Az.Automation</span></span>
* <span data-ttu-id="8d30d-1295">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1295">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="8d30d-1296">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="8d30d-1296">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="8d30d-1297">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1297">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1298">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1298">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1299">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1299">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="8d30d-1300">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1300">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8d30d-1301">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1301">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="8d30d-1302">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1302">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="8d30d-1303">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1303">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="8d30d-1304">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1304">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="8d30d-1305">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1305">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="8d30d-1306">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1306">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="8d30d-1307">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1307">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-1308">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-1308">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-1309">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="8d30d-1309">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="8d30d-1310">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="8d30d-1310">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-1311">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-1311">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-1312">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1312">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-1313">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1313">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-1314">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1314">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="8d30d-1315">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1315">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="8d30d-1316">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1316">New cmdlets are:</span></span>
    - <span data-ttu-id="8d30d-1317">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8d30d-1317">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8d30d-1318">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8d30d-1318">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8d30d-1319">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8d30d-1319">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8d30d-1320">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8d30d-1320">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-1321">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1321">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-1322">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="8d30d-1322">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="8d30d-1323">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1323">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="8d30d-1324">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1324">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="8d30d-1325">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1325">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="8d30d-1326">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1326">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="8d30d-1327">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1327">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="8d30d-1328">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1328">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="8d30d-1329">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1329">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="8d30d-1330">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1330">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="8d30d-1331">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1331">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="8d30d-1332">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1332">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="8d30d-1333">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1333">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="8d30d-1334">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="8d30d-1334">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="8d30d-1335">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="8d30d-1335">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="8d30d-1336">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="8d30d-1336">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="8d30d-1337">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1337">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="8d30d-1338">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1338">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="8d30d-1339">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-1339">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="8d30d-1340">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1340">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="8d30d-1341">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-1341">Overall improved help files</span></span>
* <span data-ttu-id="8d30d-1342">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1342">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1343">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1343">Az.Network</span></span>
* <span data-ttu-id="8d30d-1344">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1344">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="8d30d-1345">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="8d30d-1345">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="8d30d-1346">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="8d30d-1346">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="8d30d-1347">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="8d30d-1347">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="8d30d-1348">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="8d30d-1348">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="8d30d-1349">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="8d30d-1349">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="8d30d-1350">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1350">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="8d30d-1351">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="8d30d-1351">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="8d30d-1352">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-1352">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="8d30d-1353">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1353">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="8d30d-1354">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-1354">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="8d30d-1355">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="8d30d-1355">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="8d30d-1356">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1356">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1357">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="8d30d-1357">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="8d30d-1358">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1358">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="8d30d-1359">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1359">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d30d-1360">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="8d30d-1360">New-VpnSite</span></span>
        - <span data-ttu-id="8d30d-1361">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="8d30d-1361">Update-VpnSite</span></span>
        - <span data-ttu-id="8d30d-1362">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1362">New-VpnConnection</span></span>
        - <span data-ttu-id="8d30d-1363">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1363">Update-VpnConnection</span></span>
* <span data-ttu-id="8d30d-1364">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="8d30d-1364">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1365">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1365">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1366">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1366">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="8d30d-1367">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="8d30d-1367">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1368">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1368">Az.Resources</span></span>
* <span data-ttu-id="8d30d-1369">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1369">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-1370">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1370">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-1371">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1371">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="8d30d-1372">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1372">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="8d30d-1373">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8d30d-1373">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8d30d-1374">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1374">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8d30d-1375">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8d30d-1375">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8d30d-1376">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1376">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="8d30d-1377">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8d30d-1377">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8d30d-1378">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8d30d-1378">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8d30d-1379">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1379">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8d30d-1380">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8d30d-1380">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8d30d-1381">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1381">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="8d30d-1382">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8d30d-1382">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8d30d-1383">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1383">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8d30d-1384">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8d30d-1384">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8d30d-1385">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="8d30d-1385">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="8d30d-1386">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1386">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d30d-1387">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d30d-1387">Az.SignalR</span></span>
* <span data-ttu-id="8d30d-1388">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1388">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1389">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1389">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1390">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1390">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="8d30d-1391">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="8d30d-1391">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="8d30d-1392">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1392">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="8d30d-1393">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1393">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="8d30d-1394">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="8d30d-1394">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1395">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1395">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1396">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1396">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="8d30d-1397">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="8d30d-1397">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="8d30d-1398">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-1398">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="8d30d-1399">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-1399">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="8d30d-1400">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1400">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="8d30d-1401">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-1401">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="8d30d-1402">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="8d30d-1402">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="8d30d-1403">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-1403">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8d30d-1404">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-1404">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8d30d-1405">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-1405">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8d30d-1406">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-1406">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1407">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1407">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1408">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="8d30d-1408">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="8d30d-1409">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="8d30d-1409">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="8d30d-1410">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1410">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="8d30d-1411">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1411">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="8d30d-1412">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-1412">General</span></span>
* <span data-ttu-id="8d30d-1413">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="8d30d-1413">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1414">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1414">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1415">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1415">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="8d30d-1416">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8d30d-1416">Az.Aks</span></span>
* <span data-ttu-id="8d30d-1417">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1417">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="8d30d-1418">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="8d30d-1418">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-1419">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1419">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-1420">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="8d30d-1420">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="8d30d-1421">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="8d30d-1421">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="8d30d-1422">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1422">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="8d30d-1423">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="8d30d-1423">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="8d30d-1424">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1424">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-1425">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-1425">Az.Batch</span></span>
* <span data-ttu-id="8d30d-1426">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="8d30d-1426">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-1427">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-1427">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-1428">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="8d30d-1428">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1429">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1429">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1430">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1430">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="8d30d-1431">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-1431">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="8d30d-1432">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="8d30d-1432">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="8d30d-1433">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1433">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="8d30d-1434">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="8d30d-1434">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="8d30d-1435">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d30d-1435">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="8d30d-1436">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="8d30d-1436">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="8d30d-1437">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1437">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-1438">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-1438">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-1439">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1439">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="8d30d-1440">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="8d30d-1440">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="8d30d-1441">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="8d30d-1441">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="8d30d-1442">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="8d30d-1442">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-1443">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-1443">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-1444">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1444">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-1445">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1445">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-1446">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-1446">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="8d30d-1447">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="8d30d-1447">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="8d30d-1448">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="8d30d-1448">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="8d30d-1449">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="8d30d-1449">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="8d30d-1450">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8d30d-1450">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8d30d-1451">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1451">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-1452">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1452">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-1453">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-1453">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1454">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1454">Az.Network</span></span>
* <span data-ttu-id="8d30d-1455">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1455">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="8d30d-1456">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1456">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="8d30d-1457">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1457">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="8d30d-1458">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="8d30d-1458">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="8d30d-1459">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1459">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="8d30d-1460">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1460">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="8d30d-1461">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="8d30d-1461">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-1462">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1462">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-1463">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1463">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="8d30d-1464">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1464">Added example</span></span>
    - <span data-ttu-id="8d30d-1465">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1465">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="8d30d-1466">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="8d30d-1466">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="8d30d-1467">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="8d30d-1467">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1468">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1468">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1469">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1469">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1470">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1470">Az.Resources</span></span>
* <span data-ttu-id="8d30d-1471">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="8d30d-1471">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="8d30d-1472">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="8d30d-1472">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="8d30d-1473">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="8d30d-1473">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="8d30d-1474">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-1474">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d30d-1475">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d30d-1475">Az.ServiceBus</span></span>
* <span data-ttu-id="8d30d-1476">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-1476">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="8d30d-1477">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="8d30d-1477">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="8d30d-1478">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="8d30d-1478">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-1479">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1479">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-1480">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1480">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="8d30d-1481">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1481">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="8d30d-1482">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="8d30d-1482">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="8d30d-1483">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1483">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="8d30d-1484">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="8d30d-1484">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="8d30d-1485">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="8d30d-1485">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1486">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1486">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1487">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1487">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1488">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1488">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1489">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1489">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="8d30d-1490">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="8d30d-1490">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="8d30d-1491">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-1491">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="8d30d-1492">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1492">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="8d30d-1493">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="8d30d-1493">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="8d30d-1494">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1494">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1495">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1495">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1496">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8d30d-1496">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="8d30d-1497">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1497">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1498">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1498">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1499">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8d30d-1499">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="8d30d-1500">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1500">Az.ApplicationInsights</span></span>
* <span data-ttu-id="8d30d-1501">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1501">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-1502">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1502">Az.Automation</span></span>
* <span data-ttu-id="8d30d-1503">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="8d30d-1503">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-1504">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1504">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-1505">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1505">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1506">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1506">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1507">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1507">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8d30d-1508">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8d30d-1508">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8d30d-1509">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-1509">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="8d30d-1510">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="8d30d-1510">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-1511">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-1511">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-1512">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-1512">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="8d30d-1513">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1513">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-1514">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1514">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-1515">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8d30d-1515">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8d30d-1516">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="8d30d-1516">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-1517">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-1517">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-1518">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1518">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d30d-1519">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-1519">Az.LogicApp</span></span>
* <span data-ttu-id="8d30d-1520">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="8d30d-1520">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="8d30d-1521">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="8d30d-1521">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="8d30d-1522">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1522">Az.ManagedServices</span></span>
* <span data-ttu-id="8d30d-1523">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1523">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1524">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1524">Az.Network</span></span>
* <span data-ttu-id="8d30d-1525">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="8d30d-1525">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="8d30d-1526">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1526">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1527">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d30d-1527">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d30d-1528">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1528">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d30d-1529">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1529">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1530">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1530">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1531">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1531">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1532">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1532">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d30d-1533">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="8d30d-1533">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="8d30d-1534">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1534">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="8d30d-1535">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="8d30d-1535">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="8d30d-1536">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1536">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="8d30d-1537">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1537">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="8d30d-1538">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1538">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="8d30d-1539">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="8d30d-1539">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="8d30d-1540">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="8d30d-1540">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="8d30d-1541">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="8d30d-1541">Updated cmdlets</span></span>
        - <span data-ttu-id="8d30d-1542">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1542">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8d30d-1543">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1543">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8d30d-1544">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1544">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8d30d-1545">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1545">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8d30d-1546">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-1546">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="8d30d-1547">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1547">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d30d-1548">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1548">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8d30d-1549">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1549">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8d30d-1550">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1550">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="8d30d-1551">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="8d30d-1551">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="8d30d-1552">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1552">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="8d30d-1553">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1553">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-1554">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1554">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-1555">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1555">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="8d30d-1556">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1556">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1557">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1557">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1558">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1558">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8d30d-1559">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1559">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="8d30d-1560">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1560">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="8d30d-1561">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1561">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8d30d-1562">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1562">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="8d30d-1563">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1563">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8d30d-1564">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1564">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="8d30d-1565">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1565">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8d30d-1566">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-1566">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="8d30d-1567">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1567">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1568">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1568">Az.Resources</span></span>
- <span data-ttu-id="8d30d-1569">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1569">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="8d30d-1570">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="8d30d-1570">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d30d-1571">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d30d-1571">Az.ServiceBus</span></span>
* <span data-ttu-id="8d30d-1572">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8d30d-1572">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8d30d-1573">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="8d30d-1573">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1574">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1574">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1575">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="8d30d-1575">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="8d30d-1576">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="8d30d-1576">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="8d30d-1577">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1577">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1578">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1578">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1579">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="8d30d-1579">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d30d-1580">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d30d-1580">Az.StorageSync</span></span>
* <span data-ttu-id="8d30d-1581">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1581">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="8d30d-1582">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="8d30d-1582">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1583">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1583">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1584">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-1584">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="8d30d-1585">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-1585">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="8d30d-1586">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-1586">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="8d30d-1587">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1587">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1588">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1588">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1589">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="8d30d-1589">Add support for profile cmdlets</span></span>
* <span data-ttu-id="8d30d-1590">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="8d30d-1590">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="8d30d-1591">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="8d30d-1591">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8d30d-1592">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1592">Az.Advisor</span></span>
* <span data-ttu-id="8d30d-1593">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1593">GA release of Az.Advisor</span></span>
* <span data-ttu-id="8d30d-1594">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1594">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-1595">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1595">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-1596">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="8d30d-1596">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="8d30d-1597">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1597">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="8d30d-1598">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="8d30d-1598">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="8d30d-1599">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1599">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="8d30d-1600">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="8d30d-1600">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="8d30d-1601">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1601">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="8d30d-1602">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="8d30d-1602">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-1603">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1603">Az.Automation</span></span>
* <span data-ttu-id="8d30d-1604">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="8d30d-1604">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1605">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1605">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1606">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1606">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-1607">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-1607">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-1608">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1608">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d30d-1609">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d30d-1609">Az.EventGrid</span></span>
* <span data-ttu-id="8d30d-1610">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1610">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-1611">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1611">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-1612">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1612">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1613">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1613">Az.Network</span></span>
* <span data-ttu-id="8d30d-1614">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="8d30d-1614">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="8d30d-1615">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1615">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-1616">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1616">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-1617">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="8d30d-1617">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="8d30d-1618">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="8d30d-1618">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-1619">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1619">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-1620">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="8d30d-1620">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1621">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1621">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1622">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="8d30d-1622">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1623">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1623">Az.Resources</span></span>
    - <span data-ttu-id="8d30d-1624">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="8d30d-1624">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="8d30d-1625">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="8d30d-1625">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="8d30d-1626">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-1626">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="8d30d-1627">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="8d30d-1627">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d30d-1628">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d30d-1628">Az.ServiceBus</span></span>
* <span data-ttu-id="8d30d-1629">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="8d30d-1629">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1630">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1630">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1631">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="8d30d-1631">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="8d30d-1632">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1632">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="8d30d-1633">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1633">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d30d-1634">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1634">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d30d-1635">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1635">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d30d-1636">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1636">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8d30d-1637">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1637">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8d30d-1638">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1638">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="8d30d-1639">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="8d30d-1639">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1640">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1640">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1641">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1641">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="8d30d-1642">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d30d-1642">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="8d30d-1643">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="8d30d-1643">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="8d30d-1644">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="8d30d-1644">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="8d30d-1645">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-1645">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="8d30d-1646">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1646">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8d30d-1647">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1647">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8d30d-1648">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="8d30d-1648">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="8d30d-1649">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d30d-1649">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="8d30d-1650">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d30d-1650">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d30d-1651">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d30d-1651">Az.StorageSync</span></span>
* <span data-ttu-id="8d30d-1652">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1652">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="8d30d-1653">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1653">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1654">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1654">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1655">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="8d30d-1655">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="8d30d-1656">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="8d30d-1656">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="8d30d-1657">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8d30d-1657">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="8d30d-1658">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="8d30d-1658">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="8d30d-1659">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="8d30d-1659">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1660">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1660">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1661">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1661">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="8d30d-1662">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1662">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="8d30d-1663">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8d30d-1663">Az.Dns</span></span>
* <span data-ttu-id="8d30d-1664">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1664">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d30d-1665">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d30d-1665">Az.EventGrid</span></span>
* <span data-ttu-id="8d30d-1666">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1666">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="8d30d-1667">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1667">New cmdlets:</span></span>
    - <span data-ttu-id="8d30d-1668">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d30d-1668">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d30d-1669">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1669">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d30d-1670">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d30d-1670">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d30d-1671">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1671">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="8d30d-1672">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d30d-1672">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d30d-1673">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1673">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d30d-1674">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-1674">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8d30d-1675">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1675">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d30d-1676">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-1676">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8d30d-1677">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1677">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="8d30d-1678">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1678">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8d30d-1679">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1679">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="8d30d-1680">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="8d30d-1680">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="8d30d-1681">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="8d30d-1681">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="8d30d-1682">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1682">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8d30d-1683">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1683">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="8d30d-1684">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1684">Updated cmdlets:</span></span>
    - <span data-ttu-id="8d30d-1685">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1685">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="8d30d-1686">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1686">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8d30d-1687">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1687">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8d30d-1688">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="8d30d-1688">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="8d30d-1689">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1689">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="8d30d-1690">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="8d30d-1690">Event subscription expiration date,</span></span>
            - <span data-ttu-id="8d30d-1691">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1691">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="8d30d-1692">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1692">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="8d30d-1693">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="8d30d-1693">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="8d30d-1694">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1694">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="8d30d-1695">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1695">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="8d30d-1696">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8d30d-1696">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="8d30d-1697">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1697">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="8d30d-1698">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1698">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-1699">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1699">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-1700">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-1700">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="8d30d-1701">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1701">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="8d30d-1702">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-1702">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="8d30d-1703">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="8d30d-1703">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1704">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1704">Az.Network</span></span>
* <span data-ttu-id="8d30d-1705">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8d30d-1705">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="8d30d-1706">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1706">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1707">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="8d30d-1707">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="8d30d-1708">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1708">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="8d30d-1709">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1709">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1710">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8d30d-1710">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="8d30d-1711">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1711">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="8d30d-1712">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1712">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1713">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1713">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d30d-1714">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1714">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d30d-1715">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d30d-1715">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d30d-1716">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1716">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="8d30d-1717">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1717">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8d30d-1718">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d30d-1718">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="8d30d-1719">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1719">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1720">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d30d-1720">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d30d-1721">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d30d-1721">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d30d-1722">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d30d-1722">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d30d-1723">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1723">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="8d30d-1724">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1724">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="8d30d-1725">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1725">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="8d30d-1726">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1726">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="8d30d-1727">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1727">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="8d30d-1728">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1728">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="8d30d-1729">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="8d30d-1729">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="8d30d-1730">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-1730">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="8d30d-1731">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1731">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="8d30d-1732">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-1732">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="8d30d-1733">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="8d30d-1733">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="8d30d-1734">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1734">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="8d30d-1735">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1735">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="8d30d-1736">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="8d30d-1736">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="8d30d-1737">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-1737">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="8d30d-1738">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1738">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8d30d-1739">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="8d30d-1739">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="8d30d-1740">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8d30d-1740">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="8d30d-1741">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="8d30d-1741">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="8d30d-1742">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="8d30d-1742">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="8d30d-1743">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1743">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="8d30d-1744">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1744">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8d30d-1745">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1745">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8d30d-1746">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1746">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-1747">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1747">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-1748">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1748">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1749">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1749">Az.Resources</span></span>
* <span data-ttu-id="8d30d-1750">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="8d30d-1750">Support for additional Template Export options</span></span>
    - <span data-ttu-id="8d30d-1751">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1751">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8d30d-1752">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1752">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8d30d-1753">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="8d30d-1753">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-1754">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1754">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-1755">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="8d30d-1755">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1756">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1756">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1757">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1757">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="8d30d-1758">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1758">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="8d30d-1759">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1759">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="8d30d-1760">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-1760">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d30d-1761">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-1761">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d30d-1762">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d30d-1762">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d30d-1763">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8d30d-1763">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="8d30d-1764">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8d30d-1764">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1765">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1765">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1766">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-1766">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="8d30d-1767">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1767">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d30d-1768">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="8d30d-1768">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="8d30d-1769">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1769">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1770">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1770">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1771">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="8d30d-1771">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="8d30d-1772">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="8d30d-1772">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="8d30d-1773">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1773">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="8d30d-1774">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-1774">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-1775">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1775">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1776">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1776">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1777">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1777">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="8d30d-1778">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d30d-1778">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-1779">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-1779">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-1780">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1780">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="8d30d-1781">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="8d30d-1781">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1782">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1782">Az.Network</span></span>
* <span data-ttu-id="8d30d-1783">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1783">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="8d30d-1784">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="8d30d-1784">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-1785">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1785">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-1786">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="8d30d-1786">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1787">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1787">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1788">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="8d30d-1788">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d30d-1789">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d30d-1789">Az.ServiceBus</span></span>
* <span data-ttu-id="8d30d-1790">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="8d30d-1790">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-1791">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1791">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-1792">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1792">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="8d30d-1793">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1793">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1794">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1794">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1795">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1795">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="8d30d-1796">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-1796">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8d30d-1797">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="8d30d-1797">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="8d30d-1798">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1798">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1799">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1799">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1800">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1800">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="8d30d-1801">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1801">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8d30d-1802">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1802">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-1803">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1803">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="8d30d-1804">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1804">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="8d30d-1805">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1805">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="8d30d-1806">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="8d30d-1806">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="8d30d-1807">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1807">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="8d30d-1808">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="8d30d-1808">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="8d30d-1809">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1809">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="8d30d-1810">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1810">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="8d30d-1811">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1811">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="8d30d-1812">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="8d30d-1812">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="8d30d-1813">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="8d30d-1813">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="8d30d-1814">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="8d30d-1814">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="8d30d-1815">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="8d30d-1815">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="8d30d-1816">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1816">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="8d30d-1817">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1817">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="8d30d-1818">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1818">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="8d30d-1819">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1819">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="8d30d-1820">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="8d30d-1820">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="8d30d-1821">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1821">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="8d30d-1822">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="8d30d-1822">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="8d30d-1823">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="8d30d-1823">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="8d30d-1824">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1824">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="8d30d-1825">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1825">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="8d30d-1826">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-1826">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="8d30d-1827">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1827">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="8d30d-1828">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1828">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="8d30d-1829">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1829">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="8d30d-1830">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1830">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="8d30d-1831">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1831">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="8d30d-1832">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="8d30d-1832">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="8d30d-1833">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="8d30d-1833">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="8d30d-1834">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="8d30d-1834">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="8d30d-1835">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1835">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="8d30d-1836">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1836">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d30d-1837">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1837">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="8d30d-1838">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="8d30d-1838">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="8d30d-1839">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1839">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="8d30d-1840">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1840">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="8d30d-1841">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1841">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="8d30d-1842">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1842">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d30d-1843">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1843">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8d30d-1844">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1844">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8d30d-1845">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1845">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="8d30d-1846">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1846">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="8d30d-1847">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1847">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d30d-1848">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1848">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8d30d-1849">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1849">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8d30d-1850">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1850">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="8d30d-1851">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1851">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="8d30d-1852">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1852">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="8d30d-1853">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1853">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="8d30d-1854">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1854">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="8d30d-1855">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1855">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="8d30d-1856">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1856">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="8d30d-1857">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1857">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="8d30d-1858">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1858">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="8d30d-1859">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1859">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8d30d-1860">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1860">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8d30d-1861">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1861">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8d30d-1862">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1862">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8d30d-1863">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8d30d-1863">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8d30d-1864">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1864">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8d30d-1865">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1865">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8d30d-1866">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1866">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8d30d-1867">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="8d30d-1867">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="8d30d-1868">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1868">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="8d30d-1869">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="8d30d-1869">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="8d30d-1870">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1870">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="8d30d-1871">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="8d30d-1871">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="8d30d-1872">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1872">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="8d30d-1873">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="8d30d-1873">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="8d30d-1874">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1874">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="8d30d-1875">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1875">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="8d30d-1876">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-1876">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="8d30d-1877">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1877">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="8d30d-1878">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1878">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="8d30d-1879">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1879">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-1880">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1880">Az.Automation</span></span>
* <span data-ttu-id="8d30d-1881">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1881">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="8d30d-1882">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="8d30d-1882">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="8d30d-1883">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="8d30d-1883">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="8d30d-1884">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1884">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="8d30d-1885">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="8d30d-1885">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="8d30d-1886">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1886">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="8d30d-1887">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1887">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1888">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1888">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1889">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1889">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="8d30d-1890">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="8d30d-1890">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-1891">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-1891">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-1892">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-1892">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-1893">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1893">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-1894">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-1894">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1895">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1895">Az.Network</span></span>
* <span data-ttu-id="8d30d-1896">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1896">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="8d30d-1897">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1897">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d30d-1898">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-1898">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="8d30d-1899">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8d30d-1899">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-1900">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-1900">Az.Resources</span></span>
* <span data-ttu-id="8d30d-1901">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="8d30d-1901">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-1902">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-1902">Az.Sql</span></span>
* <span data-ttu-id="8d30d-1903">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="8d30d-1903">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="8d30d-1904">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1904">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-1905">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-1905">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-1906">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="8d30d-1906">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-1907">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1907">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-1908">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1908">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="8d30d-1909">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1909">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-1910">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-1910">Az.Compute</span></span>
* <span data-ttu-id="8d30d-1911">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1911">Proximity placement group feature.</span></span>
    - <span data-ttu-id="8d30d-1912">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1912">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="8d30d-1913">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-1913">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="8d30d-1914">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1914">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="8d30d-1915">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1915">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="8d30d-1916">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-1916">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="8d30d-1917">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8d30d-1917">Breaking changes</span></span>
    - <span data-ttu-id="8d30d-1918">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1918">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="8d30d-1919">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1919">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8d30d-1920">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8d30d-1920">Az.DeploymentManager</span></span>
* <span data-ttu-id="8d30d-1921">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-1921">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="8d30d-1922">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8d30d-1922">Az.Dns</span></span>
* <span data-ttu-id="8d30d-1923">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="8d30d-1923">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="8d30d-1924">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1924">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="8d30d-1925">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1925">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-1926">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1926">Az.FrontDoor</span></span>
* <span data-ttu-id="8d30d-1927">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="8d30d-1927">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="8d30d-1928">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1928">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-1929">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-1929">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-1930">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1930">Removed two cmdlets:</span></span>
    - <span data-ttu-id="8d30d-1931">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d30d-1931">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="8d30d-1932">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d30d-1932">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8d30d-1933">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d30d-1933">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8d30d-1934">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="8d30d-1934">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="8d30d-1935">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1935">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="8d30d-1936">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1936">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-1937">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-1937">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-1938">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1938">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="8d30d-1939">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="8d30d-1939">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="8d30d-1940">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-1940">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="8d30d-1941">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="8d30d-1941">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="8d30d-1942">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1942">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="8d30d-1943">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="8d30d-1943">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="8d30d-1944">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="8d30d-1944">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="8d30d-1945">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1945">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d30d-1946">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1946">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d30d-1947">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1947">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d30d-1948">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1948">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d30d-1949">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-1949">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d30d-1950">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="8d30d-1950">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="8d30d-1951">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="8d30d-1951">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-1952">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1952">Az.Network</span></span>
* <span data-ttu-id="8d30d-1953">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="8d30d-1953">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="8d30d-1954">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-1954">New cmdlets</span></span>
        - <span data-ttu-id="8d30d-1955">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1955">New-AzNatGateway</span></span>
        - <span data-ttu-id="8d30d-1956">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1956">Get-AzNatGateway</span></span>
        - <span data-ttu-id="8d30d-1957">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1957">Set-AzNatGateway</span></span>
        - <span data-ttu-id="8d30d-1958">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-1958">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="8d30d-1959">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="8d30d-1959">Updated cmdlets</span></span>
        - <span data-ttu-id="8d30d-1960">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8d30d-1960">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="8d30d-1961">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8d30d-1961">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="8d30d-1962">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1962">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="8d30d-1963">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1963">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="8d30d-1964">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1964">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-1965">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-1965">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-1966">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1966">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="8d30d-1967">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1967">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="8d30d-1968">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="8d30d-1968">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-1969">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-1969">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-1970">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1970">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="8d30d-1971">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1971">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="8d30d-1972">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1972">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="8d30d-1973">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1973">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="8d30d-1974">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1974">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="8d30d-1975">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1975">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="8d30d-1976">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8d30d-1976">Az.Relay</span></span>
* <span data-ttu-id="8d30d-1977">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="8d30d-1977">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d30d-1978">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d30d-1978">Az.ServiceBus</span></span>
* <span data-ttu-id="8d30d-1979">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="8d30d-1979">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-1980">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-1980">Az.Storage</span></span>
* <span data-ttu-id="8d30d-1981">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="8d30d-1981">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="8d30d-1982">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="8d30d-1982">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="8d30d-1983">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="8d30d-1983">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="8d30d-1984">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1984">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d30d-1985">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="8d30d-1985">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="8d30d-1986">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1986">New-AzStorageAccount</span></span>
    - <span data-ttu-id="8d30d-1987">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1987">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="8d30d-1988">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-1988">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-1989">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-1989">Az.Websites</span></span>
* <span data-ttu-id="8d30d-1990">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-1990">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="8d30d-1991">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="8d30d-1991">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="8d30d-1992">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-1992">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d30d-1993">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8d30d-1993">Highlights since the last major release</span></span>
* <span data-ttu-id="8d30d-1994">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="8d30d-1994">General availability of `Az` module</span></span>
* <span data-ttu-id="8d30d-1995">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d30d-1995">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d30d-1996">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d30d-1996">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d30d-1997">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-1997">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d30d-1998">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8d30d-1998">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d30d-1999">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-1999">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d30d-2000">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="8d30d-2000">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2001">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2001">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2002">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="8d30d-2002">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d30d-2003">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-2003">Az.Batch</span></span>
* <span data-ttu-id="8d30d-2004">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2004">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-2005">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-2005">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-2006">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2006">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-2007">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2007">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-2008">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2008">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2009">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2009">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2010">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="8d30d-2010">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="8d30d-2011">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2011">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d30d-2012">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8d30d-2012">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-2013">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-2013">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-2014">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2014">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2015">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2015">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-2016">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2016">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d30d-2017">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d30d-2017">Az.EventGrid</span></span>
* <span data-ttu-id="8d30d-2018">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2018">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-2019">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2019">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-2020">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="8d30d-2020">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8d30d-2021">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d30d-2021">Az.HDInsight</span></span>
* <span data-ttu-id="8d30d-2022">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2022">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-2023">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2023">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-2024">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2024">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-2025">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-2025">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-2026">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2026">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d30d-2027">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8d30d-2027">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8d30d-2028">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d30d-2028">Az.MachineLearning</span></span>
* <span data-ttu-id="8d30d-2029">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2029">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="8d30d-2030">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8d30d-2030">Az.Media</span></span>
* <span data-ttu-id="8d30d-2031">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2031">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-2032">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-2032">Az.Monitor</span></span>
  * <span data-ttu-id="8d30d-2033">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="8d30d-2033">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="8d30d-2034">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="8d30d-2034">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="8d30d-2035">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="8d30d-2035">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="8d30d-2036">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d30d-2036">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8d30d-2037">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d30d-2037">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8d30d-2038">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d30d-2038">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="8d30d-2039">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="8d30d-2039">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2040">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2040">Az.Network</span></span>
* <span data-ttu-id="8d30d-2041">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2041">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d30d-2042">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8d30d-2042">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="8d30d-2043">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8d30d-2043">Az.NotificationHubs</span></span>
* <span data-ttu-id="8d30d-2044">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2044">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-2045">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-2045">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-2046">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2046">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8d30d-2047">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8d30d-2047">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8d30d-2048">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2048">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2049">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2049">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-2050">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2050">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d30d-2051">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2051">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="8d30d-2052">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="8d30d-2052">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="8d30d-2053">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="8d30d-2053">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d30d-2054">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d30d-2054">Az.RedisCache</span></span>
* <span data-ttu-id="8d30d-2055">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2055">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2056">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2056">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2057">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8d30d-2057">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2058">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2058">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2059">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="8d30d-2059">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="8d30d-2060">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2060">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d30d-2061">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2061">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="8d30d-2062">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2062">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="8d30d-2063">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2063">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="8d30d-2064">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2064">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="8d30d-2065">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8d30d-2065">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-2066">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2066">Az.Websites</span></span>
* <span data-ttu-id="8d30d-2067">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="8d30d-2067">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="8d30d-2068">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2068">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d30d-2069">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2069">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="8d30d-2070">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2070">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="8d30d-2071">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2071">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d30d-2072">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8d30d-2072">Highlights since the last major release</span></span>
* <span data-ttu-id="8d30d-2073">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="8d30d-2073">General availability of `Az` module</span></span>
* <span data-ttu-id="8d30d-2074">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d30d-2074">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d30d-2075">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d30d-2075">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d30d-2076">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2076">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d30d-2077">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8d30d-2077">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d30d-2078">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2078">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d30d-2079">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="8d30d-2079">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2080">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2080">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2081">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="8d30d-2081">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d30d-2082">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2082">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d30d-2083">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="8d30d-2083">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="8d30d-2084">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="8d30d-2084">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-2085">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2085">Az.Automation</span></span>
* <span data-ttu-id="8d30d-2086">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2086">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="8d30d-2087">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2087">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="8d30d-2088">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2088">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2089">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2089">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2090">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-2090">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8d30d-2091">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2091">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="8d30d-2092">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2092">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d30d-2093">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="8d30d-2093">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-2094">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-2094">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-2095">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="8d30d-2095">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="8d30d-2096">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2096">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2097">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2097">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2098">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2098">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="8d30d-2099">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2099">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8d30d-2100">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="8d30d-2100">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="8d30d-2101">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8d30d-2101">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="8d30d-2102">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="8d30d-2102">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="8d30d-2103">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8d30d-2103">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2104">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2104">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2105">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2105">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-2106">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2106">Az.Storage</span></span>
* <span data-ttu-id="8d30d-2107">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2107">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="8d30d-2108">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8d30d-2108">New-AzStorageContext</span></span>
* <span data-ttu-id="8d30d-2109">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="8d30d-2109">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="8d30d-2110">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8d30d-2110">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8d30d-2111">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8d30d-2111">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8d30d-2112">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2112">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8d30d-2113">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2113">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="8d30d-2114">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d30d-2114">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="8d30d-2115">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-2115">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8d30d-2116">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-2116">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8d30d-2117">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-2117">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="8d30d-2118">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d30d-2118">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="8d30d-2119">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2119">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d30d-2120">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8d30d-2120">Highlights since the last major release</span></span>
* <span data-ttu-id="8d30d-2121">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="8d30d-2121">General availability of `Az` module</span></span>
* <span data-ttu-id="8d30d-2122">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d30d-2122">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d30d-2123">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d30d-2123">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d30d-2124">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2124">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d30d-2125">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8d30d-2125">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d30d-2126">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2126">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d30d-2127">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="8d30d-2127">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-2128">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2128">Az.Automation</span></span>
* <span data-ttu-id="8d30d-2129">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="8d30d-2129">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="8d30d-2130">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="8d30d-2130">Dynamic grouping</span></span>
    * <span data-ttu-id="8d30d-2131">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-2131">Pre-Post script</span></span>
    * <span data-ttu-id="8d30d-2132">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="8d30d-2132">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2133">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2133">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2134">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="8d30d-2134">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="8d30d-2135">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2135">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-2136">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-2136">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-2137">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-2137">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2138">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2138">Az.Network</span></span>
* <span data-ttu-id="8d30d-2139">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-2139">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="8d30d-2140">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-2140">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2141">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2141">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-2142">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="8d30d-2142">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="8d30d-2143">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="8d30d-2143">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2144">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2144">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2145">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-2145">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="8d30d-2146">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="8d30d-2146">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2147">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2147">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2148">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2148">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-2149">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2149">Az.Storage</span></span>
* <span data-ttu-id="8d30d-2150">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8d30d-2150">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="8d30d-2151">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2151">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d30d-2152">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2152">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d30d-2153">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2153">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d30d-2154">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="8d30d-2154">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="8d30d-2155">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="8d30d-2155">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="8d30d-2156">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-2156">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-2157">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2157">Az.Websites</span></span>
* <span data-ttu-id="8d30d-2158">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2158">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="8d30d-2159">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2159">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2160">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2160">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2161">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="8d30d-2161">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="8d30d-2162">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-2162">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-2163">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2163">Az.Automation</span></span>
* <span data-ttu-id="8d30d-2164">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2164">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="8d30d-2165">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2165">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="8d30d-2166">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="8d30d-2166">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-2167">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-2167">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-2168">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2168">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2169">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2169">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2170">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="8d30d-2170">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-2171">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-2171">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-2172">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="8d30d-2172">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d30d-2173">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-2173">Az.LogicApp</span></span>
* <span data-ttu-id="8d30d-2174">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="8d30d-2174">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2175">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2175">Az.Network</span></span>
* <span data-ttu-id="8d30d-2176">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2176">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2177">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2177">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-2178">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2178">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="8d30d-2179">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="8d30d-2179">SDK Update</span></span>
* <span data-ttu-id="8d30d-2180">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8d30d-2180">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="8d30d-2181">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8d30d-2181">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2182">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2182">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2183">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="8d30d-2183">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="8d30d-2184">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="8d30d-2184">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="8d30d-2185">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="8d30d-2185">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="8d30d-2186">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="8d30d-2186">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="8d30d-2187">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="8d30d-2187">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="8d30d-2188">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="8d30d-2188">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2189">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2189">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2190">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2190">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="8d30d-2191">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2191">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-2192">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2192">Az.Storage</span></span>
* <span data-ttu-id="8d30d-2193">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-2193">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="8d30d-2194">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2194">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="8d30d-2195">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2195">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d30d-2196">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="8d30d-2196">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-2197">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2197">Az.Automation</span></span>
* <span data-ttu-id="8d30d-2198">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2198">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="8d30d-2199">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2199">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="8d30d-2200">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2200">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-2201">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2201">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-2202">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2202">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2203">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2203">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2204">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="8d30d-2204">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="8d30d-2205">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="8d30d-2205">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="8d30d-2206">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2206">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="8d30d-2207">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2207">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2208">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2208">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-2209">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="8d30d-2209">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d30d-2210">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2210">Az.EventHub</span></span>
* <span data-ttu-id="8d30d-2211">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2211">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-2212">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-2212">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-2213">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="8d30d-2213">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d30d-2214">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-2214">Az.LogicApp</span></span>
* <span data-ttu-id="8d30d-2215">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="8d30d-2215">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="8d30d-2216">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2216">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="8d30d-2217">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="8d30d-2217">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="8d30d-2218">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d30d-2218">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d30d-2219">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d30d-2219">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d30d-2220">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d30d-2220">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d30d-2221">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d30d-2221">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="8d30d-2222">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="8d30d-2222">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="8d30d-2223">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2223">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d30d-2224">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2224">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d30d-2225">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2225">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d30d-2226">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2226">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="8d30d-2227">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-2227">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d30d-2228">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-2228">Az.Monitor</span></span>
* <span data-ttu-id="8d30d-2229">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="8d30d-2229">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2230">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2230">Az.Network</span></span>
* <span data-ttu-id="8d30d-2231">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="8d30d-2231">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-2232">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-2232">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d30d-2233">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2233">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="8d30d-2234">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2234">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="8d30d-2235">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2235">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2236">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2236">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2237">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8d30d-2237">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8d30d-2238">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8d30d-2238">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="8d30d-2239">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="8d30d-2239">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="8d30d-2240">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="8d30d-2240">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2241">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2241">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2242">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="8d30d-2242">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="8d30d-2243">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="8d30d-2243">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-2244">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2244">Az.Websites</span></span>
* <span data-ttu-id="8d30d-2245">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="8d30d-2245">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="8d30d-2246">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2246">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2247">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2247">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2248">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8d30d-2248">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d30d-2249">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2249">Az.AnalysisServices</span></span>
<span data-ttu-id="8d30d-2250">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2250">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2251">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2251">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2252">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="8d30d-2252">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="8d30d-2253">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="8d30d-2253">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="8d30d-2254">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2254">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2255">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2255">Az.RecoveryServices</span></span>
<span data-ttu-id="8d30d-2256">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2256">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2257">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2257">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2258">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="8d30d-2258">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="8d30d-2259">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8d30d-2259">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8d30d-2260">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="8d30d-2260">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="8d30d-2261">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8d30d-2261">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2262">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2262">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2263">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2263">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="8d30d-2264">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="8d30d-2264">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="8d30d-2265">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="8d30d-2265">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="8d30d-2266">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2266">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2267">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2267">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2268">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="8d30d-2268">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d30d-2269">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2269">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d30d-2270">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="8d30d-2270">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2271">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2271">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d30d-2272">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="8d30d-2272">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="8d30d-2273">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2273">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2274">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2274">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2275">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8d30d-2275">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d30d-2276">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2276">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d30d-2277">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="8d30d-2277">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="8d30d-2278">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8d30d-2278">Az.Aks</span></span>
* <span data-ttu-id="8d30d-2279">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2279">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d30d-2280">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2280">Az.Automation</span></span>
* <span data-ttu-id="8d30d-2281">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="8d30d-2281">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="8d30d-2282">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2282">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d30d-2283">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d30d-2283">Az.Cdn</span></span>
* <span data-ttu-id="8d30d-2284">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2284">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2285">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2285">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2286">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2286">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="8d30d-2287">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8d30d-2287">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="8d30d-2288">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d30d-2288">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8d30d-2289">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8d30d-2289">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8d30d-2290">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2290">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d30d-2291">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d30d-2291">Az.DataFactory</span></span>
* <span data-ttu-id="8d30d-2292">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="8d30d-2292">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2293">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2293">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-2294">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="8d30d-2294">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="8d30d-2295">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="8d30d-2295">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="8d30d-2296">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2296">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-2297">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2297">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-2298">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2298">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d30d-2299">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-2299">Az.KeyVault</span></span>
* <span data-ttu-id="8d30d-2300">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2300">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2301">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2301">Az.Network</span></span>
* <span data-ttu-id="8d30d-2302">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2302">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2303">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2303">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2304">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2304">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="8d30d-2305">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2305">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="8d30d-2306">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="8d30d-2306">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="8d30d-2307">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="8d30d-2307">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="8d30d-2308">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="8d30d-2308">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="8d30d-2309">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2309">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="8d30d-2310">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="8d30d-2310">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-2311">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-2311">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-2312">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="8d30d-2312">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="8d30d-2313">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2313">Fix some error messages.</span></span>
* <span data-ttu-id="8d30d-2314">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2314">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="8d30d-2315">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2315">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d30d-2316">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d30d-2316">Az.SignalR</span></span>
* <span data-ttu-id="8d30d-2317">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2317">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2318">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2318">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2319">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2319">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d30d-2320">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="8d30d-2320">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="8d30d-2321">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="8d30d-2321">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="8d30d-2322">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="8d30d-2322">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-2323">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2323">Az.Storage</span></span>
* <span data-ttu-id="8d30d-2324">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2324">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d30d-2325">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2325">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="8d30d-2326">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="8d30d-2326">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="8d30d-2327">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="8d30d-2327">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8d30d-2328">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8d30d-2328">Az.TrafficManager</span></span>
* <span data-ttu-id="8d30d-2329">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2329">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-2330">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2330">Az.Websites</span></span>
* <span data-ttu-id="8d30d-2331">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2331">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d30d-2332">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2332">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="8d30d-2333">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-2333">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="8d30d-2334">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8d30d-2334">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d30d-2335">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2335">Az.Accounts</span></span>
* <span data-ttu-id="8d30d-2336">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="8d30d-2336">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2337">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2337">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2338">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2338">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="8d30d-2339">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="8d30d-2339">Updated the description of ID in help files</span></span>
* <span data-ttu-id="8d30d-2340">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2340">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2341">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2341">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-2342">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2342">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="8d30d-2343">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="8d30d-2343">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d30d-2344">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d30d-2344">Az.EventGrid</span></span>
* <span data-ttu-id="8d30d-2345">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2345">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="8d30d-2346">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="8d30d-2346">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="8d30d-2347">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="8d30d-2347">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8d30d-2348">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="8d30d-2348">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8d30d-2349">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="8d30d-2349">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8d30d-2350">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2350">Dead letter endpoint.</span></span>
    - <span data-ttu-id="8d30d-2351">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="8d30d-2351">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8d30d-2352">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="8d30d-2352">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8d30d-2353">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="8d30d-2353">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8d30d-2354">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2354">Dead letter endpoint.</span></span>
* <span data-ttu-id="8d30d-2355">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2355">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="8d30d-2356">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2356">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d30d-2357">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2357">Az.IotHub</span></span>
* <span data-ttu-id="8d30d-2358">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="8d30d-2358">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d30d-2359">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d30d-2359">Az.LogicApp</span></span>
* <span data-ttu-id="8d30d-2360">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="8d30d-2360">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2361">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2361">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2362">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2362">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="8d30d-2363">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="8d30d-2363">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="8d30d-2364">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="8d30d-2364">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8d30d-2365">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="8d30d-2365">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="8d30d-2366">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2366">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="8d30d-2367">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="8d30d-2367">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d30d-2368">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d30d-2368">Az.SignalR</span></span>
* <span data-ttu-id="8d30d-2369">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2369">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2370">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2370">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2371">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2371">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d30d-2372">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2372">Az.Storage</span></span>
* <span data-ttu-id="8d30d-2373">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="8d30d-2373">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="8d30d-2374">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8d30d-2374">New-AzStorageContext</span></span>
* <span data-ttu-id="8d30d-2375">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="8d30d-2375">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="8d30d-2376">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8d30d-2376">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-2377">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2377">Az.Websites</span></span>
* <span data-ttu-id="8d30d-2378">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2378">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8d30d-2379">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2379">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="8d30d-2380">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2380">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="8d30d-2381">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-2381">General</span></span>

- <span data-ttu-id="8d30d-2382">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="8d30d-2382">General Availability of Az Module</span></span>
- <span data-ttu-id="8d30d-2383">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="8d30d-2383">Online help for each module</span></span>
- <span data-ttu-id="8d30d-2384">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="8d30d-2384">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="8d30d-2385">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="8d30d-2385">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="8d30d-2386">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2386">Az.Accounts</span></span>
- <span data-ttu-id="8d30d-2387">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2387">Changed from Az.Profile</span></span>
- <span data-ttu-id="8d30d-2388">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="8d30d-2388">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8d30d-2389">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-2389">Az.ApiManagement</span></span>
- <span data-ttu-id="8d30d-2390">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="8d30d-2390">Fixes for #7002</span></span>
- <span data-ttu-id="8d30d-2391">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2391">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="8d30d-2392">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d30d-2392">Az.Batch</span></span>
- <span data-ttu-id="8d30d-2393">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2393">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="8d30d-2394">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2394">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="8d30d-2395">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2395">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="8d30d-2396">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8d30d-2396">Az.Billing</span></span>
- <span data-ttu-id="8d30d-2397">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2397">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="8d30d-2398">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2398">Az.CognitivServices</span></span>
- <span data-ttu-id="8d30d-2399">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-2399">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="8d30d-2400">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="8d30d-2400">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8d30d-2401">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2401">Az.ContainerInstance</span></span>
- <span data-ttu-id="8d30d-2402">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="8d30d-2402">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="8d30d-2403">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8d30d-2403">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="8d30d-2404">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2404">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2405">Az.DataLakeStore</span></span>
- <span data-ttu-id="8d30d-2406">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2406">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="8d30d-2407">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d30d-2407">Az.Monitor</span></span>
- <span data-ttu-id="8d30d-2408">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2408">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="8d30d-2409">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d30d-2409">Az.KeyVault</span></span>
- <span data-ttu-id="8d30d-2410">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="8d30d-2410">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="8d30d-2411">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d30d-2411">Az.MachineLearning</span></span>
- <span data-ttu-id="8d30d-2412">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2412">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="8d30d-2413">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8d30d-2413">Az.Media</span></span>
- <span data-ttu-id="8d30d-2414">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="8d30d-2414">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8d30d-2415">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2415">Az.Network</span></span>
<span data-ttu-id="8d30d-2416">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8d30d-2416">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="8d30d-2417">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d30d-2417">New cmdlets added:</span></span>
        - <span data-ttu-id="8d30d-2418">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2418">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d30d-2419">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2419">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d30d-2420">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2420">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d30d-2421">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2421">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d30d-2422">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2422">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d30d-2423">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-2423">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="8d30d-2424">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2424">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="8d30d-2425">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d30d-2425">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="8d30d-2426">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2426">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="8d30d-2427">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="8d30d-2427">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="8d30d-2428">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-2428">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8d30d-2429">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8d30d-2429">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8d30d-2430">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-2430">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="8d30d-2431">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-2431">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="8d30d-2432">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2432">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="8d30d-2433">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="8d30d-2433">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="8d30d-2434">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d30d-2434">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8d30d-2435">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d30d-2435">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8d30d-2436">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d30d-2436">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="8d30d-2437">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="8d30d-2437">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="8d30d-2438">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2438">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="8d30d-2439">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-2439">Az.OperationalInsights</span></span>
- <span data-ttu-id="8d30d-2440">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2440">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="8d30d-2441">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2441">Az.Profile</span></span>
- <span data-ttu-id="8d30d-2442">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d30d-2442">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2443">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2443">Az.RecoveryServices</span></span>
- <span data-ttu-id="8d30d-2444">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2444">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="8d30d-2445">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2445">Az.Resources</span></span>
- <span data-ttu-id="8d30d-2446">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2446">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8d30d-2447">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-2447">Az.ServiceFabric</span></span>
- <span data-ttu-id="8d30d-2448">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="8d30d-2448">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="8d30d-2449">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2449">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="8d30d-2450">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="8d30d-2450">Az.SIgnalR</span></span>
- <span data-ttu-id="8d30d-2451">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="8d30d-2451">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="8d30d-2452">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2452">Az.Sql</span></span>
- <span data-ttu-id="8d30d-2453">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="8d30d-2453">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="8d30d-2454">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="8d30d-2454">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="8d30d-2455">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2455">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="8d30d-2456">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2456">Az.Storage</span></span>
- <span data-ttu-id="8d30d-2457">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2457">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8d30d-2458">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2458">Az.Websites</span></span>
- <span data-ttu-id="8d30d-2459">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8d30d-2459">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="8d30d-2460">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2460">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="8d30d-2461">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-2461">General</span></span>

* <span data-ttu-id="8d30d-2462">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8d30d-2462">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="8d30d-2463">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2463">Az.Compute</span></span>

* <span data-ttu-id="8d30d-2464">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2464">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2465">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2465">Az.DataLakeStore</span></span>

* <span data-ttu-id="8d30d-2466">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="8d30d-2466">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="8d30d-2467">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d30d-2467">Az.FrontDoor</span></span>

* <span data-ttu-id="8d30d-2468">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="8d30d-2468">Fixed some broken links</span></span>
    - <span data-ttu-id="8d30d-2469">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2469">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="8d30d-2470">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2470">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8d30d-2471">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2471">Az.RecoveryServices</span></span>

* <span data-ttu-id="8d30d-2472">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2472">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="8d30d-2473">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2473">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="8d30d-2474">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2474">Az.Resources</span></span>

* <span data-ttu-id="8d30d-2475">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="8d30d-2475">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="8d30d-2476">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2476">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="8d30d-2477">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2477">Az.Sql</span></span>

* <span data-ttu-id="8d30d-2478">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8d30d-2478">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="8d30d-2479">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="8d30d-2479">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="8d30d-2480">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2480">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="8d30d-2481">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2481">Az.Storage</span></span>

* <span data-ttu-id="8d30d-2482">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d30d-2482">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="8d30d-2483">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="8d30d-2483">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="8d30d-2484">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2484">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8d30d-2485">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="8d30d-2485">Support Static Website configuration</span></span>
    - <span data-ttu-id="8d30d-2486">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d30d-2486">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="8d30d-2487">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d30d-2487">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8d30d-2488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2488">Az.Websites</span></span>

* <span data-ttu-id="8d30d-2489">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8d30d-2489">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="8d30d-2490">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2490">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="8d30d-2491">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2491">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="8d30d-2492">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2492">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8d30d-2493">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d30d-2493">Az.ApiManagement</span></span>
* <span data-ttu-id="8d30d-2494">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2494">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="8d30d-2495">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d30d-2495">Az.Automation</span></span>
* <span data-ttu-id="8d30d-2496">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="8d30d-2496">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="8d30d-2497">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="8d30d-2497">Added Update Management cmdlets</span></span>
* <span data-ttu-id="8d30d-2498">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="8d30d-2498">Added Source Control cmdlets</span></span>
* <span data-ttu-id="8d30d-2499">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="8d30d-2499">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="8d30d-2500">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="8d30d-2500">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="8d30d-2501">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2501">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2502">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="8d30d-2502">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="8d30d-2503">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2503">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8d30d-2504">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2504">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d30d-2505">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2505">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="8d30d-2506">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8d30d-2506">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8d30d-2507">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="8d30d-2507">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8d30d-2508">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2508">Az.Network</span></span>
* <span data-ttu-id="8d30d-2509">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="8d30d-2509">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="8d30d-2510">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="8d30d-2510">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="8d30d-2511">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2511">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="8d30d-2512">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="8d30d-2512">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="8d30d-2513">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8d30d-2513">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8d30d-2514">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2514">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="8d30d-2515">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2515">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="8d30d-2516">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8d30d-2516">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8d30d-2517">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8d30d-2517">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="8d30d-2518">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8d30d-2518">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="8d30d-2519">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8d30d-2519">Az.Relay</span></span>
* <span data-ttu-id="8d30d-2520">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2520">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="8d30d-2521">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2521">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2522">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="8d30d-2522">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="8d30d-2523">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="8d30d-2523">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="8d30d-2524">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="8d30d-2524">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8d30d-2525">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-2525">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-2526">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8d30d-2526">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="8d30d-2527">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2527">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2528">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2528">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="8d30d-2529">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2529">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d30d-2530">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2530">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d30d-2531">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2531">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d30d-2532">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d30d-2532">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d30d-2533">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d30d-2533">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d30d-2534">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d30d-2534">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d30d-2535">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d30d-2535">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d30d-2536">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d30d-2536">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="8d30d-2537">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2537">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="8d30d-2538">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2538">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="8d30d-2539">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2539">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="8d30d-2540">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2540">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8d30d-2541">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2541">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8d30d-2542">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2542">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="8d30d-2543">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2543">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="8d30d-2544">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="8d30d-2544">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="8d30d-2545">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2545">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="8d30d-2546">Geral</span><span class="sxs-lookup"><span data-stu-id="8d30d-2546">General</span></span>
* <span data-ttu-id="8d30d-2547">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="8d30d-2547">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="8d30d-2548">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2548">Az.Profile</span></span>
* <span data-ttu-id="8d30d-2549">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8d30d-2549">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="8d30d-2550">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="8d30d-2550">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="8d30d-2551">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="8d30d-2551">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="8d30d-2552">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="8d30d-2552">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="8d30d-2553">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="8d30d-2553">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="8d30d-2554">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="8d30d-2554">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="8d30d-2555">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="8d30d-2555">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-2556">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2556">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-2557">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2557">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2558">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2558">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2559">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="8d30d-2559">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="8d30d-2560">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="8d30d-2560">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="8d30d-2561">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2561">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2562">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2562">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-2563">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2563">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="8d30d-2564">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2564">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="8d30d-2565">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="8d30d-2565">Az.Insights</span></span>
* <span data-ttu-id="8d30d-2566">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="8d30d-2566">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="8d30d-2567">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="8d30d-2567">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="8d30d-2568">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="8d30d-2568">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="8d30d-2569">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="8d30d-2569">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2570">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2570">Az.Network</span></span>
* <span data-ttu-id="8d30d-2571">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="8d30d-2571">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="8d30d-2572">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-2572">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="8d30d-2573">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-2573">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="8d30d-2574">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8d30d-2574">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="8d30d-2575">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-2575">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="8d30d-2576">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d30d-2576">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="8d30d-2577">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8d30d-2577">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d30d-2578">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d30d-2578">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d30d-2579">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="8d30d-2579">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2580">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2580">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2581">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="8d30d-2581">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="8d30d-2582">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2582">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d30d-2583">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d30d-2583">Az.ServiceBus</span></span>
* <span data-ttu-id="8d30d-2584">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2584">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d30d-2585">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d30d-2585">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d30d-2586">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2586">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="8d30d-2587">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2587">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="8d30d-2588">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="8d30d-2588">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="8d30d-2589">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="8d30d-2589">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="8d30d-2590">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2590">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="8d30d-2591">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2591">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="8d30d-2592">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2592">Az.Profile</span></span>
* <span data-ttu-id="8d30d-2593">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="8d30d-2593">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="8d30d-2594">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8d30d-2594">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2595">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2595">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2596">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="8d30d-2596">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="8d30d-2597">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2597">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d30d-2598">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d30d-2598">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d30d-2599">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8d30d-2599">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="8d30d-2600">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2600">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="8d30d-2601">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2601">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8d30d-2602">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2602">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8d30d-2603">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2603">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2604">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2604">Az.Network</span></span>
* <span data-ttu-id="8d30d-2605">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2605">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="8d30d-2606">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2606">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2607">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2607">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2608">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2608">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="8d30d-2609">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="8d30d-2609">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="8d30d-2610">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2610">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="8d30d-2611">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2611">Azure.Storage</span></span>
* <span data-ttu-id="8d30d-2612">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="8d30d-2612">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="8d30d-2613">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2613">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="8d30d-2614">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8d30d-2614">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8d30d-2615">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2615">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="8d30d-2616">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="8d30d-2616">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d30d-2617">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d30d-2617">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d30d-2618">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2618">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d30d-2619">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d30d-2619">Az.Compute</span></span>
* <span data-ttu-id="8d30d-2620">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="8d30d-2620">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="8d30d-2621">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2621">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="8d30d-2622">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="8d30d-2622">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="8d30d-2623">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8d30d-2623">Az.DataFactoryV2</span></span>
* <span data-ttu-id="8d30d-2624">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2624">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d30d-2625">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d30d-2625">Az.Network</span></span>
* <span data-ttu-id="8d30d-2626">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2626">Added NetworkProfile functionality.</span></span> <span data-ttu-id="8d30d-2627">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="8d30d-2627">new cmdlets added</span></span>
    - <span data-ttu-id="8d30d-2628">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2628">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d30d-2629">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2629">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d30d-2630">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2630">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d30d-2631">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d30d-2631">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d30d-2632">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-2632">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="8d30d-2633">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-2633">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="8d30d-2634">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="8d30d-2634">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="8d30d-2635">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="8d30d-2635">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="8d30d-2636">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="8d30d-2636">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d30d-2637">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d30d-2637">Az.RedisCache</span></span>
* <span data-ttu-id="8d30d-2638">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="8d30d-2638">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="8d30d-2639">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="8d30d-2639">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d30d-2640">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d30d-2640">Az.Resources</span></span>
* <span data-ttu-id="8d30d-2641">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="8d30d-2641">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8d30d-2642">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="8d30d-2642">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d30d-2643">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d30d-2643">Az.Sql</span></span>
* <span data-ttu-id="8d30d-2644">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="8d30d-2644">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d30d-2645">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d30d-2645">Az.Websites</span></span>
* <span data-ttu-id="8d30d-2646">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="8d30d-2646">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="8d30d-2647">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="8d30d-2647">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="8d30d-2648">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8d30d-2648">0.2.0 - September 2018</span></span>
 <span data-ttu-id="8d30d-2649">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="8d30d-2649">Initial Release</span></span>
