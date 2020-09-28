---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 98bae70dbd61c74aa92e69cb67afc89ebae23f70
ms.sourcegitcommit: 15f21c40dcb7610e2fbaaabf264ad925e4224500
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90928614"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="a76a3-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a76a3-103">Azure PowerShell release notes</span></span>

## <a name="470---september-2020"></a><span data-ttu-id="a76a3-104">4.7.0 - Setembro de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-104">4.7.0 - September 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-105">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-106">Foram formatadas as mensagens das futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-106">Formatted the upcoming breaking change messages</span></span>
* <span data-ttu-id="a76a3-107">Atualização do Azure.Core para 1.4.1</span><span class="sxs-lookup"><span data-stu-id="a76a3-107">Updated Azure.Core to 1.4.1</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-108">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-108">Az.Aks</span></span>
* <span data-ttu-id="a76a3-109">Foi adicionada lógica de validação de parâmetros do lado do cliente para "New-AzAksCluster", "Set-AzAksCluster" e "New-AzAksNodePool".</span><span class="sxs-lookup"><span data-stu-id="a76a3-109">Added client side parameter validation logic for 'New-AzAksCluster', 'Set-AzAksCluster' and 'New-AzAksNodePool'.</span></span> <span data-ttu-id="a76a3-110">[#12372]</span><span class="sxs-lookup"><span data-stu-id="a76a3-110">[#12372]</span></span>
* <span data-ttu-id="a76a3-111">Foi adicionado suporte para suplementos em "New-AzAksCluster".</span><span class="sxs-lookup"><span data-stu-id="a76a3-111">Added support for add-ons in 'New-AzAksCluster'.</span></span> <span data-ttu-id="a76a3-112">[#11239]</span><span class="sxs-lookup"><span data-stu-id="a76a3-112">[#11239]</span></span>
* <span data-ttu-id="a76a3-113">Foram adicionados os cmdlets "Enable-AzAksAddOn" e "Disable-AzAksAddOn" para suplementos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-113">Added cmdlets 'Enable-AzAksAddOn' and 'Disable-AzAksAddOn' for add-ons.</span></span> <span data-ttu-id="a76a3-114">[#11239]</span><span class="sxs-lookup"><span data-stu-id="a76a3-114">[#11239]</span></span>
* <span data-ttu-id="a76a3-115">Foi adicionado o parâmetro "GenerateSshKey" para "New-AzAksCluster".</span><span class="sxs-lookup"><span data-stu-id="a76a3-115">Added parameter 'GenerateSshKey' for 'New-AzAksCluster'.</span></span> <span data-ttu-id="a76a3-116">[#12371]</span><span class="sxs-lookup"><span data-stu-id="a76a3-116">[#12371]</span></span>
* <span data-ttu-id="a76a3-117">A versão da API foi atualizada para a 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-117">Updated api version to 2020-06-01.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-118">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-118">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-119">Foram apresentados termos legais adicionais para determinadas APIs.</span><span class="sxs-lookup"><span data-stu-id="a76a3-119">Showed additional legal terms for certain APIs.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-120">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-120">Az.Compute</span></span>
* <span data-ttu-id="a76a3-121">Foi adicionado o parâmetro opcional "-EncryptionType" a "New-AzVmDiskEncryptionSetConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-121">Added the '-EncryptionType' optional parameter to 'New-AzVmDiskEncryptionSetConfig'</span></span>
* <span data-ttu-id="a76a3-122">Novos cmdlets para o novo tipo de recurso: DiskAccess "Get-AzDiskAccess", "New-AzDiskAccess", "Get-AzDiskAccess"</span><span class="sxs-lookup"><span data-stu-id="a76a3-122">New cmdlets for new resource type: DiskAccess 'Get-AzDiskAccess', 'New-AzDiskAccess', 'Get-AzDiskAccess'</span></span>
* <span data-ttu-id="a76a3-123">Foram adicionados os parâmetros opcionais "-DiskAccessId" e "-NetworkAccessPolicy" a "New-AzSnapshotConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-123">Added optional parameters '-DiskAccessId' and '-NetworkAccessPolicy' to 'New-AzSnapshotConfig'</span></span>
* <span data-ttu-id="a76a3-124">Foram adicionados os parâmetros opcionais "-DiskAccessId" e "-NetworkAccessPolicy" a "New-AzDiskConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-124">Added optional parameters '-DiskAccessId' and '-NetworkAccessPolicy' to 'New-AzDiskConfig'</span></span>
* <span data-ttu-id="a76a3-125">Foi adicionada a propriedade "PatchStatus" à Vista de Instância de VirtualMachine</span><span class="sxs-lookup"><span data-stu-id="a76a3-125">Added 'PatchStatus' property to VirtualMachine Instance View</span></span>
* <span data-ttu-id="a76a3-126">Foi adicionada a propriedade "VMHealth" à vista de instância da máquina virtual, que é o objeto devolvido quando "Get-AzVm" é invocado com "-Status"</span><span class="sxs-lookup"><span data-stu-id="a76a3-126">Added 'VMHealth' property to the virtual machine's instance view, which is the returned object when 'Get-AzVm' is invoked with '-Status'</span></span>
* <span data-ttu-id="a76a3-127">Foi adicionado o campo "AssignedHost" às vistas de instância "Get-AzVM" e "Get-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="a76a3-127">Added 'AssignedHost' field to 'Get-AzVM' and 'Get-AzVmss' instance views.</span></span> <span data-ttu-id="a76a3-128">O campo mostra o ID de recurso da instância da máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a76a3-128">The field shows the resource id of the virtual machine instance</span></span>
* <span data-ttu-id="a76a3-129">Foi adicionado o parâmetro opcional "-SupportAutomaticPlacement" a "New-AzHostGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-129">Added optional parameter '-SupportAutomaticPlacement' to 'New-AzHostGroup'</span></span> 
* <span data-ttu-id="a76a3-130">Foi adicionado o parâmetro "-HostGroupId" a "New-AzVm" e "New-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="a76a3-130">Added the '-HostGroupId' parameter to 'New-AzVm' and 'New-AzVmss'</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-131">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-131">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-132">Atualização da versão do SDK de .Net do ADF para 4.11.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-132">Updated ADF .Net SDK version to 4.11.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-133">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-133">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-134">Foram adicionados novos cmdlets de Cluster - "New-AzEventHubCluster", "Set-AzEventHubCluster", "Get-AzEventHubCluster", "Remove-AzEventHubCluster", "Get-AzEventHubClustersAvailableRegions".</span><span class="sxs-lookup"><span data-stu-id="a76a3-134">Added new Cluster cmdlets - 'New-AzEventHubCluster', 'Set-AzEventHubCluster', 'Get-AzEventHubCluster', 'Remove-AzEventHubCluster', 'Get-AzEventHubClustersAvailableRegions'.</span></span>
* <span data-ttu-id="a76a3-135">Foi corrigido o problema #10722: Correção para atribuir apenas "Listen" aos direitos de AuthorizationRule.</span><span class="sxs-lookup"><span data-stu-id="a76a3-135">Fixed for issue #10722 : Fix for assigning only 'Listen' to AuthorizationRule rights.</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="a76a3-136">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="a76a3-136">Az.Functions</span></span>
* <span data-ttu-id="a76a3-137">Foi removida a capacidade de criar Funções V2 em regiões que não as suportam.</span><span class="sxs-lookup"><span data-stu-id="a76a3-137">Removed the ability to create v2 Functions in regions that do not support it.</span></span>
* <span data-ttu-id="a76a3-138">PowerShell 6.2 preterido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-138">Deprecated PowerShell 6.2.</span></span> <span data-ttu-id="a76a3-139">Foi adicionado um aviso para quando um utilizador criar uma aplicação de funções do PowerShell 6.2 que recomenda a criação de uma aplicação de funções do PowerShell 7.0.</span><span class="sxs-lookup"><span data-stu-id="a76a3-139">Added a warning for when a user creates a PowerShell 6.2 function app that advises them to create a PowerShell 7.0 function app instead.</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-140">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-140">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-141">Criação de cluster com configuração de Dimensionamento Automático suportada</span><span class="sxs-lookup"><span data-stu-id="a76a3-141">Supported creating cluster with Autoscale configuration</span></span>
    - <span data-ttu-id="a76a3-142">Foi adicionado o novo parâmetro "AutoscaleConfiguration" ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-142">Add new parameter 'AutoscaleConfiguration' to the cmdlet 'New-AzHDInsightCluster'</span></span>
* <span data-ttu-id="a76a3-143">Configuração de Dimensionamento Automático do cluster em funcionamento suportada</span><span class="sxs-lookup"><span data-stu-id="a76a3-143">Supported operating cluster's Autoscale configuration</span></span>
    - <span data-ttu-id="a76a3-144">Foi adicionado o novo cmdlet "Get-AzHDInsihgtClusterAutoscaleConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-144">Add new cmdlet 'Get-AzHDInsihgtClusterAutoscaleConfiguration'</span></span>
    - <span data-ttu-id="a76a3-145">Foi adicionado o novo cmdlet "New-AzHDInsihgtClusterAutoscaleConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-145">Add new cmdlet 'New-AzHDInsihgtClusterAutoscaleConfiguration'</span></span>
    - <span data-ttu-id="a76a3-146">Foi adicionado o novo cmdlet "Set-AzHDInsihgtClusterAutoscaleConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-146">Add new cmdlet 'Set-AzHDInsihgtClusterAutoscaleConfiguration'</span></span>
    - <span data-ttu-id="a76a3-147">Foi adicionado o novo cmdlet "Remove-AzHDInsihgtClusterAutoscaleConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-147">Add new cmdlet 'Remove-AzHDInsihgtClusterAutoscaleConfiguration'</span></span>
    - <span data-ttu-id="a76a3-148">Foi adicionado o novo cmdlet "New-AzHDInsihgtClusterAutoscaleScheduleCondition"</span><span class="sxs-lookup"><span data-stu-id="a76a3-148">Add new cmdlet 'New-AzHDInsihgtClusterAutoscaleScheduleCondition'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-149">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-149">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-150">Foi adicionado o suporte da autorização RBAC [#10557]</span><span class="sxs-lookup"><span data-stu-id="a76a3-150">Added support for RBAC authorization [#10557]</span></span>
* <span data-ttu-id="a76a3-151">Processamento de erros melhorado em "Set-AzKeyVaultAccessPolicy" [#4007]</span><span class="sxs-lookup"><span data-stu-id="a76a3-151">Enhanced error handling in 'Set-AzKeyVaultAccessPolicy' [#4007]</span></span>

#### <a name="azkusto"></a><span data-ttu-id="a76a3-152">Az.Kusto</span><span class="sxs-lookup"><span data-stu-id="a76a3-152">Az.Kusto</span></span>
* <span data-ttu-id="a76a3-153">Disponibilidade geral do módulo "Az.Kusto"</span><span class="sxs-lookup"><span data-stu-id="a76a3-153">General availability of 'Az.Kusto' module</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-154">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-154">Az.Network</span></span>
* <span data-ttu-id="a76a3-155">[Alteração interruptiva] Os cmdlets abaixo foram atualizados para estarem alinhados com o router e o hub virtuais de recursos</span><span class="sxs-lookup"><span data-stu-id="a76a3-155">[Breaking Change] Updated below cmdlets to align resource virtual router and virtual hub</span></span>
    - <span data-ttu-id="a76a3-156">"New-AzVirtualRouter":</span><span class="sxs-lookup"><span data-stu-id="a76a3-156">'New-AzVirtualRouter':</span></span> 
        - <span data-ttu-id="a76a3-157">Foi adicionado o parâmetro -HostedSubnet para suportar o recurso subordinado da configuração de IP</span><span class="sxs-lookup"><span data-stu-id="a76a3-157">Added -HostedSubnet parameter to support IP configuration child resource</span></span>
        - <span data-ttu-id="a76a3-158">-HostedGateway e -HostedGatewayId foram eliminados</span><span class="sxs-lookup"><span data-stu-id="a76a3-158">deleted -HostedGateway and -HostedGatewayId</span></span>
    - <span data-ttu-id="a76a3-159">"Get-AzVirtualRouter":</span><span class="sxs-lookup"><span data-stu-id="a76a3-159">'Get-AzVirtualRouter':</span></span>
        - <span data-ttu-id="a76a3-160">Foi adicionado um conjunto de parâmetros ao nível da subscrição</span><span class="sxs-lookup"><span data-stu-id="a76a3-160">Added subscription level parameter set</span></span>
    - <span data-ttu-id="a76a3-161">"Remove-AzVirtualRouter"</span><span class="sxs-lookup"><span data-stu-id="a76a3-161">'Remove-AzVirtualRouter'</span></span>
    - <span data-ttu-id="a76a3-162">"Add-AzVirtualRouterPeer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-162">'Add-AzVirtualRouterPeer'</span></span>
    - <span data-ttu-id="a76a3-163">"Get-AzVirtualRouterPeer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-163">'Get-AzVirtualRouterPeer'</span></span>
    - <span data-ttu-id="a76a3-164">"Remove-AzVirtualRouterPeer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-164">'Remove-AzVirtualRouterPeer'</span></span>
* <span data-ttu-id="a76a3-165">Foi adicionado um novo cmdlet para a Porta do Azure Express Route</span><span class="sxs-lookup"><span data-stu-id="a76a3-165">Added new cmdlet for Azure Express Route Port</span></span>
    - <span data-ttu-id="a76a3-166">"New-AzExpressRoutePortLOA"</span><span class="sxs-lookup"><span data-stu-id="a76a3-166">'New-AzExpressRoutePortLOA'</span></span>
* <span data-ttu-id="a76a3-167">Foi adicionada a propriedade RemoteBgpCommunities ao Recurso de Peering de VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="a76a3-167">Added RemoteBgpCommunities property to the VirtualNetwork Peering Resource</span></span>
* <span data-ttu-id="a76a3-168">Foi modificada a mensagem de aviso de "New-AzLoadBalancerFrontendIpConfig", "New-AzPublicIpAddress" e "New-AzPublicIpPrefix".</span><span class="sxs-lookup"><span data-stu-id="a76a3-168">Modified the warning message for 'New-AzLoadBalancerFrontendIpConfig', 'New-AzPublicIpAddress' and 'New-AzPublicIpPrefix'.</span></span>
* <span data-ttu-id="a76a3-169">Foi adicionado VpnGatewayIpConfigurations à saída "Get-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-169">Added VpnGatewayIpConfigurations to 'Get-AzVpnGateway' output</span></span>
* <span data-ttu-id="a76a3-170">Foi corrigido o erro de "Set-AzApplicationGatewaySslCertificate" [#9488]</span><span class="sxs-lookup"><span data-stu-id="a76a3-170">Fixed bug for 'Set-AzApplicationGatewaySslCertificate' [#9488]</span></span>
* <span data-ttu-id="a76a3-171">Foi adicionado o parâmetro "AllowActiveFTP" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="a76a3-171">Added 'AllowActiveFTP' parameter to 'AzureFirewall'</span></span>
* <span data-ttu-id="a76a3-172">Foram atualizados os seguintes comandos para a funcionalidade: Ativação da definição/remoção de segurança na Internet no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="a76a3-172">Updated below commands for feature: Enable internet security set/remove on VirtualWan P2SVpnGateway.</span></span>
- <span data-ttu-id="a76a3-173">Atualização de "New-AzP2sVpnGateway": Foi adicionado o parâmetro opcional "EnableInternetSecurityFlag" para que os clientes definam como true para ativar a segurança na Internet no P2SVpnGateway, que será aplicado aos clientes de Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="a76a3-173">Updated 'New-AzP2sVpnGateway': Added optional switch parameter 'EnableInternetSecurityFlag' for customers to set true to enable internet security on P2SVpnGateway, which will be applied for Point to site clients.</span></span>
- <span data-ttu-id="a76a3-174">Atualização de "Update-AzP2sVpnGateway": Foi adicionado o parâmetro opcional "EnableInternetSecurityFlag" ou "DisableInternetSecurityFlag" para que os clientes definam como true/false para ativar/desativar a segurança na Internet no P2SVpnGateway, que será aplicado aos clientes de Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="a76a3-174">Updated 'Update-AzP2sVpnGateway': Added optional switch parameters 'EnableInternetSecurityFlag' or 'DisableInternetSecurityFlag' for customers to set true/false to enable/disable internet security on P2SVpnGateway, which will be applied for Point to site clients.</span></span>
* <span data-ttu-id="a76a3-175">Foi adicionado o novo cmdlet "Reset-AzP2sVpnGateway" para que os clientes redefinam/reiniciem o P2SVpnGateway de VirtualWan para resolução de problemas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-175">Added new cmdlet 'Reset-AzP2sVpnGateway' for customers to reset/reboot their VirtualWan P2SVpnGateway for troubleshooting.</span></span>
* <span data-ttu-id="a76a3-176">Foi adicionado o novo cmdlet "Reset-AzVpnGateway" para que os clientes redefinam/reiniciem o VpnGateway de VirtualWan para resolução de problemas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-176">Added new cmdlet 'Reset-AzVpnGateway' for customers to reset/reboot their VirtualWan VpnGateway for troubleshooting.</span></span>
* <span data-ttu-id="a76a3-177">Atualização de "Set-AzVirtualNetworkSubnetConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-177">Updated 'Set-AzVirtualNetworkSubnetConfig'</span></span>
    - <span data-ttu-id="a76a3-178">Definir as propriedades do NSG e da Tabela de Encaminhamento da sub-rede como null se estiverem definidas explicitamente nos parâmetros [#1548][#9718]</span><span class="sxs-lookup"><span data-stu-id="a76a3-178">Set NSG and Route Table properties of subnet to null if explicitly set in parameters [#1548][#9718]</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-179">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-179">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-180">Foi corrigido o Estado de Eliminação para Itens de Cópia de Segurança das cargas de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a76a3-180">Fixed the Delete State for workload Backup Items.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-181">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-181">Az.Resources</span></span>
* <span data-ttu-id="a76a3-182">Foi adicionada uma verificação em falta para Set-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a76a3-182">Added missing check for Set-AzRoleAssignment</span></span>
* <span data-ttu-id="a76a3-183">Foi adicionado o atributo de alteração interruptiva ao parâmetro "SubscriptionId" de "Get-AzResourceGroupDeploymentOperation"</span><span class="sxs-lookup"><span data-stu-id="a76a3-183">Added breaking change attribute to 'SubscriptionId' parameter of 'Get-AzResourceGroupDeploymentOperation'</span></span>
* <span data-ttu-id="a76a3-184">Foram atualizados os cmdlets What-If do modelo do ARM para mostrar as alterações de recursos "Ignore" no final</span><span class="sxs-lookup"><span data-stu-id="a76a3-184">Updated ARM template What-If cmdlets to show 'Ignore' resource changes last</span></span>
* <span data-ttu-id="a76a3-185">Foram corrigidos os problemas de serialização de parâmetros seguros e de matriz para cmdlets de implementação [#12773]</span><span class="sxs-lookup"><span data-stu-id="a76a3-185">Fixed secure and array parameter serialization issues for deployment cmdlets [#12773]</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-186">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-186">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-187">Foram adicionados novos cmdlets aos tipos de nós e clusters geridos:</span><span class="sxs-lookup"><span data-stu-id="a76a3-187">Added new cmdlets for managed clusters and node types:</span></span>
    - <span data-ttu-id="a76a3-188">"New-AzServiceFabricManagedCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-188">'New-AzServiceFabricManagedCluster'</span></span>
    - <span data-ttu-id="a76a3-189">"Get-AzServiceFabricManagedCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-189">'Get-AzServiceFabricManagedCluster'</span></span>
    - <span data-ttu-id="a76a3-190">"Set-AzServiceFabricManagedCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-190">'Set-AzServiceFabricManagedCluster'</span></span>
    - <span data-ttu-id="a76a3-191">"Remove-AzServiceFabricManagedCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-191">'Remove-AzServiceFabricManagedCluster'</span></span>
    - <span data-ttu-id="a76a3-192">"Add-AzServiceFabricManagedClusterClientCertificate"</span><span class="sxs-lookup"><span data-stu-id="a76a3-192">'Add-AzServiceFabricManagedClusterClientCertificate'</span></span>
    - <span data-ttu-id="a76a3-193">"Remove-AzServiceFabricManagedClusterClientCertificate"</span><span class="sxs-lookup"><span data-stu-id="a76a3-193">'Remove-AzServiceFabricManagedClusterClientCertificate'</span></span>
    - <span data-ttu-id="a76a3-194">"New-AzServiceFabricManagedNodeType"</span><span class="sxs-lookup"><span data-stu-id="a76a3-194">'New-AzServiceFabricManagedNodeType'</span></span>
    - <span data-ttu-id="a76a3-195">"Get-AzServiceFabricManagedNodeType"</span><span class="sxs-lookup"><span data-stu-id="a76a3-195">'Get-AzServiceFabricManagedNodeType'</span></span>
    - <span data-ttu-id="a76a3-196">"Set-AzServiceFabricManagedNodeType"</span><span class="sxs-lookup"><span data-stu-id="a76a3-196">'Set-AzServiceFabricManagedNodeType'</span></span>
    - <span data-ttu-id="a76a3-197">"Remove-AzServiceFabricManagedNodeType"</span><span class="sxs-lookup"><span data-stu-id="a76a3-197">'Remove-AzServiceFabricManagedNodeType'</span></span>
    - <span data-ttu-id="a76a3-198">"Add-AzServiceFabricManagedNodeTypeVMExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-198">'Add-AzServiceFabricManagedNodeTypeVMExtension'</span></span>
    - <span data-ttu-id="a76a3-199">"Add-AzServiceFabricManagedNodeTypeVMSecret"</span><span class="sxs-lookup"><span data-stu-id="a76a3-199">'Add-AzServiceFabricManagedNodeTypeVMSecret'</span></span>
    - <span data-ttu-id="a76a3-200">"Remove-AzServiceFabricManagedNodeTypeVMExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-200">'Remove-AzServiceFabricManagedNodeTypeVMExtension'</span></span>
    - <span data-ttu-id="a76a3-201">"Restart-AzServiceFabricManagedNodeTyp"</span><span class="sxs-lookup"><span data-stu-id="a76a3-201">'Restart-AzServiceFabricManagedNodeTyp'</span></span>
* <span data-ttu-id="a76a3-202">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2020-03-01 para o modelo atual e 2020-01-01-preview para clusters geridos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-202">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2020-03-01 for the current model and 2020-01-01-preview for managed clusters.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-203">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-203">Az.Sql</span></span>
* <span data-ttu-id="a76a3-204">Foi adicionado BackupStorageRedundancy a "New-AzSqlInstance" e "Get-AzSqlInstance"</span><span class="sxs-lookup"><span data-stu-id="a76a3-204">Added BackupStorageRedundancy to 'New-AzSqlInstance' and 'Get-AzSqlInstance'</span></span>
* <span data-ttu-id="a76a3-205">Foi adicionado o cmdlet "Get-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="a76a3-205">Added cmdlet 'Get-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="a76a3-206">Foi adicionado o cmdlet "Enable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="a76a3-206">Added cmdlet 'Enable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="a76a3-207">Foi adicionado o parâmetro Force a "New-AzSqlInstance"</span><span class="sxs-lookup"><span data-stu-id="a76a3-207">Added Force parameter to 'New-AzSqlInstance'</span></span>
* <span data-ttu-id="a76a3-208">Foram adicionados cmdlets para o serviço Managed Database Log Replay</span><span class="sxs-lookup"><span data-stu-id="a76a3-208">Added cmdlets for Managed Database Log Replay service</span></span>
    - <span data-ttu-id="a76a3-209">"Start-AzSqlInstanceDatabaseLogReplay"</span><span class="sxs-lookup"><span data-stu-id="a76a3-209">'Start-AzSqlInstanceDatabaseLogReplay'</span></span>
    - <span data-ttu-id="a76a3-210">"Get-AzSqlInstanceDatabaseLogReplay"</span><span class="sxs-lookup"><span data-stu-id="a76a3-210">'Get-AzSqlInstanceDatabaseLogReplay'</span></span>
    - <span data-ttu-id="a76a3-211">"Complete-AzSqlInstanceDatabaseLogReplay"</span><span class="sxs-lookup"><span data-stu-id="a76a3-211">'Complete-AzSqlInstanceDatabaseLogReplay'</span></span>
    - <span data-ttu-id="a76a3-212">"Stop-AzSqlInstanceDatabaseLogReplay"</span><span class="sxs-lookup"><span data-stu-id="a76a3-212">'Stop-AzSqlInstanceDatabaseLogReplay'</span></span>
* <span data-ttu-id="a76a3-213">Foi adicionado o cmdlet "Get-AzSqlInstanceActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="a76a3-213">Added cmdlet 'Get-AzSqlInstanceActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="a76a3-214">Foi adicionado o cmdlet "Enable-AzSqlInstanceActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="a76a3-214">Added cmdlet 'Enable-AzSqlInstanceActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="a76a3-215">Foi adicionado o cmdlet "Disable-AzSqlInstanceActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="a76a3-215">Added cmdlet 'Disable-AzSqlInstanceActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="a76a3-216">Foram adicionados os cmdlets "New-AzSqlDatabaseImport" e "New-AzSqlDatabaseExport" para suportar a funcionalidade de isolamento de rede</span><span class="sxs-lookup"><span data-stu-id="a76a3-216">Updated cmdlets 'New-AzSqlDatabaseImport' and 'New-AzSqlDatabaseExport' to support network isolation functionality</span></span>
* <span data-ttu-id="a76a3-217">Foi adicionado o cmdlet "New-AzSqlDatabaseImportExisting"</span><span class="sxs-lookup"><span data-stu-id="a76a3-217">Added cmdlet 'New-AzSqlDatabaseImportExisting'</span></span>
* <span data-ttu-id="a76a3-218">Foram atualizados os cmdlets das Bases de Dados para suportar a especificação do tipo de armazenamento de cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="a76a3-218">Updated Databases cmdlets to support backup storage type specification</span></span>
* <span data-ttu-id="a76a3-219">Foi adicionado o parâmetro Force a "New-AzSqlDatabase"</span><span class="sxs-lookup"><span data-stu-id="a76a3-219">Added Force parameter to 'New-AzSqlDatabase'</span></span>
* <span data-ttu-id="a76a3-220">Foi adicionado um aviso para a configuração de BackupStorageRedundancy nas regiões selecionadas em "New-AzSqlDatabase"</span><span class="sxs-lookup"><span data-stu-id="a76a3-220">Added warning for BackupStorageRedundancy configuration in select regions in 'New-AzSqlDatabase'</span></span>
* <span data-ttu-id="a76a3-221">Foram atualizados os cmdlets ActiveDirectoryOnlyAuthentication para o servidor e a instância para incluir ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-221">Updated ActiveDirectoryOnlyAuthentication cmdlets for server and instance to include ResourceId and InputObject</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-222">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-222">Az.Storage</span></span>
* <span data-ttu-id="a76a3-223">Foi corrigida a falha no blob de carregamento através da atualização de Microsoft.Azure.Storage.DataMovement 2.0.0 [#12220]</span><span class="sxs-lookup"><span data-stu-id="a76a3-223">Fixed upload blob fail by upgrade to Microsoft.Azure.Storage.DataMovement 2.0.0 [#12220]</span></span>
* <span data-ttu-id="a76a3-224">Restauro para um Ponto Anterior no Tempo suportado</span><span class="sxs-lookup"><span data-stu-id="a76a3-224">Supported Point In Time Restore</span></span>
    - <span data-ttu-id="a76a3-225">"Enable-AzStorageBlobRestorePolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-225">'Enable-AzStorageBlobRestorePolicy'</span></span>
    - <span data-ttu-id="a76a3-226">"Disable-AzStorageBlobRestorePolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-226">'Disable-AzStorageBlobRestorePolicy'</span></span>
    - <span data-ttu-id="a76a3-227">"New-AzStorageBlobRangeToRestore"</span><span class="sxs-lookup"><span data-stu-id="a76a3-227">'New-AzStorageBlobRangeToRestore'</span></span>
    - <span data-ttu-id="a76a3-228">"Restore-AzStorageBlobRange"</span><span class="sxs-lookup"><span data-stu-id="a76a3-228">'Restore-AzStorageBlobRange'</span></span>
* <span data-ttu-id="a76a3-229">Suporte para obter o estado de restauro de blobs da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeBlobRestoreStatus</span><span class="sxs-lookup"><span data-stu-id="a76a3-229">Supported get blob restore status of Storage account by run get-AzureRMStorageAccount with parameter -IncludeBlobRestoreStatus</span></span> 
    - <span data-ttu-id="a76a3-230">"Get-AzureRMStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-230">'Get-AzureRMStorageAccount'</span></span>
* <span data-ttu-id="a76a3-231">Foi adicionada uma mensagem de aviso de alteração interruptiva para alteração da saída dos cmdlets futuros</span><span class="sxs-lookup"><span data-stu-id="a76a3-231">Added breaking change warning message for upcoming cmdlet output change</span></span>
    - <span data-ttu-id="a76a3-232">"Get-AzStorageContainerStoredAccessPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-232">'Get-AzStorageContainerStoredAccessPolicy'</span></span>
    - <span data-ttu-id="a76a3-233">"Set-AzStorageContainerStoredAccessPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-233">'Set-AzStorageContainerStoredAccessPolicy'</span></span>
    - <span data-ttu-id="a76a3-234">"Set-AzStorageAccountManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-234">'Set-AzStorageAccountManagementPolicy'</span></span>
    - <span data-ttu-id="a76a3-235">"Get-AzStorageAccountManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-235">'Get-AzStorageAccountManagementPolicy'</span></span>
    - <span data-ttu-id="a76a3-236">"Add-AzStorageAccountManagementPolicyAction"</span><span class="sxs-lookup"><span data-stu-id="a76a3-236">'Add-AzStorageAccountManagementPolicyAction'</span></span>
    - <span data-ttu-id="a76a3-237">"New-AzStorageAccountManagementPolicyRule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-237">'New-AzStorageAccountManagementPolicyRule'</span></span>
* <span data-ttu-id="a76a3-238">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.8</span><span class="sxs-lookup"><span data-stu-id="a76a3-238">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.8</span></span>

### <a name="thanks-to-our-community-contributors"></a><span data-ttu-id="a76a3-239">Agradecemos aos colaboradores da comunidade</span><span class="sxs-lookup"><span data-stu-id="a76a3-239">Thanks to our community contributors</span></span>
* <span data-ttu-id="a76a3-240">Thomas Van Laere (@ThomVanL), adição de Dockerfile-alpine-3.10 (#12911)</span><span class="sxs-lookup"><span data-stu-id="a76a3-240">Thomas Van Laere (@ThomVanL), Add Dockerfile-alpine-3.10 (#12911)</span></span> 
* <span data-ttu-id="a76a3-241">Lohith Chowdary Chilukuri (@Lochiluk), atualização de Remove-AzNetworkInterfaceIpConfig.md (#12807)</span><span class="sxs-lookup"><span data-stu-id="a76a3-241">Lohith Chowdary Chilukuri (@Lochiluk), Update Remove-AzNetworkInterfaceIpConfig.md (#12807)</span></span> 
* <span data-ttu-id="a76a3-242">Roberth Strand (@roberthstrand), Get-AzResourceGroup - Novo exemplo e limpeza (#12828)</span><span class="sxs-lookup"><span data-stu-id="a76a3-242">Roberth Strand (@roberthstrand), Get-AzResourceGroup - New example, and cleanup (#12828)</span></span> 
* <span data-ttu-id="a76a3-243">Ravi Mishra (@inmishrar), atualização da pilha de runtime da Aplicação Web do Azure para DOTNETCORE (#12833)</span><span class="sxs-lookup"><span data-stu-id="a76a3-243">Ravi Mishra (@inmishrar), update Azure Web App runtime stack to DOTNETCORE (#12833)</span></span> 
* <span data-ttu-id="a76a3-244">@jack-education, Set-AzVirtualNetworkSubnetConfig atualizado para permitir a remoção do NSG e da Tabela de Encaminhamento da sub-rede (#12351)</span><span class="sxs-lookup"><span data-stu-id="a76a3-244">@jack-education, Updated Set-AzVirtualNetworkSubnetConfig to allow NSG and Route Table to be removed from subnet (#12351)</span></span> 
* <span data-ttu-id="a76a3-245">@hagop-globanet, atualização de Add-AzApplicationGatewayCustomError.md (#12784)</span><span class="sxs-lookup"><span data-stu-id="a76a3-245">@hagop-globanet, Update Add-AzApplicationGatewayCustomError.md (#12784)</span></span> 
* <span data-ttu-id="a76a3-246">Joshua Van Daalen (@greenSacrifice)</span><span class="sxs-lookup"><span data-stu-id="a76a3-246">Joshua Van Daalen (@greenSacrifice)</span></span>
  * <span data-ttu-id="a76a3-247">Atualização da ortografia de Property para Property (#12821)</span><span class="sxs-lookup"><span data-stu-id="a76a3-247">Update spelling of Property to Property (#12821)</span></span> 
  * <span data-ttu-id="a76a3-248">Atualização dos exemplos de New-AzResourceLock.md (#12806)</span><span class="sxs-lookup"><span data-stu-id="a76a3-248">Update New-AzResourceLock.md examples (#12806)</span></span>
* <span data-ttu-id="a76a3-249">Eragon Riddle (@eragonriddle), correção do nome do campo do parâmetro no exemplo (#12825)</span><span class="sxs-lookup"><span data-stu-id="a76a3-249">Eragon Riddle (@eragonriddle), Corrected parameter field name in the example (#12825)</span></span> 
* <span data-ttu-id="a76a3-250">@rossifumax, correção do erro de digitação em New-AzConfigurationAssignment.md (#12701)</span><span class="sxs-lookup"><span data-stu-id="a76a3-250">@rossifumax, Fix typo in New-AzConfigurationAssignment.md (#12701)</span></span>

## <a name="461---august-2020"></a><span data-ttu-id="a76a3-251">4.6.1 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-251">4.6.1 - August 2020</span></span>
#### <a name="azcompute"></a><span data-ttu-id="a76a3-252">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-252">Az.Compute</span></span>
* <span data-ttu-id="a76a3-253">Correção do parâmetro "-EncryptionAtHost" em "New-AzVm" para remover o valor predefinido de falso [#12776]</span><span class="sxs-lookup"><span data-stu-id="a76a3-253">Patched '-EncryptionAtHost' parameter in 'New-AzVm' to remove default value of false [#12776]</span></span>

## <a name="460---august-2020"></a><span data-ttu-id="a76a3-254">4.6.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-254">4.6.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-255">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-255">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-256">São carregados todos os ambientes de cloud pública quando o ponto final de deteção não devolve o AzureCloud predefinido ou outros ambientes públicos [#12633]</span><span class="sxs-lookup"><span data-stu-id="a76a3-256">Loaded all public cloud environments when discovery endpoint doesn't return default AzureCloud or other public environments [#12633]</span></span>
* <span data-ttu-id="a76a3-257">Exposição de SubscriptionPolicies em "Get-AzSubscription" [#12551]</span><span class="sxs-lookup"><span data-stu-id="a76a3-257">Exposed SubscriptionPolicies in 'Get-AzSubscription' [#12551]</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-258">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-258">Az.Automation</span></span>
* <span data-ttu-id="a76a3-259">Adição de parâmetros "-RunOn" a "Set-AzAutomationWebhook" para especificar um Grupo de Função de Trabalho Híbrida</span><span class="sxs-lookup"><span data-stu-id="a76a3-259">Added '-RunOn' parameters to 'Set-AzAutomationWebhook' to specify a Hybrid Worker Group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-260">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-260">Az.Compute</span></span>
* <span data-ttu-id="a76a3-261">Adição do parâmetro "-EncryptionAtHost" a "New-AzVm", "New-AzVmss", "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVM" e "Update-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="a76a3-261">Added '-EncryptionAtHost' parameter to 'New-AzVm', 'New-AzVmss', 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVM', and 'Update-AzVmss'</span></span>
* <span data-ttu-id="a76a3-262">Adição de "SecurityProfile" ao objeto de retorno "Get-AzVM" e "Get-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="a76a3-262">Added 'SecurityProfile' to 'Get-AzVM' and 'Get-AzVmss' return object</span></span>
* <span data-ttu-id="a76a3-263">Adição do comutador "-InstanceView" como parâmetro opcional a "Get-AzHostGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-263">Added '-InstanceView' switch as optional parameter to 'Get-AzHostGroup'</span></span>
* <span data-ttu-id="a76a3-264">Adição do novo cmdlet "Invoke-AzVmPatchAssessment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-264">Added new cmdlet 'Invoke-AzVmPatchAssessment'</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-265">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-265">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-266">Adição das propriedades em falta à classe PSPipelineRun.</span><span class="sxs-lookup"><span data-stu-id="a76a3-266">Added missing properties to PSPipelineRun class.</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-267">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-267">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-268">É suportada a criação de clusters com encriptação na funcionalidade de anfitrião.</span><span class="sxs-lookup"><span data-stu-id="a76a3-268">Supported creating cluster with encryption at host feature.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-269">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-269">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-270">Adição de mensagens de aviso para planear a desativação da eliminação recuperável</span><span class="sxs-lookup"><span data-stu-id="a76a3-270">Added warning messages for planning to disable soft delete</span></span>
* <span data-ttu-id="a76a3-271">Adição de mensagens de aviso para planear a remoção do atributo SecretValueText</span><span class="sxs-lookup"><span data-stu-id="a76a3-271">Added warning messages for planning to remove attribute SecretValueText</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="a76a3-272">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="a76a3-272">Az.Maintenance</span></span>
* <span data-ttu-id="a76a3-273">Adição de campos relacionados com agendamento opcionais a "New-AzMaintenanceConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-273">Added optional schedule related fields to 'New-AzMaintenanceConfiguration'</span></span>
* <span data-ttu-id="a76a3-274">Adição do novo cmdlet para "Get-AzMaintenancePublicConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-274">Added new cmdlet for 'Get-AzMaintenancePublicConfiguration'</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="a76a3-275">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-275">Az.ManagedServices</span></span>
* <span data-ttu-id="a76a3-276">Adição de avisos de alteração interruptiva nos cmdlets de atribuição e definição de serviços geridos</span><span class="sxs-lookup"><span data-stu-id="a76a3-276">Added breaking change warnings on cmdlets of managed services assignment and definition</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-277">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-277">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-278">Expansão do parâmetro definido em "Set-AzDiagnosticSetting" para a separação da ativação de Registos e Métricas [#12482]</span><span class="sxs-lookup"><span data-stu-id="a76a3-278">Extended the parameter set in 'Set-AzDiagnosticSetting' for separation of Logs and Metrics enablement [#12482]</span></span>
* <span data-ttu-id="a76a3-279">Correção do erro de "Add-AzMetricAlertRuleV2" ao obter o alerta de métrica do pipeline</span><span class="sxs-lookup"><span data-stu-id="a76a3-279">Fixed bug for 'Add-AzMetricAlertRuleV2' when getting metric alert from pipeline</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-280">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-280">Az.Resources</span></span>
* <span data-ttu-id="a76a3-281">Atualização da resposta "Get-AzPolicyAlias" no sentido de incluir informações que indicam se o alias pode ser modificado pelo Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="a76a3-281">Updated 'Get-AzPolicyAlias' response to include information indicating whether the alias is modifiable by Azure Policy.</span></span>
* <span data-ttu-id="a76a3-282">Criação do novo cmdlet "Set-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-282">Created new cmdlet 'Set-AzRoleAssignment'</span></span>
* <span data-ttu-id="a76a3-283">Adição de "Get-AzDeploymentManagementGroupWhatIfResult" para obter os resultados de Hipóteses do modelo do ARM no âmbito do Grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="a76a3-283">Added 'Get-AzDeploymentManagementGroupWhatIfResult' for getting ARM template What-If results at management Group scope</span></span>
* <span data-ttu-id="a76a3-284">Adição do novo cmdlet "Get-AzTenantWhatIfResult" para obter os resultados de Hipóteses do modelo do ARM no âmbito do inquilino</span><span class="sxs-lookup"><span data-stu-id="a76a3-284">Added 'Get-AzTenantWhatIfResult' new cmdlet for getting ARM template What-If results at tenant scope</span></span>
* <span data-ttu-id="a76a3-285">Substituição de "-WhatIf" e "-Confirm" por "New-AzManagementGroupDeployment" e "New-AzTenantDeployment" no sentido de utilizar os resultados de Hipóteses do modelo do ARM</span><span class="sxs-lookup"><span data-stu-id="a76a3-285">Overrode '-WhatIf' and '-Confirm' for 'New-AzManagementGroupDeployment' and 'New-AzTenantDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="a76a3-286">Correção dos comportamentos de "-WhatIf" e "-Confirm" para os novos cmdlets de implementação para que estejam em conformidade com Falso e</span><span class="sxs-lookup"><span data-stu-id="a76a3-286">Fixed the behaviors of '-WhatIf' and '-Confirm' for new deployment cmdlets so they comply with False and</span></span> 
* <span data-ttu-id="a76a3-287">Correção do erro de serialização de "-TemplateObject" e "TemplateParameterObject" [#1528] [#6292]</span><span class="sxs-lookup"><span data-stu-id="a76a3-287">Fixed serialization error for '-TemplateObject' and 'TemplateParameterObject' [#1528] [#6292]</span></span>
* <span data-ttu-id="a76a3-288">Adição do atributo de alteração interruptiva a "Get-AzResourceGroupDeploymentOperation" para a próxima alteração do tipo de saída</span><span class="sxs-lookup"><span data-stu-id="a76a3-288">Added breaking change attribute to 'Get-AzResourceGroupDeploymentOperation' for the upcoming output type change</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a76a3-289">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a76a3-289">Az.SignalR</span></span>
* <span data-ttu-id="a76a3-290">Correção dos erros dos ficheiros de ajuda "Restart-AzSignalR" e "Update-AzSignalR"</span><span class="sxs-lookup"><span data-stu-id="a76a3-290">Fixed 'Restart-AzSignalR' and 'Update-AzSignalR' help files errors</span></span>
* <span data-ttu-id="a76a3-291">Adição dos cmdlets "Update-AzSignalRNetworkAcl" e "Set-AzSignalRUpstream"</span><span class="sxs-lookup"><span data-stu-id="a76a3-291">Added cmdlets 'Update-AzSignalRNetworkAcl', 'Set-AzSignalRUpstream'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-292">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-292">Az.Storage</span></span>
* <span data-ttu-id="a76a3-293">É suportada a aceleração da consulta de blobs</span><span class="sxs-lookup"><span data-stu-id="a76a3-293">Supported blob query acceleration</span></span>
    -  <span data-ttu-id="a76a3-294">"Get-AzStorageBlobQueryResult"</span><span class="sxs-lookup"><span data-stu-id="a76a3-294">'Get-AzStorageBlobQueryResult'</span></span>
    -  <span data-ttu-id="a76a3-295">"New-AzStorageBlobQueryConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-295">'New-AzStorageBlobQueryConfig'</span></span>
* <span data-ttu-id="a76a3-296">Atualização do ficheiro de ajuda, com a adição de mais descrições e a correção de erros de digitação</span><span class="sxs-lookup"><span data-stu-id="a76a3-296">Updated help file, added more description, and fixed typo</span></span>
    -  <span data-ttu-id="a76a3-297">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-297">'Start-AzStorageBlobCopy'</span></span>
    -  <span data-ttu-id="a76a3-298">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="a76a3-298">'Get-AzDataLakeGen2Item'</span></span>
* <span data-ttu-id="a76a3-299">Correção da falha de transferência de blobs quando o subdiretório relacionado não existe [#12592]</span><span class="sxs-lookup"><span data-stu-id="a76a3-299">Fixed download blob fail when related sub directory not exist [#12592]</span></span>
    -  <span data-ttu-id="a76a3-300">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-300">'Get-AzStorageBlobContent'</span></span>
* <span data-ttu-id="a76a3-301">É suportada a Política de Replicação Definir/Obter/Remover Objeto nas Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-301">Supported Set/Get/Remove Object Replication Policy on Storage accounts</span></span>
    - <span data-ttu-id="a76a3-302">"New-AzStorageObjectReplicationPolicyRule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-302">'New-AzStorageObjectReplicationPolicyRule'</span></span>
    - <span data-ttu-id="a76a3-303">"Set-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-303">'Set-AzStorageObjectReplicationPolicy'</span></span>
    - <span data-ttu-id="a76a3-304">"Get-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-304">'Get-AzStorageObjectReplicationPolicy'</span></span>
    - <span data-ttu-id="a76a3-305">"Remove-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-305">'Remove-AzStorageObjectReplicationPolicy'</span></span>
* <span data-ttu-id="a76a3-306">Suporte para ativar/desativar o ChangeFeed no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-306">Supported enable/disable ChangeFeed on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="a76a3-307">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="a76a3-307">'Update-AzStorageBlobServiceProperty'</span></span>

## <a name="450---august-2020"></a><span data-ttu-id="a76a3-308">4.5.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-308">4.5.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-309">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-309">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-310">"Connect-AzAccount" atualizado para aceitar o parâmetro "MaxContextPopulation" [#9865]</span><span class="sxs-lookup"><span data-stu-id="a76a3-310">Updated 'Connect-AzAccount' to accept parameter 'MaxContextPopulation' [#9865]</span></span>
* <span data-ttu-id="a76a3-311">Versão de SubscriptionClient atualizada para a de 2019-06-01 e apresentação de domínios de inquilino [#9838]</span><span class="sxs-lookup"><span data-stu-id="a76a3-311">Updated SubscriptionClient version to 2019-06-01 and display tenant domains [#9838]</span></span>
* <span data-ttu-id="a76a3-312">Inquilino principal suportado e informações do inquilino managedBy da subscrição</span><span class="sxs-lookup"><span data-stu-id="a76a3-312">Supported home tenant and managedBy tenant information of subscription</span></span>
* <span data-ttu-id="a76a3-313">Nome do módulo corrigido, informações da versão nos dados telemétricos</span><span class="sxs-lookup"><span data-stu-id="a76a3-313">Corrected module name, version info in telemetry data</span></span>
* <span data-ttu-id="a76a3-314">SqlDatabaseDnsSuffix e ServiceManagementUrl ajustados se o ponto final dos metadados do ambiente devolverem valores incompatíveis</span><span class="sxs-lookup"><span data-stu-id="a76a3-314">Adjusted SqlDatabaseDnsSuffix and ServiceManagementUrl if environment metadata endpoint returns incompatible value</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-315">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-315">Az.Aks</span></span>
* <span data-ttu-id="a76a3-316">"ClientIdAndSecret" removido para "ServicePrincipalIdAndSecret" e "ClientIdAndSecret" definido como um alias [#12381].</span><span class="sxs-lookup"><span data-stu-id="a76a3-316">Removed 'ClientIdAndSecret' to 'ServicePrincipalIdAndSecret' and set 'ClientIdAndSecret' as an alias [#12381].</span></span>
* <span data-ttu-id="a76a3-317">"Get-AzAks"/"New-AzAks"/"Remove-AzAks"/"Set-AzAks" removidos para "Get-AzAksCluster"/"New-AzAksCluster"/"Remove-AzAksCluster"/"Set-AzAksCluster" e definição dos valores originais como alias [#12373].</span><span class="sxs-lookup"><span data-stu-id="a76a3-317">Removed 'Get-AzAks'/'New-AzAks'/'Remove-AzAks'/'Set-AzAks' to 'Get-AzAksCluster'/'New-AzAksCluster'/'Remove-AzAksCluster'/'Set-AzAksCluster' and set the original ones as alias [#12373].</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-318">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-318">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-319">Novo cmdlet "Add-AzApiManagementApiToGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-319">Added new 'Add-AzApiManagementApiToGateway' cmdlet.</span></span>
* <span data-ttu-id="a76a3-320">Novo cmdlet "Get-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-320">Added new 'Get-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="a76a3-321">Novo cmdlet "Get-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-321">Added new 'Get-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="a76a3-322">Novo cmdlet "Get-AzApiManagementGatewayKey" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-322">Added new 'Get-AzApiManagementGatewayKey' cmdlet.</span></span>
* <span data-ttu-id="a76a3-323">Novo cmdlet "New-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-323">Added new 'New-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="a76a3-324">Novo cmdlet "New-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-324">Added new 'New-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="a76a3-325">Novo cmdlet "New-AzApiManagementResourceLocationObject" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-325">Added new 'New-AzApiManagementResourceLocationObject' cmdlet.</span></span>
* <span data-ttu-id="a76a3-326">Novo cmdlet "Remove-AzApiManagementApiFromGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-326">Added new 'Remove-AzApiManagementApiFromGateway' cmdlet.</span></span>
* <span data-ttu-id="a76a3-327">Novo cmdlet "Remove-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-327">Added new 'Remove-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="a76a3-328">Novo cmdlet "Remove-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-328">Added new 'Remove-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="a76a3-329">Novo cmdlet "Update-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-329">Added new 'Update-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="a76a3-330">Foi adicionado um novo parâmetro [-GatewayId] opcional ao cmdlet "Get-AzApiManagementApi".</span><span class="sxs-lookup"><span data-stu-id="a76a3-330">Added new optional [-GatewayId] parameter to the 'Get-AzApiManagementApi' cmdlet.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-331">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-331">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-332">Utilizado "Deny" especificamente como ação NetworkRules predefinida.</span><span class="sxs-lookup"><span data-stu-id="a76a3-332">Used 'Deny' specifically as NetworkRules default action.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-333">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-333">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-334">Foi resolvido um problema em que é gerada uma exceção quando Enum.Parse tenta limitar um valor nulo a um valor de enumeração Enabled ou Disabled [#12344]</span><span class="sxs-lookup"><span data-stu-id="a76a3-334">Fixed an issue where an exception is being thrown when Enum.Parse tries to coerce a null value to an Enabled or Disabled enum values [#12344]</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-335">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-335">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-336">É suportada a criação de clusters com encriptação na funcionalidade de trânsito.</span><span class="sxs-lookup"><span data-stu-id="a76a3-336">Supported creating cluster with encryption in transit feature.</span></span>
    - <span data-ttu-id="a76a3-337">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-337">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="a76a3-338">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-338">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="a76a3-339">É suportada a criação de clusters com a funcionalidade de ligação privada:</span><span class="sxs-lookup"><span data-stu-id="a76a3-339">Supported creating cluster with private link feature:</span></span>
    - <span data-ttu-id="a76a3-340">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-340">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="a76a3-341">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-341">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="a76a3-342">Informações de rede virtual devolvidas ao chamar "New-AzHDInsightCluster" ou "Get-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-342">Returned virtual network information when calling 'New-AzHDInsightCluster' or 'Get-AzHDInsightCluster'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-343">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-343">Az.Network</span></span>
* <span data-ttu-id="a76a3-344">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-344">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="a76a3-345">Alterações não interruptivas adicionadas: Funcionalidade PeerAddressType para Peering Privado em "Remove-AzExpressRouteCircutPeeringConfig".</span><span class="sxs-lookup"><span data-stu-id="a76a3-345">Added non-breaking changes: PeerAddressType functionality for Private Peering in 'Remove-AzExpressRouteCircutPeeringConfig'.</span></span>
* <span data-ttu-id="a76a3-346">Código alterado para ignorar caso dos parâmetros AddressPrefixType e PeerAddressType.</span><span class="sxs-lookup"><span data-stu-id="a76a3-346">Code changed to ignore case for AddressPrefixType and PeerAddressType parameter.</span></span>
* <span data-ttu-id="a76a3-347">Foi modificada a mensagem de aviso de "New-AzLoadBalancerFrontendIpConfig", "New-AzPublicIpAddress" e "New-AzPublicIpPrefix".</span><span class="sxs-lookup"><span data-stu-id="a76a3-347">Modified the warning message for 'New-AzLoadBalancerFrontendIpConfig', 'New-AzPublicIpAddress' and 'New-AzPublicIpPrefix'.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-348">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-348">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-349">Opção "-ForceDelete" adicionada para "Remove-AzOperationalInsightsworkspace"</span><span class="sxs-lookup"><span data-stu-id="a76a3-349">Added '-ForceDelete' option for 'Remove-AzOperationalInsightsworkspace'</span></span>
* <span data-ttu-id="a76a3-350">Novo cmdlet "Get-AzOperationalInsightsDeletedWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="a76a3-350">Added new cmdlet 'Get-AzOperationalInsightsDeletedWorkspace'</span></span>
* <span data-ttu-id="a76a3-351">Novo cmdlet "Restore-AzOperationalInsightsWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="a76a3-351">Added new cmdlet 'Restore-AzOperationalInsightsWorkspace'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-352">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-352">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-353">Experiência de deteção de contentores/itens do Azure Backup melhorada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-353">Improved the Azure Backup container/item discovery experience.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-354">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-354">Az.Resources</span></span>
* <span data-ttu-id="a76a3-355">Propriedades "Condition", "ConditionVersion" e "Description" adicionadas a "New-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-355">Added properties 'Condition', 'ConditionVersion' and 'Description' to 'New-AzRoleAssignment'</span></span>
    - <span data-ttu-id="a76a3-356">Isto incluiu todas as alterações relevantes aos modelos de dados</span><span class="sxs-lookup"><span data-stu-id="a76a3-356">This included all the relevant changes to the data models</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-357">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-357">Az.Sql</span></span>
* <span data-ttu-id="a76a3-358">Foi corrigido o potencial erro de nome do servidor não sensível a maiúsculas e minúsculas em "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-358">Fixed potential server name case insensitive error in 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="a76a3-359">Foi corrigido o erro em que era devolvido um nome de base de dados incorreto numa base de dados existente em "New-AzSqlDatabaseSecondary"</span><span class="sxs-lookup"><span data-stu-id="a76a3-359">Fixed wrong database name returned on existing database error in 'New-AzSqlDatabaseSecondary'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-360">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-360">Az.Storage</span></span>
* <span data-ttu-id="a76a3-361">Criação de tokens de SAS de contentores/blobs suportada com nova permissão x,t</span><span class="sxs-lookup"><span data-stu-id="a76a3-361">Supported create container/blob Sas token with new permission x,t</span></span>
    -  <span data-ttu-id="a76a3-362">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="a76a3-362">'New-AzStorageBlobSASToken'</span></span>
    -  <span data-ttu-id="a76a3-363">"New-AzStorageContainerSASToken"</span><span class="sxs-lookup"><span data-stu-id="a76a3-363">'New-AzStorageContainerSASToken'</span></span>
* <span data-ttu-id="a76a3-364">Criação de tokens de SAS de contas suportada com nova permissão x,t,f</span><span class="sxs-lookup"><span data-stu-id="a76a3-364">Supported create account Sas token with new permission x,t,f</span></span>
    -  <span data-ttu-id="a76a3-365">"New-AzStorageAccountSASToken"</span><span class="sxs-lookup"><span data-stu-id="a76a3-365">'New-AzStorageAccountSASToken'</span></span>
* <span data-ttu-id="a76a3-366">Obtenção da utilização de partilha de ficheiros única suportada</span><span class="sxs-lookup"><span data-stu-id="a76a3-366">Supported get single file share usage</span></span>
    - <span data-ttu-id="a76a3-367">"Get-AzRmStorageShare"</span><span class="sxs-lookup"><span data-stu-id="a76a3-367">'Get-AzRmStorageShare'</span></span>

## <a name="440---july-2020"></a><span data-ttu-id="a76a3-368">4.4.0 - Julho de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-368">4.4.0 - July 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-369">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-369">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-370">Adição do novo cmdlet "Invoke-AzRestMethod"</span><span class="sxs-lookup"><span data-stu-id="a76a3-370">Added new cmdlet 'Invoke-AzRestMethod'</span></span>
* <span data-ttu-id="a76a3-371">Correção de um problema que pode causar erros de autenticação em cenários de vários processos, tais como executar vários cmdlets do Azure PowerShell utilizando "Start-Job" [#9448]</span><span class="sxs-lookup"><span data-stu-id="a76a3-371">Fixed an issue that may cause authentication errors in multi-process scenarios such as running multiple Azure PowerShell cmdlets using 'Start-Job' [#9448]</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-372">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-372">Az.Aks</span></span>
* <span data-ttu-id="a76a3-373">Correção do erro "Get-AzAks" uma vez que não recebe todos os clusters [#12296]</span><span class="sxs-lookup"><span data-stu-id="a76a3-373">Fixed bug 'Get-AzAks' doesn't get all clusters [#12296]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a76a3-374">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-374">Az.AnalysisServices</span></span>
* <span data-ttu-id="a76a3-375">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="a76a3-375">Removed project reference to Authentication</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-376">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-376">Az.Automation</span></span>
* <span data-ttu-id="a76a3-377">Correção do problema em que a cadeia com chars de fuga não pode ser convertida num objeto json.</span><span class="sxs-lookup"><span data-stu-id="a76a3-377">Fixed the issue that string with escape chars cannot be converted into json object.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-378">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-378">Az.Compute</span></span>
* <span data-ttu-id="a76a3-379">Adição do aviso ao utilizar "New-AzVmss" sem a versão de imagem "mais recente"</span><span class="sxs-lookup"><span data-stu-id="a76a3-379">Added warning when using 'New-AzVmss' without 'latest' image version</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-380">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-380">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-381">Adição de parâmetros globais ao Data Factory.</span><span class="sxs-lookup"><span data-stu-id="a76a3-381">Added global parameters to Data Factory.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a76a3-382">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a76a3-382">Az.EventGrid</span></span>
* <span data-ttu-id="a76a3-383">Atualização para utilizar a versão de API 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-383">Updated to use the 2020-06-01 API version.</span></span>
* <span data-ttu-id="a76a3-384">Novas funcionalidades adicionadas:</span><span class="sxs-lookup"><span data-stu-id="a76a3-384">Added new features:</span></span>
    - <span data-ttu-id="a76a3-385">Mapeamento de entrada</span><span class="sxs-lookup"><span data-stu-id="a76a3-385">Input mapping</span></span>
    - <span data-ttu-id="a76a3-386">Esquema de Entrega de Eventos</span><span class="sxs-lookup"><span data-stu-id="a76a3-386">Event Delivery Schema</span></span>
    - <span data-ttu-id="a76a3-387">Ligação Privada</span><span class="sxs-lookup"><span data-stu-id="a76a3-387">Private Link</span></span>
    - <span data-ttu-id="a76a3-388">Esquema de Eventos na Cloud V10</span><span class="sxs-lookup"><span data-stu-id="a76a3-388">Cloud Event V10 Schema</span></span>
    - <span data-ttu-id="a76a3-389">Tópico do Service Bus como Destino</span><span class="sxs-lookup"><span data-stu-id="a76a3-389">Service Bus Topic As Destination</span></span>
    - <span data-ttu-id="a76a3-390">Função do Azure como Destino</span><span class="sxs-lookup"><span data-stu-id="a76a3-390">Azure Function As Destination</span></span>
    - <span data-ttu-id="a76a3-391">Criação de batches do WebHook</span><span class="sxs-lookup"><span data-stu-id="a76a3-391">WebHook Batching</span></span>
    - <span data-ttu-id="a76a3-392">Webhook seguro (suporte de AAD)</span><span class="sxs-lookup"><span data-stu-id="a76a3-392">Secure webhook (AAD support)</span></span>
    - <span data-ttu-id="a76a3-393">IpFiltering</span><span class="sxs-lookup"><span data-stu-id="a76a3-393">IpFiltering</span></span>
* <span data-ttu-id="a76a3-394">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="a76a3-394">Updated cmdlets:</span></span>
    - <span data-ttu-id="a76a3-395">"New-AzEventGridSubscription"/"Update-AzEventGridSubscription":</span><span class="sxs-lookup"><span data-stu-id="a76a3-395">'New-AzEventGridSubscription'/'Update-AzEventGridSubscription':</span></span>
        - <span data-ttu-id="a76a3-396">Adicionar novos parâmetros opcionais para suportar a criação de batches do webhook.</span><span class="sxs-lookup"><span data-stu-id="a76a3-396">Add new optional parameters to support webhook batching.</span></span>
        - <span data-ttu-id="a76a3-397">Adicionar novos parâmetros opcionais para suportar o webhook seguro através do AAD.</span><span class="sxs-lookup"><span data-stu-id="a76a3-397">Add new optional parameters to support secured webhook using AAD.</span></span>
        - <span data-ttu-id="a76a3-398">Adicionar uma nova enumeração para o parâmetro EndpointType para suportar a função do Azure e o tópico do Service Bus enquanto novos destinos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-398">Add new enum for EndpointType parameter to support azure function and service bus topic as new destinations.</span></span>
        - <span data-ttu-id="a76a3-399">Adicionar novo parâmetro opcional para o esquema de entrega.</span><span class="sxs-lookup"><span data-stu-id="a76a3-399">Add new optional parameter for delivery schema.</span></span>
    - <span data-ttu-id="a76a3-400">"New-AzEventGridTopic"/"Update-AzEventGridTopic" e "New-AzEventGridDomain"/"Update-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="a76a3-400">'New-AzEventGridTopic'/'Update-AzEventGridTopic' and 'New-AzEventGridDomain'/'Update-AzEventGridDomain':</span></span>
        - <span data-ttu-id="a76a3-401">Adicionar novos parâmetros opcionais para suportar IpFiltering.</span><span class="sxs-lookup"><span data-stu-id="a76a3-401">Add new optional parameters to support IpFiltering.</span></span>
    - <span data-ttu-id="a76a3-402">"New-AzEventGridTopic"/"New-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="a76a3-402">'New-AzEventGridTopic'/'New-AzEventGridDomain':</span></span>
        - <span data-ttu-id="a76a3-403">Adicionar novos parâmetros opcionais para suportar o Mapeamento de entrada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-403">Add new optional parameters to support Input mapping.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-404">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-404">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-405">Módulo atualizado para utilizar a API 2020-05-01</span><span class="sxs-lookup"><span data-stu-id="a76a3-405">Updated module to use API 2020-05-01</span></span>
* <span data-ttu-id="a76a3-406">Adição de suporte do Private Link para recursos de Armazenamento, Cofre de chaves e Serviço de Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="a76a3-406">Added Private link support for Storage, Keyvault and Web App Service resources</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-407">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-407">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-408">Suporte para a criação de cluster com armazenamento ADLSGen1/2 em clouds nacionais.</span><span class="sxs-lookup"><span data-stu-id="a76a3-408">Supported creating cluster with ADLSGen1/2 storage in national clouds.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-409">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-409">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-410">Correção do erro em "Get-AzDiagnosticSetting" quando as métricas ou registos são nulos [#12272]</span><span class="sxs-lookup"><span data-stu-id="a76a3-410">Fixed bug for 'Get-AzDiagnosticSetting' when metrics or logs are null [#12272]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-411">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-411">Az.Network</span></span>
* <span data-ttu-id="a76a3-412">Correção da troca de parâmetros na ligação VWan HubVnet</span><span class="sxs-lookup"><span data-stu-id="a76a3-412">Fixed parameters swap in VWan HubVnet connection</span></span>
* <span data-ttu-id="a76a3-413">Adição de novos cmdlets para Sites de Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-413">Added new cmdlets for Azure Network Virtual Appliance Sites</span></span>
    - <span data-ttu-id="a76a3-414">"Get-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="a76a3-414">'Get-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="a76a3-415">"New-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="a76a3-415">'New-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="a76a3-416">"Remove-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="a76a3-416">'Remove-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="a76a3-417">"Update-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="a76a3-417">'Update-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="a76a3-418">"New-AzOffice365PolicyProperty"</span><span class="sxs-lookup"><span data-stu-id="a76a3-418">'New-AzOffice365PolicyProperty'</span></span>
* <span data-ttu-id="a76a3-419">Adição de novos cmdlets para Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-419">Added new cmdlets for Azure Network Virtual Appliance</span></span>
    - <span data-ttu-id="a76a3-420">"Get-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="a76a3-420">'Get-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="a76a3-421">"New-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="a76a3-421">'New-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="a76a3-422">"Remove-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="a76a3-422">'Remove-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="a76a3-423">"Update-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="a76a3-423">'Update-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="a76a3-424">"Get-AzNetworkVirtualApplianceSku"</span><span class="sxs-lookup"><span data-stu-id="a76a3-424">'Get-AzNetworkVirtualApplianceSku'</span></span>
    - <span data-ttu-id="a76a3-425">"New-AzVirtualApplianceSkuProperty"</span><span class="sxs-lookup"><span data-stu-id="a76a3-425">'New-AzVirtualApplianceSkuProperty'</span></span>
* <span data-ttu-id="a76a3-426">Gateway de Aplicação integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="a76a3-426">Onboarded Application Gateway to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="a76a3-427">StorageSync integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="a76a3-427">Onboarded StorageSync to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="a76a3-428">SignalR integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="a76a3-428">Onboarded SignalR to Private Link Common Cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-429">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-429">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-430">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="a76a3-430">Removed project reference to Authentication</span></span>
* <span data-ttu-id="a76a3-431">Os cmdlets afinados do Azure Backup ajudam o texto a ser mais preciso.</span><span class="sxs-lookup"><span data-stu-id="a76a3-431">Azure Backup tuned cmdlets help text to be more accurate.</span></span>
* <span data-ttu-id="a76a3-432">O Azure Backup adicionou suporte para obter tarefas de agentes MAB através do cmdlet "Get-AzRecoveryServicesBackupJob".</span><span class="sxs-lookup"><span data-stu-id="a76a3-432">Azure Backup added support for fetching MAB agent jobs using 'Get-AzRecoveryServicesBackupJob' cmdlet.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-433">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-433">Az.Resources</span></span>
* <span data-ttu-id="a76a3-434">Atualização de "Save-AzResourceGroupDeploymentTemplate" para utilizar o SDK.</span><span class="sxs-lookup"><span data-stu-id="a76a3-434">Updated 'Save-AzResourceGroupDeploymentTemplate' to use the SDK.</span></span>
* <span data-ttu-id="a76a3-435">Adição do cmdlet "Unregister-AzResourceProvider".</span><span class="sxs-lookup"><span data-stu-id="a76a3-435">Added 'Unregister-AzResourceProvider' cmdlet.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-436">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-436">Az.Sql</span></span>
* <span data-ttu-id="a76a3-437">Adição de suporte para o Principal de serviço e utilizadores convidados no cmdlet Set-AzSqlInstanceActiveDirectoryAdministrator</span><span class="sxs-lookup"><span data-stu-id="a76a3-437">Added support for Service principal and guest users in Set-AzSqlInstanceActiveDirectoryAdministrator cmdlet'</span></span>
* <span data-ttu-id="a76a3-438">Correção de um erro em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-438">Fixed a bug in Data Classification cmdlets.'</span></span>
* <span data-ttu-id="a76a3-439">Adição de suporte para a ativação pós-falha do Azure SQL Managed Instance: "Invoke-AzSqlInstanceFailover"</span><span class="sxs-lookup"><span data-stu-id="a76a3-439">Added support for Azure SQL Managed Instance failover: 'Invoke-AzSqlInstanceFailover'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-440">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-440">Az.Storage</span></span>
* <span data-ttu-id="a76a3-441">Correção do erro de que o UserAgent não é adicionado para alguns cmdlets do plano de dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-441">Fixed the issue that UserAgent is not added for some data plane cmdlets.</span></span>
* <span data-ttu-id="a76a3-442">Suporte para a criação/atualização da Conta de armazenamento com MinimumTlsVersion e AllowBlobPublicAccess</span><span class="sxs-lookup"><span data-stu-id="a76a3-442">Supported create/update Storage account with MinimumTlsVersion and AllowBlobPublicAccess</span></span>
    -  <span data-ttu-id="a76a3-443">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-443">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="a76a3-444">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-444">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="a76a3-445">Suporte para Permitir/desativar o controlo de versões no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-445">Support enable/disable versioning on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="a76a3-446">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="a76a3-446">'Update-AzStorageBlobServiceProperty'</span></span>
* <span data-ttu-id="a76a3-447">Suporte para a lista de blobs com versões de blobs</span><span class="sxs-lookup"><span data-stu-id="a76a3-447">Support list blobs with blob versions</span></span>
    - <span data-ttu-id="a76a3-448">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="a76a3-448">'Get-AzStorageBlob'</span></span>
* <span data-ttu-id="a76a3-449">Suporte para obter/remover instantâneo de blob único ou versão do blob</span><span class="sxs-lookup"><span data-stu-id="a76a3-449">Support get/remove single blob snapshot or blob version</span></span>
    - <span data-ttu-id="a76a3-450">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="a76a3-450">'Get-AzStorageBlob'</span></span>
    - <span data-ttu-id="a76a3-451">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="a76a3-451">'Remove-AzStorageBlob'</span></span>
* <span data-ttu-id="a76a3-452">Suporte para pipeline a partir do objeto de blob gerado a partir de Azure.Storage.Blobs V12</span><span class="sxs-lookup"><span data-stu-id="a76a3-452">Support pipeline from blob object generated from Azure.Storage.Blobs V12</span></span>
    - <span data-ttu-id="a76a3-453">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-453">'Get-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="a76a3-454">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="a76a3-454">'New-AzStorageBlobSASToken'</span></span>
    - <span data-ttu-id="a76a3-455">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="a76a3-455">'Remove-AzStorageBlob'</span></span>
    - <span data-ttu-id="a76a3-456">"Set-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-456">'Set-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="a76a3-457">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-457">'Start-AzStorageBlobCopy'</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a76a3-458">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a76a3-458">Az.StorageSync</span></span>
* <span data-ttu-id="a76a3-459">Adição de uma nova versão StorageSync SDK para ApiVersion 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="a76a3-459">Added a new version StorageSync SDK targeting ApiVersion 2020-03-01</span></span>
* <span data-ttu-id="a76a3-460">Adição de cmdlet do Serviço de Sincronização de Armazenamento de Atualização</span><span class="sxs-lookup"><span data-stu-id="a76a3-460">Added Update Storage Sync Service cmdlet</span></span>
    - <span data-ttu-id="a76a3-461">"Set-AzStorageSyncService"</span><span class="sxs-lookup"><span data-stu-id="a76a3-461">'Set-AzStorageSyncService'</span></span>
* <span data-ttu-id="a76a3-462">Adição de IncomingTrafficPolicy e PrivateEndpointConnections para cmdlets StorageSyncService.</span><span class="sxs-lookup"><span data-stu-id="a76a3-462">Added IncomingTrafficPolicy and PrivateEndpointConnections to StorageSyncService cmdlets.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-463">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-463">Az.Websites</span></span>
* <span data-ttu-id="a76a3-464">Adição de suporte para a realização de operações para Slots em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="a76a3-464">Added support to perform operations for Slots not in the same resource group as the App Service Plan</span></span>

## <a name="430---june-2020"></a><span data-ttu-id="a76a3-465">4.3.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-465">4.3.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-466">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-467">Suporte para a deteção da definição do ambiente por predefinição e adição de ambiente através de "Add-AzEnvironment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-467">Supported discovering environment setting by default and adding environment via 'Add-AzEnvironment'</span></span>
* <span data-ttu-id="a76a3-468">Atualizar assemblagens pré-carregadas [#12024], [#11976]</span><span class="sxs-lookup"><span data-stu-id="a76a3-468">Update preloaded assemblies [#12024], [#11976]</span></span>
* <span data-ttu-id="a76a3-469">Atualização da assemblagem Azure.Core</span><span class="sxs-lookup"><span data-stu-id="a76a3-469">Updated Azure.Core assembly</span></span>
* <span data-ttu-id="a76a3-470">Correção de um problema que pode provocar a falha de "Connect-AzAccount" numa execução de múltiplos threads [#11201]</span><span class="sxs-lookup"><span data-stu-id="a76a3-470">Fixed an issue that may cause 'Connect-AzAccount' to fail in multi-threaded execution [#11201]</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-471">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-471">Az.Aks</span></span>
* <span data-ttu-id="a76a3-472">Substituição da utilização da [API AccessProfile](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) antiga por chamadas para as APIs [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) e [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials)</span><span class="sxs-lookup"><span data-stu-id="a76a3-472">Replaced usage of old [AccessProfile API](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) with calls to [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) and [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials) APIs</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-473">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-473">Az.Batch</span></span>
* <span data-ttu-id="a76a3-474">Atualização da versão do SDK de Az.Batch para utilizar "Microsoft.Azure.Management.Batch" para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-474">Updated Az.Batch to use 'Microsoft.Azure.Management.Batch' SDK version to 11.0.0</span></span>
* <span data-ttu-id="a76a3-475">Adição da capacidade de definir a Identidade BatchAccount no cmdlet "New-AzBatchAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-475">Added the ability to set the BatchAccount Identity in the 'New-AzBatchAccount' cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-476">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-476">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-477">Suporte para a apresentação das capacidades da conta.</span><span class="sxs-lookup"><span data-stu-id="a76a3-477">Supported displaying account capabilities.</span></span>
* <span data-ttu-id="a76a3-478">Suporte para a modificação de PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="a76a3-478">Supported modifying PublicNetworkAccess.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-479">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-479">Az.Compute</span></span>
* <span data-ttu-id="a76a3-480">Adição do parâmetro SimulateEviction aos cmdlets Set-AzVM e Set-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="a76a3-480">Added SimulateEviction parameter to Set-AzVM and Set-AzVmssVM cmdlets.</span></span>
* <span data-ttu-id="a76a3-481">Adição de "Premium_LRS" ao mecanismo de preenchimento de argumentos do parâmetro StorageAccountType para o cmdlet New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="a76a3-481">Added 'Premium_LRS' to the argument completer of StorageAccountType parameter for New-AzGalleryImageVersion cmdlet.</span></span>
* <span data-ttu-id="a76a3-482">Adição de subestados a VMCustomScriptExtension [#11297]</span><span class="sxs-lookup"><span data-stu-id="a76a3-482">Added Substatuses to VMCustomScriptExtension [#11297]</span></span>
* <span data-ttu-id="a76a3-483">Adição de "Delete" ao mecanismo de preenchimento de argumentos do parâmetro EvictionPolicy para os cmdlets New-AzVM e New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="a76a3-483">Added 'Delete' to the argument completer of EvictionPolicy parameter for New-AzVM and New-AzVMConfig cmdlets.</span></span>
* <span data-ttu-id="a76a3-484">Correção do nome da nova Extensão de VM para SAP</span><span class="sxs-lookup"><span data-stu-id="a76a3-484">Fixed name of new VM Extension for SAP</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-485">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-485">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-486">Atualização da versão do SDK de .Net do ADF para 4.9.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-486">Updated ADF .Net SDK version to 4.9.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-487">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-487">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-488">Adição de parâmetros de Identidade Gerida aos cmdlets "New-AzEventHubNamespace" e "Set-AzEventHubNamespace"</span><span class="sxs-lookup"><span data-stu-id="a76a3-488">Added Managed Identity parameters to 'New-AzEventHubNamespace' and 'Set-AzEventHubNamespace' cmdlets</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="a76a3-489">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="a76a3-489">Az.Functions</span></span>
* <span data-ttu-id="a76a3-490">Adição de suporte para a criação de aplicações de funções do PowerShell 7.0 e de Java 11</span><span class="sxs-lookup"><span data-stu-id="a76a3-490">Added support to create PowerShell 7.0 and Java 11 function apps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-491">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-491">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-492">Suporte para listagem de anfitriões e reinício de anfitriões específicos do cluster HDInsight.</span><span class="sxs-lookup"><span data-stu-id="a76a3-492">Supported listing hosts and restart specific hosts of the HDInsight cluster.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="a76a3-493">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="a76a3-493">Az.HealthcareApis</span></span>
* <span data-ttu-id="a76a3-494">Atualização da versão do SDK para 1.1.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-494">Updated the SDK version to 1.1.0</span></span>
* <span data-ttu-id="a76a3-495">Adição de suporte para as definições de Exportação e a Identidade Gerida</span><span class="sxs-lookup"><span data-stu-id="a76a3-495">Added support for Export settings and Managed Identity</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-496">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-496">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-497">Correção do parâmetro de objeto de entrada para "Set-AzActivityLogAlert"</span><span class="sxs-lookup"><span data-stu-id="a76a3-497">Fixed input object parameter for 'Set-AzActivityLogAlert'</span></span>
* <span data-ttu-id="a76a3-498">Correção do parâmetro "InputObject" para "Set-AzActionGroup" [#10868]</span><span class="sxs-lookup"><span data-stu-id="a76a3-498">Fixed 'InputObject' parameter for 'Set-AzActionGroup' [#10868]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-499">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-499">Az.Network</span></span>
* <span data-ttu-id="a76a3-500">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-500">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="a76a3-501">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-501">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="a76a3-502">"New-AzFirewallPolicyDnsSetting"</span><span class="sxs-lookup"><span data-stu-id="a76a3-502">'New-AzFirewallPolicyDnsSetting'</span></span>
    - <span data-ttu-id="a76a3-503">Suporte para FQDN de Destino nas Regras de Rede para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-503">Support for Destination FQDN in Network Rules for Firewall Policy</span></span>
* <span data-ttu-id="a76a3-504">Adição de suporte para operações de conjuntos de endereços back-end</span><span class="sxs-lookup"><span data-stu-id="a76a3-504">Added support for backend address pool operations</span></span>
    - <span data-ttu-id="a76a3-505">"New-AzLoadBalancerBackendAddressConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-505">'New-AzLoadBalancerBackendAddressConfig'</span></span>
    - <span data-ttu-id="a76a3-506">"New-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="a76a3-506">'New-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="a76a3-507">"Set-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="a76a3-507">'Set-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="a76a3-508">"Remove-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="a76a3-508">'Remove-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="a76a3-509">"Get-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="a76a3-509">'Get-AzLoadBalancerBackendAddressPool'</span></span>
* <span data-ttu-id="a76a3-510">Adição de validação de nomes para "New-AzIpGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-510">Added name validation for 'New-AzIpGroup'</span></span>
* <span data-ttu-id="a76a3-511">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-511">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="a76a3-512">"New-AzFirewallPolicyThreatIntelWhitelist"</span><span class="sxs-lookup"><span data-stu-id="a76a3-512">'New-AzFirewallPolicyThreatIntelWhitelist'</span></span>
* <span data-ttu-id="a76a3-513">Foram atualizados os seguintes comandos para a funcionalidade: Definição/remoção de servidores DNS personalizados no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="a76a3-513">Updated below commands for feature: Custom dns servers set/remove on VirtualWan P2SVpnGateway.</span></span>
    - <span data-ttu-id="a76a3-514">Atualização de New-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="a76a3-514">Updated New-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
    - <span data-ttu-id="a76a3-515">Atualização de Update-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="a76a3-515">Updated Update-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
* <span data-ttu-id="a76a3-516">Atualização de "Update-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-516">Updated 'Update-AzVpnGateway'</span></span>
    - <span data-ttu-id="a76a3-517">Adição do parâmetro opcional "-BgpPeeringAddress" para os clientes especificarem os respetivos bgps personalizados a definir no VpnGateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-517">Added optional parameter '-BgpPeeringAddress' for customers to specify their custom bgps to set on VpnGateway.</span></span>
* <span data-ttu-id="a76a3-518">Adição de novo cmdlet para suportar a reposição do estado de encaminhamento de um recurso VirtualHub:</span><span class="sxs-lookup"><span data-stu-id="a76a3-518">Added new cmdlet to support resetting the routing state of a VirtualHub resource:</span></span>
    - <span data-ttu-id="a76a3-519">"Reset-AzHubRouter"</span><span class="sxs-lookup"><span data-stu-id="a76a3-519">'Reset-AzHubRouter'</span></span>
* <span data-ttu-id="a76a3-520">Atualização dos elementos indicados abaixo com base na alteração recente de Swagger para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-520">Updated below things based on recent swagger change for Firewall Policy</span></span>
    - <span data-ttu-id="a76a3-521">Alteração de nomes para RuleGroup, RuleCollectionGroup e RuleType</span><span class="sxs-lookup"><span data-stu-id="a76a3-521">Changes names for RuleGroup, RuleCollectionGroup and RuleType</span></span>
    - <span data-ttu-id="a76a3-522">Adição de suporte para Coleções de Regras de NAT da Política de Firewall para suportar várias Coleções de Regras de NAT</span><span class="sxs-lookup"><span data-stu-id="a76a3-522">Added support for Firewall Policy NAT Rule Collections to support multiple NAT Rule Collection</span></span>
* <span data-ttu-id="a76a3-523">[Alteração Interruptiva] Adição do parâmetro obrigatório "SourceIpGroup" para "New-AzFirewallPolicyApplicationRule" e "New-AzFirewallPolicyNetworkRule".</span><span class="sxs-lookup"><span data-stu-id="a76a3-523">[Breaking Change] Added mandatory parameter 'SourceIpGroup' for 'New-AzFirewallPolicyApplicationRule' and 'New-AzFirewallPolicyNetworkRule'.</span></span>
* <span data-ttu-id="a76a3-524">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a76a3-524">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="a76a3-525">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a76a3-525">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="a76a3-526">[Alteração Interruptiva] Remoção de parâmetros obrigatórios: "TranslatedAddress", "TranslatedPort" para "New-AzFirewallPolicyNatRuleCollection".</span><span class="sxs-lookup"><span data-stu-id="a76a3-526">[Breaking Change] Removed mandatory parameters: 'TranslatedAddress', 'TranslatedPort' for 'New-AzFirewallPolicyNatRuleCollection'.</span></span>
* <span data-ttu-id="a76a3-527">Adição de novos cmdlets para suportar PrivateLink no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-527">Added new cmdlets to support PrivateLink On Application Gateway</span></span>
    - <span data-ttu-id="a76a3-528">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-528">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="a76a3-529">"Get-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-529">'Get-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="a76a3-530">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-530">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="a76a3-531">"Set-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-531">'Set-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="a76a3-532">"Remove-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-532">'Remove-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="a76a3-533">"New-AzApplicationGatewayPrivateLinkIpConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-533">'New-AzApplicationGatewayPrivateLinkIpConfiguration'</span></span>
* <span data-ttu-id="a76a3-534">Adição de novos cmdlets para o recurso subordinado HubRouteTables de VirtualHub.</span><span class="sxs-lookup"><span data-stu-id="a76a3-534">Added new cmdlets for HubRouteTables child resource of VirtualHub.</span></span>
    - <span data-ttu-id="a76a3-535">"New-AzVHubRoute"</span><span class="sxs-lookup"><span data-stu-id="a76a3-535">'New-AzVHubRoute'</span></span>
    - <span data-ttu-id="a76a3-536">"New-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="a76a3-536">'New-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="a76a3-537">"Get-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="a76a3-537">'Get-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="a76a3-538">"Update-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="a76a3-538">'Update-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="a76a3-539">"Remove-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="a76a3-539">'Remove-AzVHubRouteTable'</span></span>
* <span data-ttu-id="a76a3-540">Atualização dos cmdlets existentes para suportar o parâmetro de entrada opcional RoutingConfiguration para encaminhamento personalizado em VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="a76a3-540">Updated existing cmdlets to support optional RoutingConfiguration input parameter for custom routing in VirtualWan.</span></span>
    - <span data-ttu-id="a76a3-541">"New-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-541">'New-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="a76a3-542">"Set-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-542">'Set-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="a76a3-543">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-543">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="a76a3-544">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-544">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="a76a3-545">"New-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-545">'New-AzVpnConnection'</span></span>
    - <span data-ttu-id="a76a3-546">"Update-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-546">'Update-AzVpnConnection'</span></span>
    - <span data-ttu-id="a76a3-547">"New-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-547">'New-AzP2sVpnGateway'</span></span>
    - <span data-ttu-id="a76a3-548">"Update-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-548">'Update-AzP2sVpnGateway'</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-549">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-549">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-550">Correção do erro PSWorkspace não implementa IOperationalInsightsWorkspace [#12135]</span><span class="sxs-lookup"><span data-stu-id="a76a3-550">Fixed bug PSWorkspace doesn't implement IOperationalInsightsWorkspace [#12135]</span></span>
* <span data-ttu-id="a76a3-551">Adição de "pergb2018" ao conjunto de valores válidos do parâmetro "Sku" em "Set-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="a76a3-551">Added 'pergb2018' to valid value set of parameter 'Sku' in 'Set-AzOperationalInsightsWorkspace'</span></span> 
* <span data-ttu-id="a76a3-552">Adição do alias "FunctionParameters" para o parâmetro "FunctionParameter" a</span><span class="sxs-lookup"><span data-stu-id="a76a3-552">Added alias 'FunctionParameters' for parameter 'FunctionParameter' to</span></span>
    - <span data-ttu-id="a76a3-553">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="a76a3-553">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="a76a3-554">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="a76a3-554">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-555">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-555">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-556">Adição de suporte no Azure Backup para a obtenção de itens de MAB.</span><span class="sxs-lookup"><span data-stu-id="a76a3-556">Azure Backup added support for fetching MAB items.</span></span>
* <span data-ttu-id="a76a3-557">Suporte do Azure Site Recovery para o tipo de disco "StandardSSD_LRS"</span><span class="sxs-lookup"><span data-stu-id="a76a3-557">Azure Site Recovery supports disk type 'StandardSSD_LRS'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-558">Az.Resources</span></span>
* <span data-ttu-id="a76a3-559">Adição de "UsageLocation", "GivenName", "Surname", "AccountEnabled", "MailNickname", "Mail" em "PSADUser" [#10526] [#10497]</span><span class="sxs-lookup"><span data-stu-id="a76a3-559">Added 'UsageLocation', 'GivenName', 'Surname', 'AccountEnabled', 'MailNickname', 'Mail' on 'PSADUser' [#10526] [#10497]</span></span>
* <span data-ttu-id="a76a3-560">Correção do problema em que "-Mail" não funciona em "Get-AzADUser" [#11981]</span><span class="sxs-lookup"><span data-stu-id="a76a3-560">Fixed issue that '-Mail' doesn't work on 'Get-AzADUser' [#11981]</span></span>
* <span data-ttu-id="a76a3-561">Adição do parâmetro "-ExcludeChangeType" a "Get-AzDeploymentWhatIfResult" e "Get-AzResourceGroupDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="a76a3-561">Added '-ExcludeChangeType' parameter to 'Get-AzDeploymentWhatIfResult' and 'Get-AzResourceGroupDeploymentWhatIfResult'</span></span>
* <span data-ttu-id="a76a3-562">Adição do parâmetro "-WhatIfExcludeChangeType" a "New-AzDeployment" e "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-562">Added '-WhatIfExcludeChangeType' parameter to 'New-AzDeployment' and 'New-AzResourceGroupDeployment'</span></span>
* <span data-ttu-id="a76a3-563">Atualização de cmdlets "Test-Az\*Deployment" para apresentação de mensagens de erro melhores</span><span class="sxs-lookup"><span data-stu-id="a76a3-563">Updated 'Test-Az\*Deployment' cmdlets to show better error messages</span></span>
* <span data-ttu-id="a76a3-564">Correção da mensagem de ajuda para o parâmetro "-Name" de criação de implementação e cmdlets What-If</span><span class="sxs-lookup"><span data-stu-id="a76a3-564">Fixed help message for '-Name' parameter of deployment create and What-If cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-565">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-565">Az.Sql</span></span>
* <span data-ttu-id="a76a3-566">Adição de suporte para o principal de serviço para o cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="a76a3-566">Added support for service principal for Set SQL Server Azure Active Directory Admin cmdlet</span></span>
* <span data-ttu-id="a76a3-567">Correção de problema de sincronização em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-567">Fixed sync issue in Data Classification cmdlets.</span></span>
* <span data-ttu-id="a76a3-568">Suporte para a pesquisa de utilizador por correio em "Set-AzSqlServerActiveDirectoryAdministrator" [#12192]</span><span class="sxs-lookup"><span data-stu-id="a76a3-568">Supported searching user by mail on 'Set-AzSqlServerActiveDirectoryAdministrator' [#12192]</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-569">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-569">Az.Storage</span></span>
* <span data-ttu-id="a76a3-570">Suporte para a criação de Conta de armazenamento com RequireInfrastructureEncryption</span><span class="sxs-lookup"><span data-stu-id="a76a3-570">Supported create Storage account with RequireInfrastructureEncryption</span></span>
    -  <span data-ttu-id="a76a3-571">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-571">'New-AzStorageAccount'</span></span>
* <span data-ttu-id="a76a3-572">Mudança da lógica de carregamento de Azure.Core para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-572">Moved the logic of loading Azure.Core to Az.Accounts</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-573">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-573">Az.Websites</span></span>
* <span data-ttu-id="a76a3-574">Adição de salvaguarda para eliminar a aplicação Web criada em caso de falha do restauro em "Restore-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="a76a3-574">Added safeguard to delete created webapp if restore failed in 'Restore-AzDeletedWebApp'</span></span>
* <span data-ttu-id="a76a3-575">Adição de "SourceWebApp.Location" para "New-AzWebApp" e "New-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="a76a3-575">Added 'SourceWebApp.Location' for 'New-AzWebApp' and 'New-AzWebAppSlot'</span></span>
* <span data-ttu-id="a76a3-576">Correção do erro que impedia a alteração de definições de Contentor em "Set-AzWebApp" e "Set-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="a76a3-576">Fixed bug that prevented changing Container settings in 'Set-AzWebApp' and 'Set-AzWebAppSlot'</span></span>
* <span data-ttu-id="a76a3-577">Correção do erro para obter SiteConfig quando -Name não é fornecido para Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-577">Fixed bug to get SiteConfig when -Name is not given for Get-AzWebApp</span></span>
* <span data-ttu-id="a76a3-578">Adição de suporte para a criação de ASP para Aplicações Linux</span><span class="sxs-lookup"><span data-stu-id="a76a3-578">Added a support to create ASP for Linux Apps</span></span>
* <span data-ttu-id="a76a3-579">Adição de exceções para clonagem entre grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="a76a3-579">Added exceptions for clone across resource groups</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="a76a3-580">4.2.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-580">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-581">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-581">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-582">Correção de um problema que fazia com que o Az ignorasse registos nas tarefas da Automatização do Azure ou do PowerShell [#11492]</span><span class="sxs-lookup"><span data-stu-id="a76a3-582">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a76a3-583">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-583">Az.AnalysisServices</span></span>
* <span data-ttu-id="a76a3-584">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="a76a3-584">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-585">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-585">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-586">Atualização da versão de assemblagem dos cmdlets de gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="a76a3-586">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="a76a3-587">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a76a3-587">Az.Billing</span></span>
* <span data-ttu-id="a76a3-588">Atualização da versão de assemblagem dos cmdlets de consumo</span><span class="sxs-lookup"><span data-stu-id="a76a3-588">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-589">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-589">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-590">Suporte para o controlo de PrivateEndpoint e PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="a76a3-590">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-591">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-591">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-592">Atualização da versão de assemblagem dos cmdlets V2 de fábrica de dados</span><span class="sxs-lookup"><span data-stu-id="a76a3-592">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="a76a3-593">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-593">Az.DataShare</span></span>
* <span data-ttu-id="a76a3-594">Disponibilidade geral do módulo "Az.DataShare"</span><span class="sxs-lookup"><span data-stu-id="a76a3-594">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="a76a3-595">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="a76a3-595">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="a76a3-596">Disponibilidade geral do módulo "Az.DesktopVirtualization"</span><span class="sxs-lookup"><span data-stu-id="a76a3-596">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-597">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-597">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-598">Atualização do SDK para a versão 0.21.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-598">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="a76a3-599">Adição de parâmetros opcionais a</span><span class="sxs-lookup"><span data-stu-id="a76a3-599">Added optional parameters to</span></span> 
    - <span data-ttu-id="a76a3-600">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="a76a3-600">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="a76a3-601">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="a76a3-601">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-602">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-602">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-603">Correção do exemplo 3 de "Start-AzPolicyComplianceScan"</span><span class="sxs-lookup"><span data-stu-id="a76a3-603">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="a76a3-604">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a76a3-604">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="a76a3-605">Atualização da versão de assemblagem dos cmdlets do PowerBI</span><span class="sxs-lookup"><span data-stu-id="a76a3-605">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="a76a3-606">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="a76a3-606">Az.PrivateDns</span></span>
* <span data-ttu-id="a76a3-607">Correção da formatação da cadeia de saída verbosa de Remove-AzPrivateDnsRecordSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-607">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-608">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-608">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-609">Suporte do Azure Site Recovery para a criação de um plano de recuperação para replicação zona a zona a partir de uma entrada xml.</span><span class="sxs-lookup"><span data-stu-id="a76a3-609">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="a76a3-610">Atualização da versão de assemblagem dos cmdlets do SiteRecovery e Backup</span><span class="sxs-lookup"><span data-stu-id="a76a3-610">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-611">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-611">Az.Resources</span></span>
* <span data-ttu-id="a76a3-612">Adição do parâmetro Tail aos cmdlets Get-AzDeploymentScriptLog e Save-AzDeploymentScriptLog</span><span class="sxs-lookup"><span data-stu-id="a76a3-612">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="a76a3-613">Formatação da propriedade Output e apresentação da mesma na saída do cmdlet Get-AzDeploymentScript</span><span class="sxs-lookup"><span data-stu-id="a76a3-613">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="a76a3-614">Mudança de nome do parâmetro -DeploymentScriptInputObject para -DeploymentScriptObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-614">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="a76a3-615">Correção do nome em falta do ficheiro/destino nas mensagens de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="a76a3-615">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="a76a3-616">Atualização da versão de assemblagem dos cmdlets de gestor de recursos e de etiquetas</span><span class="sxs-lookup"><span data-stu-id="a76a3-616">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-617">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-617">Az.Sql</span></span>
* <span data-ttu-id="a76a3-618">Adição de UsePrivateLinkConnection a "New-AzSqlSyncGroup", "Update-AzSqlSyncGroup", "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="a76a3-618">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="a76a3-619">Adição de SyncMemberAzureDatabaseResourceId a "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="a76a3-619">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="a76a3-620">Adição do suporte de pesquisa de Utilizador convidado ao cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="a76a3-620">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-621">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-621">Az.Storage</span></span>
* <span data-ttu-id="a76a3-622">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="a76a3-622">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="a76a3-623">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-623">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="a76a3-624">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="a76a3-624">Highlights since the last release</span></span>
* <span data-ttu-id="a76a3-625">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="a76a3-625">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="a76a3-626">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="a76a3-626">General availability of Az.Functions</span></span> 
* <span data-ttu-id="a76a3-627">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="a76a3-627">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-628">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-628">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-629">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="a76a3-629">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="a76a3-630">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="a76a3-630">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-631">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-631">Az.Aks</span></span>
* <span data-ttu-id="a76a3-632">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="a76a3-632">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="a76a3-633">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="a76a3-633">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="a76a3-634">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="a76a3-634">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-635">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-635">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-636">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="a76a3-636">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="a76a3-637">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="a76a3-637">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="a76a3-638">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="a76a3-638">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="a76a3-639">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="a76a3-639">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="a76a3-640">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="a76a3-640">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="a76a3-641">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="a76a3-641">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="a76a3-642">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="a76a3-642">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="a76a3-643">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="a76a3-643">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="a76a3-644">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="a76a3-644">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="a76a3-645">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="a76a3-645">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="a76a3-646">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="a76a3-646">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="a76a3-647">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="a76a3-647">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="a76a3-648">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="a76a3-648">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="a76a3-649">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="a76a3-649">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="a76a3-650">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="a76a3-650">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="a76a3-651">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="a76a3-651">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="a76a3-652">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-652">Az.ApplicationInsights</span></span>
* <span data-ttu-id="a76a3-653">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="a76a3-653">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="a76a3-654">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="a76a3-654">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="a76a3-655">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="a76a3-655">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-656">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-656">Az.Batch</span></span>
* <span data-ttu-id="a76a3-657">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="a76a3-657">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="a76a3-658">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="a76a3-658">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="a76a3-659">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="a76a3-659">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="a76a3-660">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="a76a3-660">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="a76a3-661">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="a76a3-661">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="a76a3-662">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="a76a3-662">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="a76a3-663">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="a76a3-663">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="a76a3-664">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="a76a3-664">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="a76a3-665">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="a76a3-665">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-666">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-666">Az.Compute</span></span>
* <span data-ttu-id="a76a3-667">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="a76a3-667">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="a76a3-668">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-668">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="a76a3-669">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-669">Breaking changes</span></span>
    - <span data-ttu-id="a76a3-670">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="a76a3-670">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="a76a3-671">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="a76a3-671">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="a76a3-672">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="a76a3-672">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="a76a3-673">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="a76a3-673">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="a76a3-674">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="a76a3-674">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="a76a3-675">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="a76a3-675">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="a76a3-676">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="a76a3-676">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-677">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-677">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-678">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-678">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-679">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-679">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-680">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="a76a3-680">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="a76a3-681">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="a76a3-681">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="a76a3-682">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="a76a3-682">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="a76a3-683">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="a76a3-683">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="a76a3-684">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="a76a3-684">Az.Functions</span></span>
* <span data-ttu-id="a76a3-685">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="a76a3-685">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-686">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-686">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-687">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="a76a3-687">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="a76a3-688">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="a76a3-688">Az.HealthcareApis</span></span>
* <span data-ttu-id="a76a3-689">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="a76a3-689">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-690">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-690">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-691">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="a76a3-691">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="a76a3-692">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="a76a3-692">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="a76a3-693">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="a76a3-693">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="a76a3-694">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="a76a3-694">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="a76a3-695">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="a76a3-695">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="a76a3-696">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-696">New cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-697">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-697">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="a76a3-698">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-698">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="a76a3-699">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-699">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="a76a3-700">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-700">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="a76a3-701">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="a76a3-701">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="a76a3-702">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-702">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-703">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-703">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-704">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="a76a3-704">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="a76a3-705">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="a76a3-705">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="a76a3-706">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="a76a3-706">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="a76a3-707">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="a76a3-707">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="a76a3-708">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="a76a3-708">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="a76a3-709">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="a76a3-709">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="a76a3-710">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="a76a3-710">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-711">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-711">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-712">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="a76a3-712">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="a76a3-713">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="a76a3-713">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="a76a3-714">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="a76a3-714">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="a76a3-715">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="a76a3-715">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="a76a3-716">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="a76a3-716">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="a76a3-717">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="a76a3-717">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="a76a3-718">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="a76a3-718">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-719">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-719">Az.Network</span></span>
* <span data-ttu-id="a76a3-720">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="a76a3-720">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="a76a3-721">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="a76a3-721">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="a76a3-722">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="a76a3-722">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="a76a3-723">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-723">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="a76a3-724">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="a76a3-724">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="a76a3-725">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-725">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-726">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="a76a3-726">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="a76a3-727">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="a76a3-727">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="a76a3-728">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="a76a3-728">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="a76a3-729">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="a76a3-729">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="a76a3-730">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="a76a3-730">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="a76a3-731">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-731">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="a76a3-732">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="a76a3-732">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="a76a3-733">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="a76a3-733">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="a76a3-734">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="a76a3-734">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="a76a3-735">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="a76a3-735">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="a76a3-736">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-736">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="a76a3-737">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-737">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="a76a3-738">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-738">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="a76a3-739">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-739">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="a76a3-740">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-740">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="a76a3-741">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="a76a3-741">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="a76a3-742">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="a76a3-742">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="a76a3-743">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-743">Updated cmdlet:</span></span>
        - <span data-ttu-id="a76a3-744">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-744">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-745">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-745">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-746">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="a76a3-746">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="a76a3-747">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="a76a3-747">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="a76a3-748">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="a76a3-748">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="a76a3-749">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="a76a3-749">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="a76a3-750">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="a76a3-750">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="a76a3-751">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="a76a3-751">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="a76a3-752">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="a76a3-752">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="a76a3-753">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="a76a3-753">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-754">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-754">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-755">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-755">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="a76a3-756">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="a76a3-756">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="a76a3-757">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-757">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="a76a3-758">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="a76a3-758">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="a76a3-759">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a76a3-759">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-760">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-760">Az.Resources</span></span>
* <span data-ttu-id="a76a3-761">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="a76a3-761">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="a76a3-762">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="a76a3-762">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="a76a3-763">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="a76a3-763">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="a76a3-764">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="a76a3-764">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="a76a3-765">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="a76a3-765">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="a76a3-766">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="a76a3-766">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="a76a3-767">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="a76a3-767">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="a76a3-768">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="a76a3-768">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="a76a3-769">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="a76a3-769">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="a76a3-770">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="a76a3-770">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="a76a3-771">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="a76a3-771">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="a76a3-772">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="a76a3-772">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="a76a3-773">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="a76a3-773">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="a76a3-774">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="a76a3-774">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="a76a3-775">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="a76a3-775">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="a76a3-776">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="a76a3-776">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="a76a3-777">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-777">'New-AzDeployment'</span></span>
    - <span data-ttu-id="a76a3-778">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-778">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="a76a3-779">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-779">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="a76a3-780">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-780">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-781">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-781">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-782">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="a76a3-782">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-783">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-783">Az.Sql</span></span>
* <span data-ttu-id="a76a3-784">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="a76a3-784">Enhance performance of:</span></span>
    - <span data-ttu-id="a76a3-785">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="a76a3-785">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="a76a3-786">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="a76a3-786">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="a76a3-787">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="a76a3-787">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="a76a3-788">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="a76a3-788">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="a76a3-789">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="a76a3-789">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="a76a3-790">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="a76a3-790">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="a76a3-791">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="a76a3-791">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="a76a3-792">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="a76a3-792">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="a76a3-793">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-793">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="a76a3-794">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="a76a3-794">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-795">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-795">Az.Storage</span></span>
* <span data-ttu-id="a76a3-796">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-796">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="a76a3-797">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="a76a3-797">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="a76a3-798">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-798">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="a76a3-799">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="a76a3-799">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="a76a3-800">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="a76a3-800">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="a76a3-801">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="a76a3-801">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="a76a3-802">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-802">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="a76a3-803">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-803">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="a76a3-804">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="a76a3-804">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="a76a3-805">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-805">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="a76a3-806">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="a76a3-806">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="a76a3-807">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="a76a3-807">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="a76a3-808">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="a76a3-808">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="a76a3-809">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-809">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="a76a3-810">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-810">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="a76a3-811">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-811">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="a76a3-812">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-812">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="a76a3-813">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="a76a3-813">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="a76a3-814">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="a76a3-814">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="a76a3-815">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="a76a3-815">Supported failover Storage account</span></span>
    - <span data-ttu-id="a76a3-816">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="a76a3-816">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="a76a3-817">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="a76a3-817">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="a76a3-818">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="a76a3-818">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="a76a3-819">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="a76a3-819">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="a76a3-820">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="a76a3-820">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="a76a3-821">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="a76a3-821">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="a76a3-822">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="a76a3-822">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="a76a3-823">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-823">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="a76a3-824">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-824">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="a76a3-825">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-825">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="a76a3-826">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="a76a3-826">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="a76a3-827">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="a76a3-827">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="a76a3-828">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="a76a3-828">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="a76a3-829">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="a76a3-829">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="a76a3-830">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="a76a3-830">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="a76a3-831">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="a76a3-831">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="a76a3-832">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="a76a3-832">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="a76a3-833">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="a76a3-833">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="a76a3-834">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="a76a3-834">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="a76a3-835">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a76a3-835">Az.TrafficManager</span></span>
* <span data-ttu-id="a76a3-836">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="a76a3-836">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-837">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-837">Az.Websites</span></span>
* <span data-ttu-id="a76a3-838">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="a76a3-838">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="a76a3-839">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-839">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="a76a3-840">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="a76a3-840">Highlights since the last release</span></span>
* <span data-ttu-id="a76a3-841">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="a76a3-841">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-842">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-842">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-843">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="a76a3-843">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-844">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-844">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-845">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="a76a3-845">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="a76a3-846">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="a76a3-846">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-847">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-847">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-848">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="a76a3-848">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-849">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-849">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-850">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="a76a3-850">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-851">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-851">Az.Compute</span></span>
* <span data-ttu-id="a76a3-852">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="a76a3-852">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="a76a3-853">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="a76a3-853">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-854">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-854">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-855">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-855">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-856">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="a76a3-856">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="a76a3-857">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="a76a3-857">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="a76a3-858">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-858">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="a76a3-859">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-859">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-860">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="a76a3-860">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="a76a3-861">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="a76a3-861">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="a76a3-862">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="a76a3-862">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="a76a3-863">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-863">New cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-864">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-864">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="a76a3-865">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-865">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="a76a3-866">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-866">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="a76a3-867">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-867">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="a76a3-868">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-868">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-869">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-869">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-870">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="a76a3-870">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="a76a3-871">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="a76a3-871">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="a76a3-872">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="a76a3-872">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="a76a3-873">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="a76a3-873">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="a76a3-874">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="a76a3-874">Az.Maintenance</span></span>
* <span data-ttu-id="a76a3-875">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-875">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-876">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-876">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-877">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="a76a3-877">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="a76a3-878">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="a76a3-878">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="a76a3-879">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="a76a3-879">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="a76a3-880">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="a76a3-880">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="a76a3-881">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="a76a3-881">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="a76a3-882">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="a76a3-882">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="a76a3-883">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="a76a3-883">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="a76a3-884">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="a76a3-884">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-885">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-885">Az.Network</span></span>
* <span data-ttu-id="a76a3-886">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="a76a3-886">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="a76a3-887">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-887">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="a76a3-888">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-888">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="a76a3-889">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-889">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="a76a3-890">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-890">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="a76a3-891">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="a76a3-891">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="a76a3-892">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-892">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="a76a3-893">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="a76a3-893">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="a76a3-894">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="a76a3-894">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="a76a3-895">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-895">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="a76a3-896">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="a76a3-896">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="a76a3-897">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="a76a3-897">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="a76a3-898">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="a76a3-898">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="a76a3-899">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="a76a3-899">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="a76a3-900">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-900">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="a76a3-901">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-901">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-902">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-902">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-903">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="a76a3-903">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="a76a3-904">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="a76a3-904">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-905">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-905">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-906">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="a76a3-906">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-907">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-907">Az.Sql</span></span>
* <span data-ttu-id="a76a3-908">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="a76a3-908">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="a76a3-909">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="a76a3-909">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-910">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-910">Az.Storage</span></span>
* <span data-ttu-id="a76a3-911">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="a76a3-911">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="a76a3-912">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-912">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="a76a3-913">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-913">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="a76a3-914">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-914">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="a76a3-915">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="a76a3-915">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="a76a3-916">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="a76a3-916">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="a76a3-917">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="a76a3-917">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="a76a3-918">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="a76a3-918">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="a76a3-919">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="a76a3-919">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="a76a3-920">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="a76a3-920">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="a76a3-921">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="a76a3-921">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="a76a3-922">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-922">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="a76a3-923">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="a76a3-923">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="a76a3-924">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-924">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="a76a3-925">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-925">General</span></span>
* <span data-ttu-id="a76a3-926">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="a76a3-926">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="a76a3-927">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="a76a3-927">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="a76a3-928">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="a76a3-928">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="a76a3-929">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="a76a3-929">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="a76a3-930">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a76a3-930">Az.Billing</span></span>
  - <span data-ttu-id="a76a3-931">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-931">Az.Compute</span></span>
  - <span data-ttu-id="a76a3-932">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="a76a3-932">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="a76a3-933">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-933">Az.EventHub</span></span>
  - <span data-ttu-id="a76a3-934">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-934">Az.IotHub</span></span>
  - <span data-ttu-id="a76a3-935">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-935">Az.KeyVault</span></span>
  - <span data-ttu-id="a76a3-936">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-936">Az.Monitor</span></span>
  - <span data-ttu-id="a76a3-937">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-937">Az.Network</span></span>
  - <span data-ttu-id="a76a3-938">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-938">Az.Resources</span></span>
  - <span data-ttu-id="a76a3-939">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-939">Az.Storage</span></span>
  - <span data-ttu-id="a76a3-940">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-940">Az.Websites</span></span>
* <span data-ttu-id="a76a3-941">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-941">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="a76a3-942">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a76a3-942">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="a76a3-943">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="a76a3-943">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="a76a3-944">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-944">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-945">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-945">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-946">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="a76a3-946">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-947">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-947">Az.Compute</span></span>
* <span data-ttu-id="a76a3-948">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="a76a3-948">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="a76a3-949">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="a76a3-949">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="a76a3-950">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="a76a3-950">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="a76a3-951">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="a76a3-951">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="a76a3-952">[#11354]</span><span class="sxs-lookup"><span data-stu-id="a76a3-952">[#11354]</span></span>
* <span data-ttu-id="a76a3-953">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="a76a3-953">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="a76a3-954">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-954">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="a76a3-955">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-955">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="a76a3-956">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-956">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="a76a3-957">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-957">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="a76a3-958">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-958">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="a76a3-959">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="a76a3-959">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="a76a3-960">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-960">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="a76a3-961">[#11257]</span><span class="sxs-lookup"><span data-stu-id="a76a3-961">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-962">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-962">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-963">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-963">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="a76a3-964">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="a76a3-964">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-965">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-965">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-966">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="a76a3-966">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="a76a3-967">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-967">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-968">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-968">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-969">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="a76a3-969">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-970">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-970">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-971">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a76a3-971">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="a76a3-972">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-972">New Cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-973">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="a76a3-973">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="a76a3-974">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="a76a3-974">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-975">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-975">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-976">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="a76a3-976">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-977">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-977">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-978">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="a76a3-978">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-979">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-979">Az.Network</span></span>
* <span data-ttu-id="a76a3-980">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="a76a3-980">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="a76a3-981">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-981">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="a76a3-982">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="a76a3-982">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="a76a3-983">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="a76a3-983">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="a76a3-984">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="a76a3-984">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="a76a3-985">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="a76a3-985">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-986">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-986">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-987">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="a76a3-987">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-988">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-988">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-989">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-989">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="a76a3-990">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="a76a3-990">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="a76a3-991">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-991">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="a76a3-992">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="a76a3-992">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="a76a3-993">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-993">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="a76a3-994">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="a76a3-994">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-995">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-995">Az.Resources</span></span>
* <span data-ttu-id="a76a3-996">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="a76a3-996">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="a76a3-997">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="a76a3-997">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="a76a3-998">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="a76a3-998">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="a76a3-999">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-999">Added example.</span></span>
* <span data-ttu-id="a76a3-1000">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1000">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="a76a3-1001">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="a76a3-1001">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1002">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1002">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1003">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1003">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="a76a3-1004">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1004">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="a76a3-1005">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1005">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="a76a3-1006">Az.Support</span><span class="sxs-lookup"><span data-stu-id="a76a3-1006">Az.Support</span></span>
* <span data-ttu-id="a76a3-1007">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1007">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1008">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1008">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1009">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="a76a3-1009">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="a76a3-1010">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1010">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="a76a3-1011">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1011">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="a76a3-1012">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1012">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="a76a3-1013">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1013">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="a76a3-1014">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-1014">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1015">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1015">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1016">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1016">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="a76a3-1017">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1017">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="a76a3-1018">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="a76a3-1018">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-1019">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-1019">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-1020">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1020">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="a76a3-1021">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1021">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="a76a3-1022">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="a76a3-1022">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="a76a3-1023">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1023">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-1024">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-1024">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-1025">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1025">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-1026">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1026">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-1027">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1027">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="a76a3-1028">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1028">New Cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-1029">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1029">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a76a3-1030">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1030">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a76a3-1031">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1031">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a76a3-1032">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1032">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="a76a3-1033">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1033">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="a76a3-1034">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1034">New Cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-1035">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1035">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="a76a3-1036">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1036">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="a76a3-1037">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1037">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="a76a3-1038">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1038">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="a76a3-1039">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1039">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="a76a3-1040">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1040">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="a76a3-1041">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1041">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="a76a3-1042">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1042">New Cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-1043">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1043">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="a76a3-1044">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1044">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="a76a3-1045">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1045">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-1046">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1046">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-1047">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1047">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1048">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1048">Az.Network</span></span>
* <span data-ttu-id="a76a3-1049">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1049">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="a76a3-1050">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1050">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="a76a3-1051">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1051">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="a76a3-1052">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1052">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1053">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1053">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1054">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1054">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="a76a3-1055">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1055">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="a76a3-1056">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1056">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="a76a3-1057">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="a76a3-1057">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="a76a3-1058">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="a76a3-1058">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="a76a3-1059">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="a76a3-1059">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="a76a3-1060">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1060">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="a76a3-1061">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1061">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="a76a3-1062">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1062">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="a76a3-1063">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1063">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="a76a3-1064">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1064">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="a76a3-1065">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="a76a3-1065">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="a76a3-1066">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1066">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="a76a3-1067">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1067">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1068">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1068">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1069">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1069">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="a76a3-1070">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1070">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="a76a3-1071">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="a76a3-1071">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="a76a3-1072">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="a76a3-1072">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="a76a3-1073">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="a76a3-1073">Remove an LTR backup</span></span>
    - <span data-ttu-id="a76a3-1074">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="a76a3-1074">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="a76a3-1075">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="a76a3-1075">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="a76a3-1076">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-1076">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="a76a3-1077">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1077">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1078">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1078">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1079">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1079">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="a76a3-1080">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1080">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="a76a3-1081">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="a76a3-1081">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="a76a3-1082">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1082">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="a76a3-1083">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1083">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1084">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1084">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1085">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1085">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="a76a3-1086">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="a76a3-1086">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="a76a3-1087">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="a76a3-1087">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="a76a3-1088">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1088">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="a76a3-1089">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="a76a3-1089">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="a76a3-1090">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-1090">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a76a3-1091">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a76a3-1091">Highlights since the last major release</span></span>
* <span data-ttu-id="a76a3-1092">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1092">Updated client side telemetry.</span></span>
* <span data-ttu-id="a76a3-1093">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1093">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="a76a3-1094">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1094">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1095">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1095">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1096">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="a76a3-1096">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-1097">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1097">Az.Automation</span></span>
* <span data-ttu-id="a76a3-1098">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1098">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-1099">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1099">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-1100">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1100">Updated SDK to 7.0</span></span>
* <span data-ttu-id="a76a3-1101">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="a76a3-1101">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1102">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1102">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1103">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="a76a3-1103">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-1104">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1104">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-1105">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="a76a3-1105">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-1106">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1106">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-1107">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1107">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="a76a3-1108">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1108">New Cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-1109">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1109">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a76a3-1110">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1110">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a76a3-1111">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1111">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a76a3-1112">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1112">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-1113">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-1113">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-1114">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="a76a3-1114">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-1115">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1115">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-1116">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1116">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="a76a3-1117">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1117">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="a76a3-1118">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="a76a3-1118">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1119">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1119">Az.Network</span></span>
* <span data-ttu-id="a76a3-1120">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1120">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="a76a3-1121">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1121">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="a76a3-1122">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1122">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="a76a3-1123">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1123">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="a76a3-1124">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1124">No new cmdlets are added.</span></span> <span data-ttu-id="a76a3-1125">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1125">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1126">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1126">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1127">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1127">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1128">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1128">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1129">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="a76a3-1129">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="a76a3-1130">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1130">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="a76a3-1131">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1131">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="a76a3-1132">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="a76a3-1132">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="a76a3-1133">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1133">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="a76a3-1134">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="a76a3-1134">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="a76a3-1135">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1135">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="a76a3-1136">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="a76a3-1136">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1137">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1137">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1138">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1138">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="a76a3-1139">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="a76a3-1139">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="a76a3-1140">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="a76a3-1140">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="a76a3-1141">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="a76a3-1141">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="a76a3-1142">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="a76a3-1142">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a76a3-1143">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a76a3-1143">Az.StorageSync</span></span>
* <span data-ttu-id="a76a3-1144">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1144">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="a76a3-1145">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-1145">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a76a3-1146">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a76a3-1146">Highlights since the last major release</span></span>
* <span data-ttu-id="a76a3-1147">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="a76a3-1147">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="a76a3-1148">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1148">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1149">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1150">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="a76a3-1150">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="a76a3-1151">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="a76a3-1151">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-1152">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-1152">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-1153">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="a76a3-1153">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="a76a3-1154">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="a76a3-1154">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="a76a3-1155">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="a76a3-1155">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="a76a3-1156">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1156">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1157">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1157">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1158">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1158">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="a76a3-1159">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1159">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="a76a3-1160">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1160">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="a76a3-1161">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1161">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="a76a3-1162">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1162">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1163">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1163">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1164">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1164">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="a76a3-1165">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="a76a3-1165">Az.DeploymentManager</span></span>
* <span data-ttu-id="a76a3-1166">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1166">Adds LIST operations for resources</span></span>
* <span data-ttu-id="a76a3-1167">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-1167">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-1168">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-1168">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-1169">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1169">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-1170">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-1170">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-1171">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1171">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1172">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1172">Az.Network</span></span>
* <span data-ttu-id="a76a3-1173">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1173">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="a76a3-1174">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="a76a3-1174">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="a76a3-1175">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1175">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="a76a3-1176">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="a76a3-1176">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="a76a3-1177">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1177">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="a76a3-1178">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1178">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="a76a3-1179">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1179">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="a76a3-1180">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-1180">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="a76a3-1181">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1181">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-1182">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-1182">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="a76a3-1183">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-1183">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="a76a3-1184">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1184">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="a76a3-1185">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1185">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-1186">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-1186">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-1187">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="a76a3-1187">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="a76a3-1188">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1188">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="a76a3-1189">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="a76a3-1189">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="a76a3-1190">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="a76a3-1190">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1191">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1191">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1192">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1192">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="a76a3-1193">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1193">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1194">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1194">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1195">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="a76a3-1195">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="a76a3-1196">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="a76a3-1196">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1197">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1197">Az.Sql</span></span>
<span data-ttu-id="a76a3-1198">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1198">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1199">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1199">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1200">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-1200">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="a76a3-1201">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-1201">New-AzStorageAccount</span></span>
* <span data-ttu-id="a76a3-1202">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1202">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="a76a3-1203">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1203">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1204">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1204">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1205">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="a76a3-1205">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="a76a3-1206">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="a76a3-1206">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="a76a3-1207">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a76a3-1207">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1208">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1208">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1209">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="a76a3-1209">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-1210">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-1210">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-1211">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="a76a3-1211">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1212">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1212">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1213">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1213">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="a76a3-1214">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-1214">Az.ContainerInstance</span></span>
* <span data-ttu-id="a76a3-1215">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1215">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="a76a3-1216">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1216">Az.DataBoxEdge</span></span>
* <span data-ttu-id="a76a3-1217">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1217">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a76a3-1218">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1218">Get the Edge Storage Container</span></span>
* <span data-ttu-id="a76a3-1219">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1219">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a76a3-1220">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1220">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="a76a3-1221">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1221">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a76a3-1222">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1222">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="a76a3-1223">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1223">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a76a3-1224">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1224">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="a76a3-1225">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1225">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="a76a3-1226">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1226">Get the Edge Storage Account</span></span>
* <span data-ttu-id="a76a3-1227">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1227">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="a76a3-1228">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1228">Create new Edge Storage Account</span></span>
* <span data-ttu-id="a76a3-1229">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1229">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="a76a3-1230">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1230">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="a76a3-1231">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1231">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="a76a3-1232">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="a76a3-1232">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="a76a3-1233">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1233">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="a76a3-1234">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="a76a3-1234">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1235">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1235">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1236">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="a76a3-1236">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="a76a3-1237">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1237">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="a76a3-1238">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1238">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="a76a3-1239">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="a76a3-1239">Az.DevTestLabs</span></span>
* <span data-ttu-id="a76a3-1240">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="a76a3-1240">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-1241">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1241">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-1242">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="a76a3-1242">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-1243">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-1243">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-1244">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1244">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="a76a3-1245">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a76a3-1245">Az.MachineLearning</span></span>
* <span data-ttu-id="a76a3-1246">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="a76a3-1246">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="a76a3-1247">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a76a3-1247">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="a76a3-1248">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-1248">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="a76a3-1249">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a76a3-1249">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="a76a3-1250">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a76a3-1250">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="a76a3-1251">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a76a3-1251">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="a76a3-1252">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="a76a3-1252">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="a76a3-1253">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="a76a3-1253">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1254">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1254">Az.Network</span></span>
* <span data-ttu-id="a76a3-1255">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="a76a3-1255">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1256">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1256">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1257">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1257">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="a76a3-1258">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1258">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="a76a3-1259">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1259">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="a76a3-1260">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1260">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1261">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1261">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1262">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1262">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1263">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1263">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1264">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="a76a3-1264">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="a76a3-1265">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="a76a3-1265">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="a76a3-1266">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="a76a3-1266">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="a76a3-1267">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="a76a3-1267">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1268">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1268">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1269">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="a76a3-1269">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="a76a3-1270">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1270">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="a76a3-1271">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="a76a3-1271">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="a76a3-1272">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-1272">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="a76a3-1273">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1273">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="a76a3-1274">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-1274">General</span></span>
* <span data-ttu-id="a76a3-1275">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1275">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1276">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1276">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1277">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1277">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="a76a3-1278">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1278">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-1279">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-1279">Az.Batch</span></span>
* <span data-ttu-id="a76a3-1280">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1280">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1281">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1281">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1282">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1282">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-1283">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1283">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-1284">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="a76a3-1284">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="a76a3-1285">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="a76a3-1285">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="a76a3-1286">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="a76a3-1286">Az.HealthcareApis</span></span>
* <span data-ttu-id="a76a3-1287">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="a76a3-1287">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-1288">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-1288">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-1289">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="a76a3-1289">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="a76a3-1290">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="a76a3-1290">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="a76a3-1291">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="a76a3-1291">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-1292">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1292">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-1293">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1293">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="a76a3-1294">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="a76a3-1294">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="a76a3-1295">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1295">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1296">Az.Network</span></span>
* <span data-ttu-id="a76a3-1297">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1297">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1298">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1298">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1299">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1299">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="a76a3-1300">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1300">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1301">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1302">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1302">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1303">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1304">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="a76a3-1304">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="a76a3-1305">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="a76a3-1305">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="a76a3-1306">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a76a3-1306">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="a76a3-1307">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="a76a3-1307">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="a76a3-1308">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="a76a3-1308">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="a76a3-1309">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1309">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="a76a3-1310">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1310">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="a76a3-1311">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-1311">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="a76a3-1312">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-1312">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="a76a3-1313">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1313">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="a76a3-1314">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="a76a3-1314">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="a76a3-1315">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="a76a3-1315">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="a76a3-1316">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="a76a3-1316">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="a76a3-1317">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1317">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a76a3-1318">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a76a3-1318">Highlights since the last major release</span></span>
* <span data-ttu-id="a76a3-1319">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="a76a3-1319">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="a76a3-1320">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="a76a3-1320">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1321">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1321">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1322">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="a76a3-1322">VM Reapply feature</span></span>
    - <span data-ttu-id="a76a3-1323">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="a76a3-1323">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="a76a3-1324">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1324">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="a76a3-1325">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-1325">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="a76a3-1326">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a76a3-1326">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="a76a3-1327">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-1327">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="a76a3-1328">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="a76a3-1328">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="a76a3-1329">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="a76a3-1329">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="a76a3-1330">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="a76a3-1330">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="a76a3-1331">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="a76a3-1331">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="a76a3-1332">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-1332">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="a76a3-1333">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="a76a3-1333">Az.DataBoxEdge</span></span>
* <span data-ttu-id="a76a3-1334">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1334">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="a76a3-1335">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1335">Get the Order</span></span>
* <span data-ttu-id="a76a3-1336">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1336">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="a76a3-1337">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1337">Create new Order</span></span>
* <span data-ttu-id="a76a3-1338">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1338">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="a76a3-1339">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1339">Remove the Order</span></span>
* <span data-ttu-id="a76a3-1340">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1340">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="a76a3-1341">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="a76a3-1341">Now creates Local Share</span></span>
* <span data-ttu-id="a76a3-1342">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1342">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="a76a3-1343">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="a76a3-1343">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="a76a3-1344">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1344">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="a76a3-1345">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="a76a3-1345">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="a76a3-1346">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1346">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="a76a3-1347">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="a76a3-1347">Gets the information about Triggers</span></span>
* <span data-ttu-id="a76a3-1348">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1348">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="a76a3-1349">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="a76a3-1349">Create new Triggers</span></span>
* <span data-ttu-id="a76a3-1350">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="a76a3-1350">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="a76a3-1351">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="a76a3-1351">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1352">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1352">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1353">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1353">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="a76a3-1354">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1354">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-1355">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-1355">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-1356">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="a76a3-1356">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-1357">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1357">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-1358">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="a76a3-1358">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-1359">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1359">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-1360">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-1360">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="a76a3-1361">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-1361">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="a76a3-1362">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="a76a3-1362">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="a76a3-1363">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-1363">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1364">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1364">Az.Network</span></span>
* <span data-ttu-id="a76a3-1365">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1365">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="a76a3-1366">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="a76a3-1366">Az.PrivateDns</span></span>
* <span data-ttu-id="a76a3-1367">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1367">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1368">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1368">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1369">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1369">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="a76a3-1370">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1370">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="a76a3-1371">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1371">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a76a3-1372">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a76a3-1372">Az.RedisCache</span></span>
* <span data-ttu-id="a76a3-1373">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1373">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="a76a3-1374">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1374">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="a76a3-1375">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1375">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1376">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1376">Az.Resources</span></span>
- <span data-ttu-id="a76a3-1377">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1377">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="a76a3-1378">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="a76a3-1378">Updated create policy definition help example</span></span>
- <span data-ttu-id="a76a3-1379">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1379">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="a76a3-1380">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1380">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="a76a3-1381">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1381">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1382">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1382">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1383">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1383">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="a76a3-1384">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="a76a3-1384">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="a76a3-1385">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1385">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="a76a3-1386">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-1386">General</span></span>
* <span data-ttu-id="a76a3-1387">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1387">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1388">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1388">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1389">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1389">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="a76a3-1390">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1390">Az.Advisor</span></span>
* <span data-ttu-id="a76a3-1391">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1391">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-1392">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-1392">Az.Batch</span></span>
* <span data-ttu-id="a76a3-1393">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1393">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="a76a3-1394">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1394">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="a76a3-1395">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1395">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="a76a3-1396">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1396">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="a76a3-1397">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1397">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="a76a3-1398">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1398">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="a76a3-1399">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1399">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="a76a3-1400">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1400">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="a76a3-1401">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1401">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="a76a3-1402">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1402">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="a76a3-1403">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1403">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="a76a3-1404">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1404">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="a76a3-1405">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1405">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="a76a3-1406">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1406">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="a76a3-1407">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1407">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="a76a3-1408">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1408">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="a76a3-1409">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1409">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="a76a3-1410">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1410">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="a76a3-1411">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1411">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="a76a3-1412">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1412">This operation is no longer supported.</span></span>
* <span data-ttu-id="a76a3-1413">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1413">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="a76a3-1414">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1414">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="a76a3-1415">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1415">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="a76a3-1416">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1416">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="a76a3-1417">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1417">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="a76a3-1418">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1418">New non-verified images are also now returned.</span></span> <span data-ttu-id="a76a3-1419">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1419">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="a76a3-1420">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1420">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="a76a3-1421">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1421">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="a76a3-1422">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1422">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="a76a3-1423">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1423">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="a76a3-1424">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1424">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="a76a3-1425">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1425">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="a76a3-1426">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1426">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="a76a3-1427">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="a76a3-1427">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="a76a3-1428">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="a76a3-1428">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-1429">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-1429">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-1430">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1430">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="a76a3-1431">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1431">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1432">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1432">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1433">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1433">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="a76a3-1434">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1434">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="a76a3-1435">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="a76a3-1435">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="a76a3-1436">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1436">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a76a3-1437">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1437">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="a76a3-1438">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="a76a3-1438">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="a76a3-1439">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-1439">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="a76a3-1440">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1440">Breaking changes</span></span>
    - <span data-ttu-id="a76a3-1441">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="a76a3-1441">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="a76a3-1442">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="a76a3-1442">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1443">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1443">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1444">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1444">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-1445">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-1445">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-1446">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="a76a3-1446">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="a76a3-1447">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1447">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="a76a3-1448">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="a76a3-1448">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="a76a3-1449">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="a76a3-1449">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="a76a3-1450">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="a76a3-1450">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="a76a3-1451">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="a76a3-1451">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-1452">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1452">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-1453">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1453">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-1454">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-1454">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-1455">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1455">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="a76a3-1456">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1456">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="a76a3-1457">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1457">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="a76a3-1458">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1458">Removed five cmdlets:</span></span>
    - <span data-ttu-id="a76a3-1459">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="a76a3-1459">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="a76a3-1460">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="a76a3-1460">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="a76a3-1461">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="a76a3-1461">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="a76a3-1462">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a76a3-1462">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="a76a3-1463">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a76a3-1463">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="a76a3-1464">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1464">Added three cmdlets:</span></span>
    - <span data-ttu-id="a76a3-1465">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1465">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="a76a3-1466">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1466">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="a76a3-1467">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1467">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="a76a3-1468">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1468">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="a76a3-1469">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1469">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="a76a3-1470">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1470">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="a76a3-1471">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1471">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="a76a3-1472">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1472">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="a76a3-1473">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1473">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="a76a3-1474">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1474">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="a76a3-1475">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1475">Added some scenario test cases.</span></span>
* <span data-ttu-id="a76a3-1476">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1476">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-1477">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1477">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-1478">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1478">Breaking changes:</span></span>
    - <span data-ttu-id="a76a3-1479">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1479">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a76a3-1480">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1480">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="a76a3-1481">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1481">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a76a3-1482">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1482">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="a76a3-1483">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1483">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="a76a3-1484">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1484">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="a76a3-1485">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1485">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="a76a3-1486">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1486">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="a76a3-1487">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1487">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a76a3-1488">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1488">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="a76a3-1489">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1489">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a76a3-1490">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1490">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1491">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1491">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1492">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1492">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-1493">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1493">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="a76a3-1494">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1494">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="a76a3-1495">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1495">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-1496">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1496">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-1497">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1497">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-1498">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1498">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-1499">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1499">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-1500">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="a76a3-1500">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1501">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1501">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1502">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1502">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1503">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1503">Az.Network</span></span>
* <span data-ttu-id="a76a3-1504">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1504">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="a76a3-1505">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1505">Updated cmdlet:</span></span>
        - <span data-ttu-id="a76a3-1506">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1506">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1507">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1507">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1508">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1508">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1509">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1509">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1510">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1510">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="a76a3-1511">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1511">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="a76a3-1512">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1512">New cmdlet:</span></span>
        - <span data-ttu-id="a76a3-1513">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="a76a3-1513">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="a76a3-1514">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1514">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="a76a3-1515">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-1515">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="a76a3-1516">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1516">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="a76a3-1517">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1517">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="a76a3-1518">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1518">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="a76a3-1519">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-1519">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="a76a3-1520">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1520">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="a76a3-1521">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1521">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-1522">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1522">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="a76a3-1523">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-1523">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="a76a3-1524">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-1524">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="a76a3-1525">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-1525">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="a76a3-1526">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1526">Set-AzVirtualHub</span></span>
* <span data-ttu-id="a76a3-1527">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="a76a3-1527">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="a76a3-1528">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1528">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a76a3-1529">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="a76a3-1529">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="a76a3-1530">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="a76a3-1530">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="a76a3-1531">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="a76a3-1531">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="a76a3-1532">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="a76a3-1532">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="a76a3-1533">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1533">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="a76a3-1534">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1534">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-1535">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1535">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="a76a3-1536">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1536">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a76a3-1537">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a76a3-1537">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a76a3-1538">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a76a3-1538">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a76a3-1539">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a76a3-1539">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a76a3-1540">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a76a3-1540">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a76a3-1541">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a76a3-1541">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="a76a3-1542">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="a76a3-1542">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="a76a3-1543">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1543">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-1544">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="a76a3-1544">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="a76a3-1545">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="a76a3-1545">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="a76a3-1546">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="a76a3-1546">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="a76a3-1547">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="a76a3-1547">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="a76a3-1548">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-1548">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="a76a3-1549">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1549">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="a76a3-1550">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1550">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a76a3-1551">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-1551">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="a76a3-1552">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-1552">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="a76a3-1553">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="a76a3-1553">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="a76a3-1554">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="a76a3-1554">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="a76a3-1555">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1555">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a76a3-1556">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1556">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="a76a3-1557">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1557">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="a76a3-1558">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1558">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="a76a3-1559">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-1559">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="a76a3-1560">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1560">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="a76a3-1561">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1561">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-1562">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1562">New-AzIpGroup</span></span>
        - <span data-ttu-id="a76a3-1563">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1563">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="a76a3-1564">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1564">Get-AzIpGroup</span></span>
        - <span data-ttu-id="a76a3-1565">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1565">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-1566">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-1566">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-1567">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1567">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1568">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1568">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1569">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1569">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="a76a3-1570">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1570">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="a76a3-1571">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1571">Removed deprecated aliases:</span></span>
* <span data-ttu-id="a76a3-1572">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1572">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="a76a3-1573">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1573">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="a76a3-1574">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1574">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="a76a3-1575">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="a76a3-1575">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="a76a3-1576">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="a76a3-1576">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="a76a3-1577">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1577">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1578">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1578">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1579">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-1579">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="a76a3-1580">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-1580">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="a76a3-1581">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-1581">Set-AzStorageAccount</span></span>
* <span data-ttu-id="a76a3-1582">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="a76a3-1582">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="a76a3-1583">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a76a3-1583">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="a76a3-1584">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a76a3-1584">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="a76a3-1585">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1585">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="a76a3-1586">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-1586">General</span></span>
* <span data-ttu-id="a76a3-1587">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1587">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1588">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1588">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1589">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1589">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-1590">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-1590">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-1591">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1591">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="a76a3-1592">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="a76a3-1592">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-1593">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1593">Az.Automation</span></span>
* <span data-ttu-id="a76a3-1594">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1594">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-1595">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-1595">Az.Batch</span></span>
* <span data-ttu-id="a76a3-1596">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1596">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1597">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1597">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1598">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-1598">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="a76a3-1599">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-1599">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="a76a3-1600">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1600">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="a76a3-1601">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1601">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1602">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1602">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1603">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1603">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="a76a3-1604">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1604">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="a76a3-1605">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1605">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-1606">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-1606">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-1607">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="a76a3-1607">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="a76a3-1608">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="a76a3-1608">Az.HealthcareApis</span></span>
* <span data-ttu-id="a76a3-1609">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1609">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="a76a3-1610">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1610">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="a76a3-1611">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="a76a3-1611">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="a76a3-1612">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1612">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-1613">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1613">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-1614">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="a76a3-1614">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="a76a3-1615">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1615">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-1616">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1616">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-1617">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="a76a3-1617">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="a76a3-1618">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1618">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="a76a3-1619">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="a76a3-1619">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="a76a3-1620">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1620">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1621">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1621">Az.Network</span></span>
* <span data-ttu-id="a76a3-1622">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1622">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="a76a3-1623">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a76a3-1623">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="a76a3-1624">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1624">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-1625">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1625">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="a76a3-1626">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1626">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a76a3-1627">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="a76a3-1627">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="a76a3-1628">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1628">Updated cmdlets:</span></span>
        - <span data-ttu-id="a76a3-1629">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1629">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a76a3-1630">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1630">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a76a3-1631">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1631">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="a76a3-1632">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="a76a3-1632">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="a76a3-1633">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="a76a3-1633">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="a76a3-1634">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1634">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="a76a3-1635">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1635">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a76a3-1636">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a76a3-1636">Az.RedisCache</span></span>
* <span data-ttu-id="a76a3-1637">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1637">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1638">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1639">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="a76a3-1639">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1640">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1640">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1641">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1641">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="a76a3-1642">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="a76a3-1642">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="a76a3-1643">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="a76a3-1643">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="a76a3-1644">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="a76a3-1644">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="a76a3-1645">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-1645">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a76a3-1646">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a76a3-1646">Az.StorageSync</span></span>
* <span data-ttu-id="a76a3-1647">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1647">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1648">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1648">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1649">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="a76a3-1649">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="a76a3-1650">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1650">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-1651">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-1651">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-1652">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1652">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="a76a3-1653">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1653">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="a76a3-1654">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="a76a3-1654">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-1655">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1655">Az.Automation</span></span>
* <span data-ttu-id="a76a3-1656">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1656">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="a76a3-1657">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="a76a3-1657">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="a76a3-1658">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1658">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1659">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1659">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1660">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1660">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="a76a3-1661">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1661">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a76a3-1662">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1662">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="a76a3-1663">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1663">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="a76a3-1664">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1664">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="a76a3-1665">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1665">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="a76a3-1666">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1666">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="a76a3-1667">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1667">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="a76a3-1668">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1668">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1669">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1669">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1670">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="a76a3-1670">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="a76a3-1671">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="a76a3-1671">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-1672">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-1672">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-1673">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1673">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-1674">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1674">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-1675">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1675">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="a76a3-1676">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1676">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="a76a3-1677">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1677">New cmdlets are:</span></span>
    - <span data-ttu-id="a76a3-1678">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1678">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="a76a3-1679">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1679">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="a76a3-1680">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1680">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="a76a3-1681">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a76a3-1681">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-1682">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1682">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-1683">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="a76a3-1683">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="a76a3-1684">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1684">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="a76a3-1685">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1685">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="a76a3-1686">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1686">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="a76a3-1687">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1687">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="a76a3-1688">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1688">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="a76a3-1689">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1689">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="a76a3-1690">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1690">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="a76a3-1691">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1691">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="a76a3-1692">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1692">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="a76a3-1693">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1693">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="a76a3-1694">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1694">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="a76a3-1695">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1695">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="a76a3-1696">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="a76a3-1696">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="a76a3-1697">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="a76a3-1697">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="a76a3-1698">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1698">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="a76a3-1699">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1699">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="a76a3-1700">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1700">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="a76a3-1701">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1701">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="a76a3-1702">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1702">Overall improved help files</span></span>
* <span data-ttu-id="a76a3-1703">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1703">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1704">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1704">Az.Network</span></span>
* <span data-ttu-id="a76a3-1705">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1705">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="a76a3-1706">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="a76a3-1706">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="a76a3-1707">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="a76a3-1707">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="a76a3-1708">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="a76a3-1708">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="a76a3-1709">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="a76a3-1709">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="a76a3-1710">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="a76a3-1710">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="a76a3-1711">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="a76a3-1711">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="a76a3-1712">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="a76a3-1712">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="a76a3-1713">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-1713">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="a76a3-1714">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1714">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="a76a3-1715">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-1715">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="a76a3-1716">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="a76a3-1716">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="a76a3-1717">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-1717">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-1718">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="a76a3-1718">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="a76a3-1719">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1719">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="a76a3-1720">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1720">Updated cmdlet:</span></span>
        - <span data-ttu-id="a76a3-1721">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="a76a3-1721">New-VpnSite</span></span>
        - <span data-ttu-id="a76a3-1722">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="a76a3-1722">Update-VpnSite</span></span>
        - <span data-ttu-id="a76a3-1723">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1723">New-VpnConnection</span></span>
        - <span data-ttu-id="a76a3-1724">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1724">Update-VpnConnection</span></span>
* <span data-ttu-id="a76a3-1725">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="a76a3-1725">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1726">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1726">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1727">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="a76a3-1727">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="a76a3-1728">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="a76a3-1728">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1729">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1729">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1730">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1730">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-1731">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-1731">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-1732">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1732">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="a76a3-1733">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1733">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="a76a3-1734">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a76a3-1734">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a76a3-1735">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="a76a3-1735">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="a76a3-1736">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a76a3-1736">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="a76a3-1737">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="a76a3-1737">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="a76a3-1738">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a76a3-1738">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a76a3-1739">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a76a3-1739">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a76a3-1740">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="a76a3-1740">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="a76a3-1741">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a76a3-1741">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="a76a3-1742">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="a76a3-1742">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="a76a3-1743">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a76a3-1743">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a76a3-1744">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="a76a3-1744">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="a76a3-1745">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a76a3-1745">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="a76a3-1746">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="a76a3-1746">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="a76a3-1747">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1747">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a76a3-1748">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a76a3-1748">Az.SignalR</span></span>
* <span data-ttu-id="a76a3-1749">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1749">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1750">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1750">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1751">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1751">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="a76a3-1752">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="a76a3-1752">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="a76a3-1753">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1753">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="a76a3-1754">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1754">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="a76a3-1755">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="a76a3-1755">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1756">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1756">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1757">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1757">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="a76a3-1758">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="a76a3-1758">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="a76a3-1759">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-1759">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="a76a3-1760">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-1760">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="a76a3-1761">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1761">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="a76a3-1762">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-1762">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="a76a3-1763">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="a76a3-1763">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="a76a3-1764">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-1764">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="a76a3-1765">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-1765">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="a76a3-1766">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-1766">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="a76a3-1767">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-1767">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1768">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1768">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1769">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="a76a3-1769">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="a76a3-1770">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="a76a3-1770">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="a76a3-1771">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1771">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="a76a3-1772">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1772">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="a76a3-1773">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-1773">General</span></span>
* <span data-ttu-id="a76a3-1774">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1774">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1775">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1775">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1776">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1776">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-1777">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-1777">Az.Aks</span></span>
* <span data-ttu-id="a76a3-1778">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1778">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="a76a3-1779">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="a76a3-1779">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-1780">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-1780">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-1781">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="a76a3-1781">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="a76a3-1782">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="a76a3-1782">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="a76a3-1783">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1783">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="a76a3-1784">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="a76a3-1784">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="a76a3-1785">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1785">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-1786">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-1786">Az.Batch</span></span>
* <span data-ttu-id="a76a3-1787">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="a76a3-1787">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-1788">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-1788">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-1789">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="a76a3-1789">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1790">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1790">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1791">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1791">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="a76a3-1792">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-1792">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="a76a3-1793">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="a76a3-1793">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="a76a3-1794">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1794">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="a76a3-1795">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="a76a3-1795">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="a76a3-1796">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a76a3-1796">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="a76a3-1797">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="a76a3-1797">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="a76a3-1798">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1798">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1799">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1799">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1800">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1800">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="a76a3-1801">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="a76a3-1801">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="a76a3-1802">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="a76a3-1802">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="a76a3-1803">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="a76a3-1803">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-1804">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-1804">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-1805">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1805">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-1806">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1806">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-1807">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1807">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="a76a3-1808">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="a76a3-1808">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="a76a3-1809">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="a76a3-1809">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="a76a3-1810">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="a76a3-1810">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="a76a3-1811">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a76a3-1811">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a76a3-1812">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1812">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-1813">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1813">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-1814">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1814">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1815">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1815">Az.Network</span></span>
* <span data-ttu-id="a76a3-1816">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="a76a3-1816">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="a76a3-1817">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1817">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="a76a3-1818">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1818">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="a76a3-1819">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="a76a3-1819">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="a76a3-1820">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1820">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="a76a3-1821">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1821">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="a76a3-1822">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="a76a3-1822">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-1823">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-1823">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-1824">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1824">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="a76a3-1825">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="a76a3-1825">Added example</span></span>
    - <span data-ttu-id="a76a3-1826">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1826">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="a76a3-1827">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="a76a3-1827">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="a76a3-1828">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="a76a3-1828">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1829">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1829">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1830">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1830">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1831">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1831">Az.Resources</span></span>
* <span data-ttu-id="a76a3-1832">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="a76a3-1832">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="a76a3-1833">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="a76a3-1833">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="a76a3-1834">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="a76a3-1834">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="a76a3-1835">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1835">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a76a3-1836">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a76a3-1836">Az.ServiceBus</span></span>
* <span data-ttu-id="a76a3-1837">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-1837">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="a76a3-1838">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="a76a3-1838">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="a76a3-1839">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="a76a3-1839">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-1840">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-1840">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-1841">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1841">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="a76a3-1842">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1842">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="a76a3-1843">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="a76a3-1843">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="a76a3-1844">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1844">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="a76a3-1845">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="a76a3-1845">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="a76a3-1846">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="a76a3-1846">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1847">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1847">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1848">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1848">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1849">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1849">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1850">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="a76a3-1850">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="a76a3-1851">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="a76a3-1851">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="a76a3-1852">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-1852">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="a76a3-1853">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1853">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="a76a3-1854">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="a76a3-1854">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="a76a3-1855">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a76a3-1855">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1856">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1856">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1857">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a76a3-1857">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="a76a3-1858">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1858">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1859">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1859">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1860">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a76a3-1860">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="a76a3-1861">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-1861">Az.ApplicationInsights</span></span>
* <span data-ttu-id="a76a3-1862">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1862">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-1863">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1863">Az.Automation</span></span>
* <span data-ttu-id="a76a3-1864">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="a76a3-1864">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-1865">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1865">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-1866">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1866">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1867">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1867">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1868">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1868">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a76a3-1869">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a76a3-1869">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a76a3-1870">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-1870">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="a76a3-1871">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="a76a3-1871">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1872">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1872">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1873">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-1873">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="a76a3-1874">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1874">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-1875">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1875">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-1876">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="a76a3-1876">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="a76a3-1877">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="a76a3-1877">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-1878">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-1878">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-1879">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="a76a3-1879">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a76a3-1880">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-1880">Az.LogicApp</span></span>
* <span data-ttu-id="a76a3-1881">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="a76a3-1881">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="a76a3-1882">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="a76a3-1882">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="a76a3-1883">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1883">Az.ManagedServices</span></span>
* <span data-ttu-id="a76a3-1884">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="a76a3-1884">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1885">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1885">Az.Network</span></span>
* <span data-ttu-id="a76a3-1886">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="a76a3-1886">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="a76a3-1887">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-1887">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-1888">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a76a3-1888">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a76a3-1889">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-1889">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a76a3-1890">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1890">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1891">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1891">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1892">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1892">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1893">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1893">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a76a3-1894">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="a76a3-1894">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="a76a3-1895">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-1895">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="a76a3-1896">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="a76a3-1896">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="a76a3-1897">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1897">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="a76a3-1898">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1898">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="a76a3-1899">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1899">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="a76a3-1900">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="a76a3-1900">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="a76a3-1901">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="a76a3-1901">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="a76a3-1902">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="a76a3-1902">Updated cmdlets</span></span>
        - <span data-ttu-id="a76a3-1903">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1903">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a76a3-1904">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1904">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a76a3-1905">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1905">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="a76a3-1906">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-1906">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a76a3-1907">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-1907">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="a76a3-1908">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-1908">Updated cmdlet:</span></span>
        - <span data-ttu-id="a76a3-1909">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1909">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="a76a3-1910">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1910">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="a76a3-1911">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1911">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="a76a3-1912">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="a76a3-1912">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="a76a3-1913">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1913">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="a76a3-1914">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1914">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-1915">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-1915">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-1916">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1916">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="a76a3-1917">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="a76a3-1917">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1918">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1918">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1919">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1919">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="a76a3-1920">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1920">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="a76a3-1921">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1921">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="a76a3-1922">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1922">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="a76a3-1923">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1923">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="a76a3-1924">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1924">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="a76a3-1925">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1925">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="a76a3-1926">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1926">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="a76a3-1927">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-1927">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="a76a3-1928">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1928">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1929">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1929">Az.Resources</span></span>
- <span data-ttu-id="a76a3-1930">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1930">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="a76a3-1931">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a76a3-1931">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a76a3-1932">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a76a3-1932">Az.ServiceBus</span></span>
* <span data-ttu-id="a76a3-1933">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="a76a3-1933">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="a76a3-1934">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="a76a3-1934">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1935">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1935">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1936">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="a76a3-1936">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="a76a3-1937">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="a76a3-1937">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="a76a3-1938">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1938">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-1939">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-1939">Az.Storage</span></span>
* <span data-ttu-id="a76a3-1940">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="a76a3-1940">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a76a3-1941">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a76a3-1941">Az.StorageSync</span></span>
* <span data-ttu-id="a76a3-1942">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1942">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="a76a3-1943">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="a76a3-1943">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-1944">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-1944">Az.Websites</span></span>
* <span data-ttu-id="a76a3-1945">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-1945">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="a76a3-1946">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-1946">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="a76a3-1947">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-1947">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="a76a3-1948">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-1948">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-1949">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-1949">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-1950">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="a76a3-1950">Add support for profile cmdlets</span></span>
* <span data-ttu-id="a76a3-1951">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="a76a3-1951">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="a76a3-1952">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="a76a3-1952">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="a76a3-1953">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1953">Az.Advisor</span></span>
* <span data-ttu-id="a76a3-1954">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a76a3-1954">GA release of Az.Advisor</span></span>
* <span data-ttu-id="a76a3-1955">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="a76a3-1955">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-1956">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-1956">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-1957">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="a76a3-1957">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="a76a3-1958">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a76a3-1958">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="a76a3-1959">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="a76a3-1959">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="a76a3-1960">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1960">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="a76a3-1961">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="a76a3-1961">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="a76a3-1962">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a76a3-1962">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="a76a3-1963">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="a76a3-1963">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-1964">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-1964">Az.Automation</span></span>
* <span data-ttu-id="a76a3-1965">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="a76a3-1965">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-1966">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-1966">Az.Compute</span></span>
* <span data-ttu-id="a76a3-1967">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-1967">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-1968">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-1968">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-1969">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1969">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a76a3-1970">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a76a3-1970">Az.EventGrid</span></span>
* <span data-ttu-id="a76a3-1971">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1971">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-1972">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-1972">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-1973">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1973">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-1974">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-1974">Az.Network</span></span>
* <span data-ttu-id="a76a3-1975">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="a76a3-1975">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="a76a3-1976">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="a76a3-1976">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-1977">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-1977">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-1978">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="a76a3-1978">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="a76a3-1979">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="a76a3-1979">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-1980">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-1980">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-1981">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="a76a3-1981">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-1982">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-1982">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-1983">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="a76a3-1983">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-1984">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-1984">Az.Resources</span></span>
    - <span data-ttu-id="a76a3-1985">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="a76a3-1985">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="a76a3-1986">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="a76a3-1986">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="a76a3-1987">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-1987">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="a76a3-1988">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="a76a3-1988">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a76a3-1989">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a76a3-1989">Az.ServiceBus</span></span>
* <span data-ttu-id="a76a3-1990">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="a76a3-1990">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-1991">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-1991">Az.Sql</span></span>
* <span data-ttu-id="a76a3-1992">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="a76a3-1992">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="a76a3-1993">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-1993">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="a76a3-1994">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a76a3-1994">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a76a3-1995">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a76a3-1995">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a76a3-1996">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a76a3-1996">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a76a3-1997">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a76a3-1997">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="a76a3-1998">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a76a3-1998">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="a76a3-1999">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a76a3-1999">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="a76a3-2000">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="a76a3-2000">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2001">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2001">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2002">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2002">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="a76a3-2003">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a76a3-2003">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="a76a3-2004">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2004">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="a76a3-2005">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="a76a3-2005">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="a76a3-2006">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2006">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="a76a3-2007">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2007">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="a76a3-2008">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2008">Set-AzStorageAccount</span></span>
* <span data-ttu-id="a76a3-2009">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="a76a3-2009">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="a76a3-2010">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a76a3-2010">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="a76a3-2011">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a76a3-2011">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a76a3-2012">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a76a3-2012">Az.StorageSync</span></span>
* <span data-ttu-id="a76a3-2013">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2013">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="a76a3-2014">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2014">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2015">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2015">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2016">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="a76a3-2016">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="a76a3-2017">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="a76a3-2017">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="a76a3-2018">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a76a3-2018">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="a76a3-2019">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="a76a3-2019">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="a76a3-2020">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="a76a3-2020">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2021">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2021">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2022">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2022">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="a76a3-2023">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2023">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="a76a3-2024">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="a76a3-2024">Az.Dns</span></span>
* <span data-ttu-id="a76a3-2025">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2025">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a76a3-2026">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a76a3-2026">Az.EventGrid</span></span>
* <span data-ttu-id="a76a3-2027">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2027">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="a76a3-2028">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2028">New cmdlets:</span></span>
    - <span data-ttu-id="a76a3-2029">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a76a3-2029">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a76a3-2030">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2030">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a76a3-2031">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a76a3-2031">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a76a3-2032">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2032">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="a76a3-2033">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a76a3-2033">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a76a3-2034">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2034">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a76a3-2035">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-2035">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="a76a3-2036">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2036">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a76a3-2037">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-2037">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="a76a3-2038">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2038">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="a76a3-2039">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2039">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="a76a3-2040">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2040">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="a76a3-2041">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="a76a3-2041">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="a76a3-2042">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="a76a3-2042">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="a76a3-2043">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2043">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="a76a3-2044">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2044">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="a76a3-2045">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2045">Updated cmdlets:</span></span>
    - <span data-ttu-id="a76a3-2046">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2046">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="a76a3-2047">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2047">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="a76a3-2048">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2048">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="a76a3-2049">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="a76a3-2049">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="a76a3-2050">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2050">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="a76a3-2051">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="a76a3-2051">Event subscription expiration date,</span></span>
            - <span data-ttu-id="a76a3-2052">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2052">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="a76a3-2053">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2053">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="a76a3-2054">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="a76a3-2054">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="a76a3-2055">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2055">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="a76a3-2056">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2056">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="a76a3-2057">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="a76a3-2057">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="a76a3-2058">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2058">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="a76a3-2059">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2059">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-2060">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2060">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-2061">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-2061">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="a76a3-2062">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="a76a3-2062">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="a76a3-2063">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-2063">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="a76a3-2064">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="a76a3-2064">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2065">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2065">Az.Network</span></span>
* <span data-ttu-id="a76a3-2066">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a76a3-2066">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="a76a3-2067">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-2067">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-2068">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="a76a3-2068">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="a76a3-2069">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="a76a3-2069">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="a76a3-2070">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-2070">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-2071">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="a76a3-2071">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="a76a3-2072">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-2072">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="a76a3-2073">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-2073">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-2074">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-2074">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a76a3-2075">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-2075">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a76a3-2076">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a76a3-2076">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a76a3-2077">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2077">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="a76a3-2078">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2078">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="a76a3-2079">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a76a3-2079">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="a76a3-2080">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-2080">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-2081">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a76a3-2081">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a76a3-2082">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a76a3-2082">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a76a3-2083">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a76a3-2083">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a76a3-2084">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2084">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="a76a3-2085">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2085">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="a76a3-2086">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2086">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="a76a3-2087">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2087">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="a76a3-2088">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2088">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="a76a3-2089">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2089">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="a76a3-2090">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="a76a3-2090">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="a76a3-2091">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2091">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="a76a3-2092">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2092">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="a76a3-2093">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2093">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="a76a3-2094">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="a76a3-2094">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="a76a3-2095">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2095">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="a76a3-2096">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2096">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="a76a3-2097">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="a76a3-2097">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="a76a3-2098">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-2098">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="a76a3-2099">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2099">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="a76a3-2100">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="a76a3-2100">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="a76a3-2101">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a76a3-2101">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="a76a3-2102">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2102">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="a76a3-2103">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="a76a3-2103">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="a76a3-2104">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2104">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="a76a3-2105">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2105">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="a76a3-2106">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2106">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="a76a3-2107">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2107">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-2108">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2108">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-2109">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2109">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2110">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2110">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2111">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2111">Support for additional Template Export options</span></span>
    - <span data-ttu-id="a76a3-2112">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2112">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="a76a3-2113">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2113">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="a76a3-2114">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="a76a3-2114">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-2115">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2115">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-2116">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2116">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2117">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2117">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2118">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2118">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="a76a3-2119">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2119">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="a76a3-2120">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2120">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="a76a3-2121">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-2121">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a76a3-2122">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-2122">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a76a3-2123">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a76a3-2123">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a76a3-2124">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="a76a3-2124">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="a76a3-2125">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="a76a3-2125">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2126">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2126">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2127">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-2127">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="a76a3-2128">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2128">New-AzStorageAccount</span></span>
* <span data-ttu-id="a76a3-2129">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="a76a3-2129">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="a76a3-2130">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2130">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2131">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2131">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2132">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="a76a3-2132">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="a76a3-2133">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="a76a3-2133">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="a76a3-2134">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2134">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="a76a3-2135">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-2135">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-2136">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2136">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2137">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2137">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2138">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2138">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="a76a3-2139">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="a76a3-2139">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-2140">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2140">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-2141">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2141">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="a76a3-2142">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="a76a3-2142">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2143">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2143">Az.Network</span></span>
* <span data-ttu-id="a76a3-2144">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2144">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="a76a3-2145">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="a76a3-2145">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-2146">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2146">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-2147">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="a76a3-2147">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2148">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2148">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-2149">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="a76a3-2149">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a76a3-2150">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a76a3-2150">Az.ServiceBus</span></span>
* <span data-ttu-id="a76a3-2151">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="a76a3-2151">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-2152">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2152">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-2153">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2153">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="a76a3-2154">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2154">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2155">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2155">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2156">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2156">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="a76a3-2157">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2157">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="a76a3-2158">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2158">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="a76a3-2159">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2159">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2160">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2160">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2161">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2161">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="a76a3-2162">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2162">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="a76a3-2163">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-2163">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-2164">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2164">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="a76a3-2165">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="a76a3-2165">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="a76a3-2166">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2166">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="a76a3-2167">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2167">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="a76a3-2168">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2168">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="a76a3-2169">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="a76a3-2169">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="a76a3-2170">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2170">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="a76a3-2171">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2171">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="a76a3-2172">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-2172">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="a76a3-2173">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="a76a3-2173">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="a76a3-2174">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="a76a3-2174">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="a76a3-2175">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="a76a3-2175">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="a76a3-2176">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="a76a3-2176">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="a76a3-2177">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2177">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="a76a3-2178">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2178">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="a76a3-2179">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2179">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="a76a3-2180">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2180">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="a76a3-2181">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="a76a3-2181">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="a76a3-2182">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2182">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="a76a3-2183">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="a76a3-2183">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="a76a3-2184">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="a76a3-2184">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="a76a3-2185">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2185">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="a76a3-2186">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2186">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="a76a3-2187">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-2187">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="a76a3-2188">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2188">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="a76a3-2189">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2189">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="a76a3-2190">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2190">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="a76a3-2191">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2191">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="a76a3-2192">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2192">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="a76a3-2193">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2193">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="a76a3-2194">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="a76a3-2194">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="a76a3-2195">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="a76a3-2195">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="a76a3-2196">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2196">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="a76a3-2197">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2197">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a76a3-2198">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2198">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="a76a3-2199">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="a76a3-2199">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="a76a3-2200">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2200">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="a76a3-2201">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2201">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="a76a3-2202">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2202">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="a76a3-2203">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2203">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a76a3-2204">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2204">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="a76a3-2205">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2205">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="a76a3-2206">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2206">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="a76a3-2207">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2207">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="a76a3-2208">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2208">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a76a3-2209">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2209">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="a76a3-2210">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2210">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="a76a3-2211">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2211">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="a76a3-2212">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2212">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="a76a3-2213">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2213">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="a76a3-2214">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2214">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="a76a3-2215">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2215">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="a76a3-2216">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2216">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="a76a3-2217">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2217">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="a76a3-2218">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2218">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="a76a3-2219">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2219">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="a76a3-2220">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2220">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="a76a3-2221">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2221">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="a76a3-2222">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2222">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="a76a3-2223">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2223">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="a76a3-2224">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a76a3-2224">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="a76a3-2225">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2225">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="a76a3-2226">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2226">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="a76a3-2227">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2227">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="a76a3-2228">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2228">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="a76a3-2229">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2229">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="a76a3-2230">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="a76a3-2230">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="a76a3-2231">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2231">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="a76a3-2232">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="a76a3-2232">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="a76a3-2233">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2233">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="a76a3-2234">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="a76a3-2234">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="a76a3-2235">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2235">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="a76a3-2236">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2236">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="a76a3-2237">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2237">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="a76a3-2238">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2238">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="a76a3-2239">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2239">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="a76a3-2240">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2240">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-2241">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2241">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2242">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2242">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="a76a3-2243">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="a76a3-2243">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="a76a3-2244">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="a76a3-2244">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="a76a3-2245">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2245">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="a76a3-2246">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="a76a3-2246">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="a76a3-2247">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2247">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="a76a3-2248">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2248">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2249">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2249">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2250">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2250">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="a76a3-2251">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="a76a3-2251">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2252">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2252">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2253">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2253">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-2254">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2254">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-2255">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-2255">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2256">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2256">Az.Network</span></span>
* <span data-ttu-id="a76a3-2257">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2257">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="a76a3-2258">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2258">Updated cmdlet:</span></span>
        - <span data-ttu-id="a76a3-2259">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-2259">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="a76a3-2260">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a76a3-2260">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2261">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2261">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2262">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2262">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2263">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2263">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2264">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="a76a3-2264">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="a76a3-2265">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2265">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2266">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2266">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2267">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="a76a3-2267">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-2268">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2268">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-2269">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2269">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="a76a3-2270">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2270">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2271">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2271">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2272">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2272">Proximity placement group feature.</span></span>
    - <span data-ttu-id="a76a3-2273">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2273">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="a76a3-2274">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2274">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="a76a3-2275">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2275">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="a76a3-2276">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2276">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="a76a3-2277">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-2277">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="a76a3-2278">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2278">Breaking changes</span></span>
    - <span data-ttu-id="a76a3-2279">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2279">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="a76a3-2280">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2280">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="a76a3-2281">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="a76a3-2281">Az.DeploymentManager</span></span>
* <span data-ttu-id="a76a3-2282">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2282">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="a76a3-2283">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="a76a3-2283">Az.Dns</span></span>
* <span data-ttu-id="a76a3-2284">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="a76a3-2284">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="a76a3-2285">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2285">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="a76a3-2286">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2286">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-2287">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2287">Az.FrontDoor</span></span>
* <span data-ttu-id="a76a3-2288">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="a76a3-2288">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="a76a3-2289">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2289">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-2290">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-2290">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-2291">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2291">Removed two cmdlets:</span></span>
    - <span data-ttu-id="a76a3-2292">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a76a3-2292">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="a76a3-2293">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a76a3-2293">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="a76a3-2294">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a76a3-2294">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="a76a3-2295">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2295">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="a76a3-2296">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2296">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="a76a3-2297">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2297">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-2298">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2298">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-2299">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="a76a3-2299">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="a76a3-2300">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="a76a3-2300">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="a76a3-2301">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2301">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="a76a3-2302">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="a76a3-2302">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="a76a3-2303">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2303">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="a76a3-2304">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="a76a3-2304">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="a76a3-2305">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="a76a3-2305">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="a76a3-2306">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2306">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a76a3-2307">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2307">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a76a3-2308">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2308">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a76a3-2309">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2309">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a76a3-2310">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2310">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a76a3-2311">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="a76a3-2311">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="a76a3-2312">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="a76a3-2312">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2313">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2313">Az.Network</span></span>
* <span data-ttu-id="a76a3-2314">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="a76a3-2314">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="a76a3-2315">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-2315">New cmdlets</span></span>
        - <span data-ttu-id="a76a3-2316">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2316">New-AzNatGateway</span></span>
        - <span data-ttu-id="a76a3-2317">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2317">Get-AzNatGateway</span></span>
        - <span data-ttu-id="a76a3-2318">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2318">Set-AzNatGateway</span></span>
        - <span data-ttu-id="a76a3-2319">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2319">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="a76a3-2320">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="a76a3-2320">Updated cmdlets</span></span>
        - <span data-ttu-id="a76a3-2321">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="a76a3-2321">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="a76a3-2322">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="a76a3-2322">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="a76a3-2323">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2323">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="a76a3-2324">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2324">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="a76a3-2325">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2325">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-2326">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2326">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-2327">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2327">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="a76a3-2328">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2328">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="a76a3-2329">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2329">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2330">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2330">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-2331">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2331">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="a76a3-2332">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2332">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="a76a3-2333">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2333">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="a76a3-2334">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2334">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="a76a3-2335">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2335">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="a76a3-2336">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2336">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="a76a3-2337">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a76a3-2337">Az.Relay</span></span>
* <span data-ttu-id="a76a3-2338">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="a76a3-2338">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a76a3-2339">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a76a3-2339">Az.ServiceBus</span></span>
* <span data-ttu-id="a76a3-2340">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="a76a3-2340">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2341">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2341">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2342">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="a76a3-2342">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="a76a3-2343">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2343">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="a76a3-2344">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2344">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="a76a3-2345">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2345">New-AzStorageAccount</span></span>
* <span data-ttu-id="a76a3-2346">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="a76a3-2346">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="a76a3-2347">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2347">New-AzStorageAccount</span></span>
    - <span data-ttu-id="a76a3-2348">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2348">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="a76a3-2349">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2349">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2350">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2350">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2351">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-2351">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="a76a3-2352">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="a76a3-2352">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="a76a3-2353">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2353">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a76a3-2354">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a76a3-2354">Highlights since the last major release</span></span>
* <span data-ttu-id="a76a3-2355">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a76a3-2355">General availability of `Az` module</span></span>
* <span data-ttu-id="a76a3-2356">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a76a3-2356">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a76a3-2357">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a76a3-2357">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a76a3-2358">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2358">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a76a3-2359">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a76a3-2359">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a76a3-2360">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2360">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a76a3-2361">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a76a3-2361">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2362">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2362">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2363">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="a76a3-2363">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a76a3-2364">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-2364">Az.Batch</span></span>
* <span data-ttu-id="a76a3-2365">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2365">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-2366">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-2366">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-2367">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2367">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-2368">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2368">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-2369">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2369">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2370">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2370">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2371">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2371">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="a76a3-2372">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2372">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a76a3-2373">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a76a3-2373">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-2374">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-2374">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-2375">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2375">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2376">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2376">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2377">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2377">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a76a3-2378">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a76a3-2378">Az.EventGrid</span></span>
* <span data-ttu-id="a76a3-2379">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2379">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-2380">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2380">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-2381">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="a76a3-2381">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a76a3-2382">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a76a3-2382">Az.HDInsight</span></span>
* <span data-ttu-id="a76a3-2383">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2383">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-2384">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2384">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-2385">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2385">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-2386">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-2386">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-2387">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2387">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a76a3-2388">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a76a3-2388">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="a76a3-2389">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a76a3-2389">Az.MachineLearning</span></span>
* <span data-ttu-id="a76a3-2390">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2390">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="a76a3-2391">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a76a3-2391">Az.Media</span></span>
* <span data-ttu-id="a76a3-2392">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2392">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-2393">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2393">Az.Monitor</span></span>
  * <span data-ttu-id="a76a3-2394">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="a76a3-2394">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="a76a3-2395">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="a76a3-2395">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="a76a3-2396">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="a76a3-2396">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="a76a3-2397">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a76a3-2397">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="a76a3-2398">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a76a3-2398">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="a76a3-2399">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a76a3-2399">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="a76a3-2400">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="a76a3-2400">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2401">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2401">Az.Network</span></span>
* <span data-ttu-id="a76a3-2402">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2402">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a76a3-2403">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a76a3-2403">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="a76a3-2404">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="a76a3-2404">Az.NotificationHubs</span></span>
* <span data-ttu-id="a76a3-2405">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2405">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-2406">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2406">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-2407">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2407">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="a76a3-2408">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a76a3-2408">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="a76a3-2409">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2409">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2410">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2410">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-2411">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2411">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a76a3-2412">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2412">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="a76a3-2413">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="a76a3-2413">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="a76a3-2414">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="a76a3-2414">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a76a3-2415">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a76a3-2415">Az.RedisCache</span></span>
* <span data-ttu-id="a76a3-2416">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2416">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2417">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2417">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2418">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a76a3-2418">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2419">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2419">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2420">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="a76a3-2420">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="a76a3-2421">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2421">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a76a3-2422">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2422">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="a76a3-2423">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2423">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="a76a3-2424">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2424">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="a76a3-2425">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2425">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="a76a3-2426">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a76a3-2426">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2427">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2427">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2428">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="a76a3-2428">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="a76a3-2429">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2429">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a76a3-2430">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2430">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="a76a3-2431">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2431">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="a76a3-2432">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2432">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a76a3-2433">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a76a3-2433">Highlights since the last major release</span></span>
* <span data-ttu-id="a76a3-2434">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a76a3-2434">General availability of `Az` module</span></span>
* <span data-ttu-id="a76a3-2435">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a76a3-2435">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a76a3-2436">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a76a3-2436">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a76a3-2437">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2437">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a76a3-2438">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a76a3-2438">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a76a3-2439">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2439">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a76a3-2440">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a76a3-2440">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2441">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2441">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2442">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="a76a3-2442">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a76a3-2443">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2443">Az.AnalysisServices</span></span>
* <span data-ttu-id="a76a3-2444">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="a76a3-2444">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="a76a3-2445">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="a76a3-2445">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-2446">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2446">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2447">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2447">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="a76a3-2448">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2448">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="a76a3-2449">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2449">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2450">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2450">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2451">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2451">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a76a3-2452">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2452">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="a76a3-2453">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2453">Az.ContainerInstance</span></span>
* <span data-ttu-id="a76a3-2454">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="a76a3-2454">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-2455">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-2455">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-2456">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="a76a3-2456">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="a76a3-2457">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2457">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2458">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2458">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2459">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2459">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="a76a3-2460">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2460">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="a76a3-2461">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="a76a3-2461">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="a76a3-2462">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a76a3-2462">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="a76a3-2463">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2463">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="a76a3-2464">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a76a3-2464">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2465">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2465">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2466">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2466">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2467">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2467">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2468">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2468">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="a76a3-2469">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a76a3-2469">New-AzStorageContext</span></span>
* <span data-ttu-id="a76a3-2470">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="a76a3-2470">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="a76a3-2471">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a76a3-2471">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a76a3-2472">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a76a3-2472">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a76a3-2473">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2473">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="a76a3-2474">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2474">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="a76a3-2475">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="a76a3-2475">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="a76a3-2476">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-2476">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a76a3-2477">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-2477">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a76a3-2478">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-2478">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="a76a3-2479">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a76a3-2479">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="a76a3-2480">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2480">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a76a3-2481">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a76a3-2481">Highlights since the last major release</span></span>
* <span data-ttu-id="a76a3-2482">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a76a3-2482">General availability of `Az` module</span></span>
* <span data-ttu-id="a76a3-2483">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a76a3-2483">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a76a3-2484">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a76a3-2484">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a76a3-2485">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2485">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a76a3-2486">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a76a3-2486">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a76a3-2487">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2487">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a76a3-2488">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a76a3-2488">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-2489">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2489">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2490">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2490">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="a76a3-2491">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="a76a3-2491">Dynamic grouping</span></span>
    * <span data-ttu-id="a76a3-2492">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2492">Pre-Post script</span></span>
    * <span data-ttu-id="a76a3-2493">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="a76a3-2493">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2494">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2494">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2495">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="a76a3-2495">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="a76a3-2496">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2496">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-2497">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-2497">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-2498">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-2498">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2499">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2499">Az.Network</span></span>
* <span data-ttu-id="a76a3-2500">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-2500">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="a76a3-2501">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2501">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2502">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2502">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-2503">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2503">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="a76a3-2504">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="a76a3-2504">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2505">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2505">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2506">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2506">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="a76a3-2507">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="a76a3-2507">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2508">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2508">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2509">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2509">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2510">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2510">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2511">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a76a3-2511">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="a76a3-2512">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2512">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a76a3-2513">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2513">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a76a3-2514">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2514">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a76a3-2515">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="a76a3-2515">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="a76a3-2516">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="a76a3-2516">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="a76a3-2517">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2517">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2518">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2519">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2519">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="a76a3-2520">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2520">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2521">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2521">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2522">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="a76a3-2522">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="a76a3-2523">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2523">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-2524">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2524">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2525">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2525">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="a76a3-2526">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2526">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="a76a3-2527">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="a76a3-2527">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-2528">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-2528">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-2529">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2529">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2530">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2530">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2531">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="a76a3-2531">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-2532">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-2532">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-2533">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="a76a3-2533">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a76a3-2534">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-2534">Az.LogicApp</span></span>
* <span data-ttu-id="a76a3-2535">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="a76a3-2535">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2536">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2536">Az.Network</span></span>
* <span data-ttu-id="a76a3-2537">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2537">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2538">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2538">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-2539">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2539">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="a76a3-2540">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="a76a3-2540">SDK Update</span></span>
* <span data-ttu-id="a76a3-2541">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a76a3-2541">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="a76a3-2542">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a76a3-2542">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2543">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2543">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2544">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2544">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="a76a3-2545">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="a76a3-2545">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="a76a3-2546">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="a76a3-2546">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="a76a3-2547">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="a76a3-2547">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="a76a3-2548">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="a76a3-2548">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="a76a3-2549">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="a76a3-2549">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2550">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2550">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2551">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2551">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="a76a3-2552">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2552">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2553">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2553">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2554">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2554">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="a76a3-2555">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2555">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="a76a3-2556">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2556">Az.AnalysisServices</span></span>
* <span data-ttu-id="a76a3-2557">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="a76a3-2557">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-2558">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2558">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2559">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2559">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="a76a3-2560">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2560">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="a76a3-2561">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2561">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-2562">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2562">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-2563">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2563">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2564">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2564">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2565">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="a76a3-2565">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="a76a3-2566">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="a76a3-2566">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="a76a3-2567">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2567">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="a76a3-2568">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2568">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2569">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2569">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2570">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="a76a3-2570">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a76a3-2571">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2571">Az.EventHub</span></span>
* <span data-ttu-id="a76a3-2572">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2572">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-2573">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-2573">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-2574">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a76a3-2574">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a76a3-2575">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-2575">Az.LogicApp</span></span>
* <span data-ttu-id="a76a3-2576">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a76a3-2576">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="a76a3-2577">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2577">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="a76a3-2578">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a76a3-2578">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="a76a3-2579">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a76a3-2579">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a76a3-2580">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a76a3-2580">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a76a3-2581">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a76a3-2581">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a76a3-2582">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a76a3-2582">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="a76a3-2583">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a76a3-2583">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="a76a3-2584">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2584">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a76a3-2585">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2585">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a76a3-2586">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2586">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a76a3-2587">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2587">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="a76a3-2588">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-2588">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a76a3-2589">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2589">Az.Monitor</span></span>
* <span data-ttu-id="a76a3-2590">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2590">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2591">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2591">Az.Network</span></span>
* <span data-ttu-id="a76a3-2592">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="a76a3-2592">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-2593">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2593">Az.OperationalInsights</span></span>
* <span data-ttu-id="a76a3-2594">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2594">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="a76a3-2595">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2595">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="a76a3-2596">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2596">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2597">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2597">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2598">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a76a3-2598">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a76a3-2599">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a76a3-2599">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="a76a3-2600">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="a76a3-2600">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="a76a3-2601">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="a76a3-2601">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2602">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2602">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2603">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="a76a3-2603">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="a76a3-2604">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="a76a3-2604">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2605">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2605">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2606">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="a76a3-2606">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="a76a3-2607">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2607">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2608">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2608">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2609">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a76a3-2609">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a76a3-2610">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2610">Az.AnalysisServices</span></span>
<span data-ttu-id="a76a3-2611">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2611">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2612">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2612">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2613">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="a76a3-2613">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="a76a3-2614">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="a76a3-2614">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="a76a3-2615">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2615">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2616">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2616">Az.RecoveryServices</span></span>
<span data-ttu-id="a76a3-2617">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2617">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2618">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2618">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2619">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2619">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="a76a3-2620">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a76a3-2620">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a76a3-2621">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="a76a3-2621">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="a76a3-2622">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a76a3-2622">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2623">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2623">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2624">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2624">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="a76a3-2625">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="a76a3-2625">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="a76a3-2626">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="a76a3-2626">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="a76a3-2627">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2627">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2628">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2628">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2629">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2629">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a76a3-2630">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2630">Az.AnalysisServices</span></span>
* <span data-ttu-id="a76a3-2631">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2631">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2632">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2632">Az.RecoveryServices</span></span>
* <span data-ttu-id="a76a3-2633">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2633">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="a76a3-2634">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2634">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2635">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2635">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2636">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a76a3-2636">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a76a3-2637">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2637">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a76a3-2638">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="a76a3-2638">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="a76a3-2639">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a76a3-2639">Az.Aks</span></span>
* <span data-ttu-id="a76a3-2640">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2640">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a76a3-2641">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2641">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2642">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="a76a3-2642">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="a76a3-2643">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2643">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a76a3-2644">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a76a3-2644">Az.Cdn</span></span>
* <span data-ttu-id="a76a3-2645">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2645">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2646">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2646">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2647">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2647">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="a76a3-2648">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a76a3-2648">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="a76a3-2649">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a76a3-2649">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a76a3-2650">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a76a3-2650">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a76a3-2651">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2651">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a76a3-2652">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a76a3-2652">Az.DataFactory</span></span>
* <span data-ttu-id="a76a3-2653">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="a76a3-2653">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2654">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2654">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2655">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="a76a3-2655">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="a76a3-2656">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="a76a3-2656">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="a76a3-2657">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2657">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-2658">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2658">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-2659">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2659">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a76a3-2660">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-2660">Az.KeyVault</span></span>
* <span data-ttu-id="a76a3-2661">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2661">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2662">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2662">Az.Network</span></span>
* <span data-ttu-id="a76a3-2663">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2663">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2664">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2664">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2665">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2665">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="a76a3-2666">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2666">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="a76a3-2667">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="a76a3-2667">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="a76a3-2668">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="a76a3-2668">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="a76a3-2669">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="a76a3-2669">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="a76a3-2670">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2670">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="a76a3-2671">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="a76a3-2671">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-2672">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2672">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-2673">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="a76a3-2673">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="a76a3-2674">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2674">Fix some error messages.</span></span>
* <span data-ttu-id="a76a3-2675">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2675">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="a76a3-2676">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2676">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a76a3-2677">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a76a3-2677">Az.SignalR</span></span>
* <span data-ttu-id="a76a3-2678">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2678">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2679">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2679">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2680">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2680">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a76a3-2681">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="a76a3-2681">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="a76a3-2682">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2682">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="a76a3-2683">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="a76a3-2683">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2684">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2684">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2685">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2685">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a76a3-2686">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2686">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="a76a3-2687">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="a76a3-2687">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="a76a3-2688">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="a76a3-2688">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="a76a3-2689">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a76a3-2689">Az.TrafficManager</span></span>
* <span data-ttu-id="a76a3-2690">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2690">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2691">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2691">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2692">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2692">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a76a3-2693">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2693">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="a76a3-2694">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2694">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="a76a3-2695">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a76a3-2695">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a76a3-2696">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2696">Az.Accounts</span></span>
* <span data-ttu-id="a76a3-2697">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="a76a3-2697">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2698">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2699">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2699">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="a76a3-2700">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a76a3-2700">Updated the description of ID in help files</span></span>
* <span data-ttu-id="a76a3-2701">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2701">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2702">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2702">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2703">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2703">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="a76a3-2704">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="a76a3-2704">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a76a3-2705">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a76a3-2705">Az.EventGrid</span></span>
* <span data-ttu-id="a76a3-2706">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2706">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="a76a3-2707">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a76a3-2707">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="a76a3-2708">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2708">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a76a3-2709">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a76a3-2709">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a76a3-2710">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a76a3-2710">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a76a3-2711">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2711">Dead letter endpoint.</span></span>
    - <span data-ttu-id="a76a3-2712">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2712">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a76a3-2713">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a76a3-2713">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a76a3-2714">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a76a3-2714">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a76a3-2715">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2715">Dead letter endpoint.</span></span>
* <span data-ttu-id="a76a3-2716">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2716">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="a76a3-2717">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2717">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a76a3-2718">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2718">Az.IotHub</span></span>
* <span data-ttu-id="a76a3-2719">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="a76a3-2719">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a76a3-2720">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a76a3-2720">Az.LogicApp</span></span>
* <span data-ttu-id="a76a3-2721">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="a76a3-2721">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2722">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2722">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2723">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2723">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="a76a3-2724">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="a76a3-2724">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="a76a3-2725">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a76a3-2725">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a76a3-2726">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="a76a3-2726">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="a76a3-2727">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2727">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="a76a3-2728">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="a76a3-2728">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a76a3-2729">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a76a3-2729">Az.SignalR</span></span>
* <span data-ttu-id="a76a3-2730">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2730">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-2731">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2731">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2732">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2732">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a76a3-2733">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2733">Az.Storage</span></span>
* <span data-ttu-id="a76a3-2734">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2734">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="a76a3-2735">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a76a3-2735">New-AzStorageContext</span></span>
* <span data-ttu-id="a76a3-2736">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2736">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="a76a3-2737">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a76a3-2737">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-2738">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2738">Az.Websites</span></span>
* <span data-ttu-id="a76a3-2739">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2739">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="a76a3-2740">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2740">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="a76a3-2741">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-2741">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="a76a3-2742">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-2742">General</span></span>

- <span data-ttu-id="a76a3-2743">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="a76a3-2743">General Availability of Az Module</span></span>
- <span data-ttu-id="a76a3-2744">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="a76a3-2744">Online help for each module</span></span>
- <span data-ttu-id="a76a3-2745">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="a76a3-2745">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="a76a3-2746">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="a76a3-2746">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="a76a3-2747">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2747">Az.Accounts</span></span>
- <span data-ttu-id="a76a3-2748">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2748">Changed from Az.Profile</span></span>
- <span data-ttu-id="a76a3-2749">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="a76a3-2749">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a76a3-2750">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-2750">Az.ApiManagement</span></span>
- <span data-ttu-id="a76a3-2751">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="a76a3-2751">Fixes for #7002</span></span>
- <span data-ttu-id="a76a3-2752">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2752">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="a76a3-2753">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a76a3-2753">Az.Batch</span></span>
- <span data-ttu-id="a76a3-2754">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2754">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="a76a3-2755">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2755">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="a76a3-2756">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2756">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="a76a3-2757">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a76a3-2757">Az.Billing</span></span>
- <span data-ttu-id="a76a3-2758">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2758">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="a76a3-2759">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2759">Az.CognitivServices</span></span>
- <span data-ttu-id="a76a3-2760">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2760">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="a76a3-2761">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="a76a3-2761">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a76a3-2762">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2762">Az.ContainerInstance</span></span>
- <span data-ttu-id="a76a3-2763">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="a76a3-2763">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="a76a3-2764">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a76a3-2764">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="a76a3-2765">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2765">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2766">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2766">Az.DataLakeStore</span></span>
- <span data-ttu-id="a76a3-2767">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2767">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="a76a3-2768">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2768">Az.Monitor</span></span>
- <span data-ttu-id="a76a3-2769">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2769">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="a76a3-2770">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a76a3-2770">Az.KeyVault</span></span>
- <span data-ttu-id="a76a3-2771">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="a76a3-2771">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="a76a3-2772">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a76a3-2772">Az.MachineLearning</span></span>
- <span data-ttu-id="a76a3-2773">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2773">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="a76a3-2774">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a76a3-2774">Az.Media</span></span>
- <span data-ttu-id="a76a3-2775">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="a76a3-2775">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a76a3-2776">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2776">Az.Network</span></span>
<span data-ttu-id="a76a3-2777">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a76a3-2777">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="a76a3-2778">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a76a3-2778">New cmdlets added:</span></span>
        - <span data-ttu-id="a76a3-2779">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2779">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a76a3-2780">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2780">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a76a3-2781">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2781">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a76a3-2782">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2782">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a76a3-2783">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2783">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a76a3-2784">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2784">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="a76a3-2785">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2785">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="a76a3-2786">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="a76a3-2786">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="a76a3-2787">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2787">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="a76a3-2788">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a76a3-2788">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="a76a3-2789">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2789">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a76a3-2790">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a76a3-2790">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a76a3-2791">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2791">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="a76a3-2792">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2792">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="a76a3-2793">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2793">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="a76a3-2794">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a76a3-2794">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="a76a3-2795">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a76a3-2795">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a76a3-2796">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a76a3-2796">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a76a3-2797">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a76a3-2797">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="a76a3-2798">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="a76a3-2798">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="a76a3-2799">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2799">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="a76a3-2800">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2800">Az.OperationalInsights</span></span>
- <span data-ttu-id="a76a3-2801">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2801">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="a76a3-2802">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2802">Az.Profile</span></span>
- <span data-ttu-id="a76a3-2803">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a76a3-2803">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2804">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2804">Az.RecoveryServices</span></span>
- <span data-ttu-id="a76a3-2805">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2805">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="a76a3-2806">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2806">Az.Resources</span></span>
- <span data-ttu-id="a76a3-2807">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2807">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a76a3-2808">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2808">Az.ServiceFabric</span></span>
- <span data-ttu-id="a76a3-2809">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="a76a3-2809">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="a76a3-2810">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2810">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="a76a3-2811">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="a76a3-2811">Az.SIgnalR</span></span>
- <span data-ttu-id="a76a3-2812">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="a76a3-2812">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="a76a3-2813">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2813">Az.Sql</span></span>
- <span data-ttu-id="a76a3-2814">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="a76a3-2814">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="a76a3-2815">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="a76a3-2815">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="a76a3-2816">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2816">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="a76a3-2817">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2817">Az.Storage</span></span>
- <span data-ttu-id="a76a3-2818">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2818">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a76a3-2819">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2819">Az.Websites</span></span>
- <span data-ttu-id="a76a3-2820">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a76a3-2820">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="a76a3-2821">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-2821">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="a76a3-2822">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-2822">General</span></span>

* <span data-ttu-id="a76a3-2823">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a76a3-2823">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="a76a3-2824">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2824">Az.Compute</span></span>

* <span data-ttu-id="a76a3-2825">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2825">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2826">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2826">Az.DataLakeStore</span></span>

* <span data-ttu-id="a76a3-2827">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="a76a3-2827">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="a76a3-2828">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a76a3-2828">Az.FrontDoor</span></span>

* <span data-ttu-id="a76a3-2829">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2829">Fixed some broken links</span></span>
    - <span data-ttu-id="a76a3-2830">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2830">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="a76a3-2831">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2831">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a76a3-2832">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2832">Az.RecoveryServices</span></span>

* <span data-ttu-id="a76a3-2833">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2833">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="a76a3-2834">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2834">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="a76a3-2835">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2835">Az.Resources</span></span>

* <span data-ttu-id="a76a3-2836">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="a76a3-2836">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="a76a3-2837">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2837">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="a76a3-2838">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2838">Az.Sql</span></span>

* <span data-ttu-id="a76a3-2839">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a76a3-2839">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="a76a3-2840">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="a76a3-2840">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="a76a3-2841">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2841">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="a76a3-2842">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2842">Az.Storage</span></span>

* <span data-ttu-id="a76a3-2843">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a76a3-2843">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="a76a3-2844">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="a76a3-2844">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="a76a3-2845">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2845">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a76a3-2846">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="a76a3-2846">Support Static Website configuration</span></span>
    - <span data-ttu-id="a76a3-2847">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a76a3-2847">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="a76a3-2848">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a76a3-2848">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a76a3-2849">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-2849">Az.Websites</span></span>

* <span data-ttu-id="a76a3-2850">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a76a3-2850">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="a76a3-2851">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2851">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="a76a3-2852">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2852">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="a76a3-2853">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-2853">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a76a3-2854">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a76a3-2854">Az.ApiManagement</span></span>
* <span data-ttu-id="a76a3-2855">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2855">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="a76a3-2856">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a76a3-2856">Az.Automation</span></span>
* <span data-ttu-id="a76a3-2857">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="a76a3-2857">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="a76a3-2858">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="a76a3-2858">Added Update Management cmdlets</span></span>
* <span data-ttu-id="a76a3-2859">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="a76a3-2859">Added Source Control cmdlets</span></span>
* <span data-ttu-id="a76a3-2860">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2860">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="a76a3-2861">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="a76a3-2861">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="a76a3-2862">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2862">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2863">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="a76a3-2863">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="a76a3-2864">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2864">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a76a3-2865">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2865">Az.ContainerInstance</span></span>
* <span data-ttu-id="a76a3-2866">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2866">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="a76a3-2867">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a76a3-2867">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a76a3-2868">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="a76a3-2868">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a76a3-2869">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2869">Az.Network</span></span>
* <span data-ttu-id="a76a3-2870">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="a76a3-2870">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="a76a3-2871">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="a76a3-2871">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="a76a3-2872">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2872">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="a76a3-2873">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="a76a3-2873">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="a76a3-2874">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a76a3-2874">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a76a3-2875">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2875">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="a76a3-2876">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2876">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="a76a3-2877">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a76a3-2877">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a76a3-2878">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a76a3-2878">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="a76a3-2879">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a76a3-2879">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="a76a3-2880">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a76a3-2880">Az.Relay</span></span>
* <span data-ttu-id="a76a3-2881">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2881">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="a76a3-2882">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2882">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2883">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="a76a3-2883">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="a76a3-2884">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="a76a3-2884">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="a76a3-2885">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="a76a3-2885">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a76a3-2886">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2886">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-2887">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a76a3-2887">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="a76a3-2888">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-2888">Az.Sql</span></span>
* <span data-ttu-id="a76a3-2889">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-2889">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="a76a3-2890">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2890">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a76a3-2891">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2891">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a76a3-2892">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2892">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a76a3-2893">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a76a3-2893">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a76a3-2894">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a76a3-2894">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a76a3-2895">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a76a3-2895">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a76a3-2896">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a76a3-2896">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a76a3-2897">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a76a3-2897">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="a76a3-2898">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2898">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="a76a3-2899">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2899">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="a76a3-2900">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2900">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="a76a3-2901">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2901">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a76a3-2902">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2902">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a76a3-2903">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2903">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="a76a3-2904">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2904">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="a76a3-2905">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="a76a3-2905">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="a76a3-2906">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-2906">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a76a3-2907">Geral</span><span class="sxs-lookup"><span data-stu-id="a76a3-2907">General</span></span>
* <span data-ttu-id="a76a3-2908">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="a76a3-2908">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="a76a3-2909">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2909">Az.Profile</span></span>
* <span data-ttu-id="a76a3-2910">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a76a3-2910">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="a76a3-2911">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="a76a3-2911">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="a76a3-2912">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="a76a3-2912">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="a76a3-2913">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="a76a3-2913">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="a76a3-2914">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="a76a3-2914">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="a76a3-2915">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="a76a3-2915">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="a76a3-2916">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="a76a3-2916">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-2917">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2917">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-2918">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2918">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2919">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2919">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2920">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="a76a3-2920">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="a76a3-2921">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="a76a3-2921">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="a76a3-2922">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2922">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2923">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2923">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2924">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2924">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="a76a3-2925">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2925">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="a76a3-2926">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2926">Az.Insights</span></span>
* <span data-ttu-id="a76a3-2927">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="a76a3-2927">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="a76a3-2928">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="a76a3-2928">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="a76a3-2929">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="a76a3-2929">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="a76a3-2930">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="a76a3-2930">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2931">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2931">Az.Network</span></span>
* <span data-ttu-id="a76a3-2932">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="a76a3-2932">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="a76a3-2933">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-2933">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="a76a3-2934">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-2934">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="a76a3-2935">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a76a3-2935">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="a76a3-2936">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-2936">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="a76a3-2937">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="a76a3-2937">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="a76a3-2938">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a76a3-2938">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a76a3-2939">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a76a3-2939">Az.PolicyInsights</span></span>
* <span data-ttu-id="a76a3-2940">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="a76a3-2940">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2941">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2941">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2942">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="a76a3-2942">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="a76a3-2943">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2943">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a76a3-2944">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a76a3-2944">Az.ServiceBus</span></span>
* <span data-ttu-id="a76a3-2945">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2945">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a76a3-2946">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a76a3-2946">Az.ServiceFabric</span></span>
* <span data-ttu-id="a76a3-2947">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2947">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="a76a3-2948">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2948">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="a76a3-2949">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="a76a3-2949">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="a76a3-2950">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="a76a3-2950">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="a76a3-2951">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2951">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="a76a3-2952">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-2952">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="a76a3-2953">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2953">Az.Profile</span></span>
* <span data-ttu-id="a76a3-2954">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="a76a3-2954">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="a76a3-2955">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a76a3-2955">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2956">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2956">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2957">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="a76a3-2957">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="a76a3-2958">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2958">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a76a3-2959">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a76a3-2959">Az.DataLakeStore</span></span>
* <span data-ttu-id="a76a3-2960">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a76a3-2960">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="a76a3-2961">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2961">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="a76a3-2962">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2962">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a76a3-2963">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2963">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a76a3-2964">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2964">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2965">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2965">Az.Network</span></span>
* <span data-ttu-id="a76a3-2966">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2966">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="a76a3-2967">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2967">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-2968">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-2968">Az.Resources</span></span>
* <span data-ttu-id="a76a3-2969">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2969">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="a76a3-2970">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="a76a3-2970">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="a76a3-2971">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-2971">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="a76a3-2972">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2972">Azure.Storage</span></span>
* <span data-ttu-id="a76a3-2973">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="a76a3-2973">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="a76a3-2974">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2974">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="a76a3-2975">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a76a3-2975">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a76a3-2976">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2976">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="a76a3-2977">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="a76a3-2977">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a76a3-2978">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a76a3-2978">Az.CognitiveServices</span></span>
* <span data-ttu-id="a76a3-2979">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2979">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a76a3-2980">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a76a3-2980">Az.Compute</span></span>
* <span data-ttu-id="a76a3-2981">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="a76a3-2981">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="a76a3-2982">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2982">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="a76a3-2983">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="a76a3-2983">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="a76a3-2984">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a76a3-2984">Az.DataFactoryV2</span></span>
* <span data-ttu-id="a76a3-2985">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2985">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a76a3-2986">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a76a3-2986">Az.Network</span></span>
* <span data-ttu-id="a76a3-2987">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2987">Added NetworkProfile functionality.</span></span> <span data-ttu-id="a76a3-2988">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="a76a3-2988">new cmdlets added</span></span>
    - <span data-ttu-id="a76a3-2989">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2989">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="a76a3-2990">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2990">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="a76a3-2991">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2991">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="a76a3-2992">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a76a3-2992">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="a76a3-2993">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2993">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="a76a3-2994">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2994">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="a76a3-2995">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="a76a3-2995">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="a76a3-2996">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="a76a3-2996">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="a76a3-2997">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="a76a3-2997">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a76a3-2998">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a76a3-2998">Az.RedisCache</span></span>
* <span data-ttu-id="a76a3-2999">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="a76a3-2999">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="a76a3-3000">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="a76a3-3000">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="a76a3-3001">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a76a3-3001">Az.Resources</span></span>
* <span data-ttu-id="a76a3-3002">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a76a3-3002">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a76a3-3003">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="a76a3-3003">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="a76a3-3004">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a76a3-3004">Az.Sql</span></span>
* <span data-ttu-id="a76a3-3005">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="a76a3-3005">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a76a3-3006">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a76a3-3006">Az.Websites</span></span>
* <span data-ttu-id="a76a3-3007">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="a76a3-3007">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="a76a3-3008">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="a76a3-3008">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="a76a3-3009">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a76a3-3009">0.2.0 - September 2018</span></span>
 <span data-ttu-id="a76a3-3010">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a76a3-3010">Initial Release</span></span>
