---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: 3cb71087a61a0fcd06c014394e8f9e5654d4c1a8
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179008"
---
# <a name="release-notes"></a><span data-ttu-id="597c6-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="597c6-103">Release notes</span></span>

<span data-ttu-id="597c6-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="597c6-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="690---september-2018"></a><span data-ttu-id="597c6-105">6.9.0 - setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-105">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="597c6-106">Geral</span><span class="sxs-lookup"><span data-stu-id="597c6-106">General</span></span>
* <span data-ttu-id="597c6-107">AzureRM.SignalR foi adicionado ao módulo de rollup AzureRM</span><span class="sxs-lookup"><span data-stu-id="597c6-107">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="597c6-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-108">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-109">Alterações menores ao código comum do armazenamento</span><span class="sxs-lookup"><span data-stu-id="597c6-109">Minor changes to the storage common code</span></span>
* <span data-ttu-id="597c6-110">Ficheiros de ajuda atualizados para incluírem todos os tipos de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="597c6-110">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="597c6-111">-ServicePrincipal alterado para non-mandatory no conjunto de parâmetros ServicePrincipalCertificateWithSubscriptionId</span><span class="sxs-lookup"><span data-stu-id="597c6-111">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="597c6-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-112">Azure.Storage</span></span>
* <span data-ttu-id="597c6-113">Suporte para a criação de Contexto de Armazenamento com OAuth.</span><span class="sxs-lookup"><span data-stu-id="597c6-113">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="597c6-114">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="597c6-114">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="597c6-115">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="597c6-115">AzureRM.Cdn</span></span>
* <span data-ttu-id="597c6-116">Standard_Microsoft adicionado ao sku de preços de Cdn.</span><span class="sxs-lookup"><span data-stu-id="597c6-116">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-117">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-117">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-118">Dependências no Cofre de Chaves e no Armazenamento movidas para as dependências comuns</span><span class="sxs-lookup"><span data-stu-id="597c6-118">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="597c6-119">Adicionado suporte para mais tamanhos de máquinas virtuais para cmdlets do AEM</span><span class="sxs-lookup"><span data-stu-id="597c6-119">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="597c6-120">Adicionado o parâmetro PublicIPPrefix a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-120">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="597c6-121">Adicionado o parâmetro ResourceId ao cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="597c6-121">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="597c6-122">Adicionado o cmdlet Invoke-AzureRmVmssVMRunCommand cmdlet</span><span class="sxs-lookup"><span data-stu-id="597c6-122">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="597c6-123">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="597c6-123">AzureRM.Dns</span></span>
* <span data-ttu-id="597c6-124">Suporte adicionado para registo de alias durante a criação de registo dns</span><span class="sxs-lookup"><span data-stu-id="597c6-124">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="597c6-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="597c6-125">AzureRM.Insights</span></span>
* <span data-ttu-id="597c6-126">Corrigidos os problemas n.º 6833 e 7102 (Área Definições de Diagnóstico)</span><span class="sxs-lookup"><span data-stu-id="597c6-126">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="597c6-127">Problemas com o nome predefinido, ou seja, “serviço”, durante a criação e listagem/obtenção das definições de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="597c6-127">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="597c6-128">Problemas ao criar definições de diagnóstico com categorias</span><span class="sxs-lookup"><span data-stu-id="597c6-128">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="597c6-129">Adicionada mensagem de preterição aos parâmetros time grains das métricas</span><span class="sxs-lookup"><span data-stu-id="597c6-129">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="597c6-130">Os parâmetros timegrains ainda são aceites (esta não é uma alteração interruptiva), mas são ignorados no back-end, uma vez que apenas PT1M é válido</span><span class="sxs-lookup"><span data-stu-id="597c6-130">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-131">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-131">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-132">Alterações aos cmdlets LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="597c6-132">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="597c6-133">LoadBalancerInboundNatPoolConfig: parâmetros IdleTimeoutInMinutes, EnableFloatingIp e EnableTcpReset adicionados</span><span class="sxs-lookup"><span data-stu-id="597c6-133">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="597c6-134">LoadBalancerInboundNatRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-134">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="597c6-135">LoadBalancerRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-135">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="597c6-136">LoadBalancerProbeConfig: suporte para o valor "Https" para o parâmetro Protocol adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-136">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="597c6-137">Adicionados comandos novos para o sub-recurso OutboundRule de LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="597c6-137">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="597c6-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="597c6-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="597c6-140">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-140">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="597c6-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="597c6-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="597c6-143">Adicionada propriedade HostedWorkloads nova para PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="597c6-143">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="597c6-144">Adicionados cmdlets novos para a funcionalidade: Azure Firewall através de ARM</span><span class="sxs-lookup"><span data-stu-id="597c6-144">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="597c6-145">Get-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-145">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="597c6-146">Set-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-146">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="597c6-147">New-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-147">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="597c6-148">Remove-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-148">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="597c6-149">New-AzureRmFirewallApplicationRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-149">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="597c6-150">New-AzureRmFirewallApplicationRule adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-150">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="597c6-151">New-AzureRmFirewallNatRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-151">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="597c6-152">New-AzureRmFirewallNatRule adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-152">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="597c6-153">New-AzureRmFirewallNetworkRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-153">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="597c6-154">New-AzureRmFirewallNetworkRule adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-154">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="597c6-155">Adicionado suporte para o certificado de raiz fidedigna e configuração de dimensionamento automático no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="597c6-155">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="597c6-156">Novos cmdlets adicionados:</span><span class="sxs-lookup"><span data-stu-id="597c6-156">New Cmdlets added:</span></span>
      - <span data-ttu-id="597c6-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="597c6-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="597c6-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="597c6-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="597c6-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="597c6-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="597c6-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="597c6-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="597c6-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="597c6-166">Cmdlets updated with optonal parameter -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-166">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="597c6-167">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="597c6-167">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="597c6-168">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="597c6-168">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="597c6-169">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="597c6-169">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="597c6-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="597c6-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="597c6-171">Cmdlets atualizados com parâmetro opcional -AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-171">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="597c6-172">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="597c6-172">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="597c6-173">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="597c6-173">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="597c6-174">Adicionado cmdlet para Ponto Final da Interface Get-AzureInterfaceEndpoint</span><span class="sxs-lookup"><span data-stu-id="597c6-174">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="597c6-175">Adicionado suporte para vários prefixos de endereços numa sub-rede.</span><span class="sxs-lookup"><span data-stu-id="597c6-175">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="597c6-176">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="597c6-176">Updated cmdlets:</span></span>
  - <span data-ttu-id="597c6-177">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-177">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="597c6-178">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-178">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="597c6-179">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-179">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="597c6-180">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-180">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="597c6-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="597c6-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="597c6-183">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-183">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="597c6-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="597c6-185">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-185">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="597c6-186">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-186">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="597c6-187">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-187">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="597c6-188">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-188">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="597c6-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="597c6-190">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-190">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="597c6-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="597c6-192">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-192">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="597c6-193">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-193">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="597c6-194">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-194">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="597c6-195">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="597c6-195">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="597c6-196">Adição de cmdlets para delegação de sub-rede</span><span class="sxs-lookup"><span data-stu-id="597c6-196">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="597c6-197">New-AzureRmDelegation: cria uma delegação nova, que pode ser adicionada a uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="597c6-197">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="597c6-198">Remove-AzureRmDelegation: recebe uma sub-rede e remove o nome da delegação especificado dessa sub-rede</span><span class="sxs-lookup"><span data-stu-id="597c6-198">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="597c6-199">Add-AzureRmDelegation: recebe uma sub-rede e adiciona o nome de serviço especificado como delegação a essa sub-rede</span><span class="sxs-lookup"><span data-stu-id="597c6-199">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="597c6-200">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="597c6-200">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="597c6-201">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="597c6-201">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="597c6-202">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="597c6-202">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="597c6-203">Suporte para discos geridos</span><span class="sxs-lookup"><span data-stu-id="597c6-203">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="597c6-204">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="597c6-204">AzureRM.RedisCache</span></span>
* <span data-ttu-id="597c6-205">Dependência de informações atualizada</span><span class="sxs-lookup"><span data-stu-id="597c6-205">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-206">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-206">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-207">New-AzureRmResourceGroupDeployment atualizado com parâmetro novo RollbackAction</span><span class="sxs-lookup"><span data-stu-id="597c6-207">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="597c6-208">Adicionado suporte para OnErrorDeployment com o parâmetro novo.</span><span class="sxs-lookup"><span data-stu-id="597c6-208">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="597c6-209">Suporte para identidades geridas nas atribuições de políticas.</span><span class="sxs-lookup"><span data-stu-id="597c6-209">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="597c6-210">Os parâmetros com valores predefinidos já não são necessários ao atribuir uma política com “New-AzureRmPolicyAssignment”</span><span class="sxs-lookup"><span data-stu-id="597c6-210">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="597c6-211">Adicionado cmdlet novo Get-AzureRmPolicyAlias para obter aliases de políticas</span><span class="sxs-lookup"><span data-stu-id="597c6-211">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-212">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-212">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-213">Problema n.º 7161 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-213">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="597c6-214">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="597c6-214">AzureRM.SignalR</span></span>
* <span data-ttu-id="597c6-215">Nomes dos SKUs atualizados para Free_F1 e Standard_S1</span><span class="sxs-lookup"><span data-stu-id="597c6-215">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="597c6-216">Adicionado campo de versão ao objeto PSSignalRResource e cadeia de ligação ao objeto PSSignalRKeys.</span><span class="sxs-lookup"><span data-stu-id="597c6-216">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="597c6-217">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-217">AzureRM.Storage</span></span>
* <span data-ttu-id="597c6-218">Suporte para política Imutabilidade em AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-218">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="597c6-219">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="597c6-219">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="597c6-220">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="597c6-220">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="597c6-221">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="597c6-221">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="597c6-222">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="597c6-222">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="597c6-223">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="597c6-223">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="597c6-224">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="597c6-224">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="597c6-225">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="597c6-225">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="597c6-226">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-226">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="597c6-227">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-227">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="597c6-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="597c6-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="597c6-230">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="597c6-230">AzureRM.Websites</span></span>
* <span data-ttu-id="597c6-231">Adicionados dois cmdlets novos: Get-AzureRmDeletedWebApp e Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="597c6-231">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="597c6-232">O comutador New-AzureRmAppServicePlan -HyperV é adicionado para criar o plano do serviço de aplicações com contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="597c6-232">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="597c6-233">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - parâmetros novos (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) adicionados para criar e gerir a aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="597c6-233">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="597c6-234">6.8.1 - Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-234">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="597c6-235">Geral</span><span class="sxs-lookup"><span data-stu-id="597c6-235">General</span></span>
* <span data-ttu-id="597c6-236">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="597c6-236">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="597c6-237">Assemblagens de runtime comum atualizadas</span><span class="sxs-lookup"><span data-stu-id="597c6-237">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="597c6-238">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="597c6-238">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="597c6-239">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="597c6-239">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="597c6-240">Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-240">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="597c6-241">Agora, os cmdlets Import-AzureRmApiManagementApi e \*-AzureRmApiManagementCertificate identificam caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="597c6-241">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="597c6-242">Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-242">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="597c6-243">O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="597c6-243">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="597c6-244">Corrigido com a atualização para 4.0.4-nuget de pré-visualização</span><span class="sxs-lookup"><span data-stu-id="597c6-244">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="597c6-245">Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-245">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="597c6-246">Foi corrigido o filtro de Odata para procurar por nome de produto</span><span class="sxs-lookup"><span data-stu-id="597c6-246">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="597c6-247">Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-247">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="597c6-248">Foi corrigido o filtro de Odata para procurar por nome na API</span><span class="sxs-lookup"><span data-stu-id="597c6-248">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="597c6-249">Foi adicionado suporte para o logger de AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="597c6-249">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="597c6-250">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-250">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-251">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="597c6-251">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="597c6-252">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="597c6-252">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="597c6-253">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="597c6-253">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="597c6-254">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="597c6-254">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-255">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-255">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-256">Representação de saída de cmdlet predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="597c6-256">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="597c6-257">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="597c6-257">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="597c6-258">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="597c6-258">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="597c6-259">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-259">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-260">Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="597c6-260">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-261">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-261">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-262">Problemas corrigidos</span><span class="sxs-lookup"><span data-stu-id="597c6-262">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="597c6-263">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="597c6-263">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="597c6-264">Suporte adicionado para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="597c6-264">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="597c6-265">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="597c6-265">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="597c6-266">Suporte adicionado para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="597c6-266">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="597c6-267">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="597c6-267">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="597c6-268">Suporte adicionado para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="597c6-268">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="597c6-269">Suporte adicionado para intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="597c6-269">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="597c6-270">Suporte adicionado para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="597c6-270">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="597c6-271">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-271">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="597c6-272">Geral</span><span class="sxs-lookup"><span data-stu-id="597c6-272">General</span></span>
* <span data-ttu-id="597c6-273">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="597c6-273">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="597c6-274">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-274">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-275">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="597c6-275">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-276">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-276">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-277">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="597c6-277">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="597c6-278">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="597c6-278">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="597c6-279">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="597c6-279">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="597c6-280">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="597c6-280">AzureRM.IotHub</span></span>
* <span data-ttu-id="597c6-281">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="597c6-281">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-282">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-282">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-283">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="597c6-283">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="597c6-284">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="597c6-284">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="597c6-285">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="597c6-285">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-286">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-286">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-287">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="597c6-287">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-289">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="597c6-289">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="597c6-290">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="597c6-290">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="597c6-291">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="597c6-291">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="597c6-292">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="597c6-292">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="597c6-293">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="597c6-293">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="597c6-294">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="597c6-294">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="597c6-295">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="597c6-295">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="597c6-296">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="597c6-296">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="597c6-297">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="597c6-297">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="597c6-298">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="597c6-298">AzureRM.Websites</span></span>
* <span data-ttu-id="597c6-299">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="597c6-299">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="597c6-300">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-300">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="597c6-301">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-301">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-302">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-302">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="597c6-303">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="597c6-303">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="597c6-304">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="597c6-304">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="597c6-305">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="597c6-305">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="597c6-306">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-306">Azure.Storage</span></span>
* <span data-ttu-id="597c6-307">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="597c6-307">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="597c6-308">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="597c6-308">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="597c6-309">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="597c6-309">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="597c6-310">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="597c6-311">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="597c6-311">Azure.AnalysisServices</span></span>
* <span data-ttu-id="597c6-312">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="597c6-313">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="597c6-313">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="597c6-314">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="597c6-315">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="597c6-315">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="597c6-316">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-316">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="597c6-317">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="597c6-317">AzureRM.Automation</span></span>
* <span data-ttu-id="597c6-318">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-318">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="597c6-319">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="597c6-319">AzureRM.Backup</span></span>
* <span data-ttu-id="597c6-320">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-320">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="597c6-321">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="597c6-321">AzureRM.Batch</span></span>
* <span data-ttu-id="597c6-322">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-322">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="597c6-323">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="597c6-323">AzureRM.Billing</span></span>
* <span data-ttu-id="597c6-324">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-324">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="597c6-325">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="597c6-325">AzureRM.Cdn</span></span>
* <span data-ttu-id="597c6-326">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-326">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="597c6-327">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="597c6-327">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="597c6-328">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-328">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-329">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-329">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-330">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-330">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="597c6-331">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-331">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="597c6-332">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="597c6-332">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="597c6-333">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="597c6-333">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="597c6-334">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="597c6-334">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="597c6-335">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="597c6-335">AzureRM.Consumption</span></span>
* <span data-ttu-id="597c6-336">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-336">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="597c6-337">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="597c6-337">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="597c6-338">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-338">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="597c6-339">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="597c6-339">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="597c6-340">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-340">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="597c6-341">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="597c6-341">AzureRM.DataFactories</span></span>
* <span data-ttu-id="597c6-342">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-342">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="597c6-343">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="597c6-343">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="597c6-344">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-344">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="597c6-345">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="597c6-345">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="597c6-346">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-346">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="597c6-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="597c6-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="597c6-348">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="597c6-348">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="597c6-349">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="597c6-349">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="597c6-350">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-350">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="597c6-351">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="597c6-351">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="597c6-352">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="597c6-352">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="597c6-353">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="597c6-354">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="597c6-354">AzureRM.Dns</span></span>
* <span data-ttu-id="597c6-355">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="597c6-356">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="597c6-356">AzureRM.EventGrid</span></span>
* <span data-ttu-id="597c6-357">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="597c6-358">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="597c6-358">AzureRM.EventHub</span></span>
* <span data-ttu-id="597c6-359">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="597c6-360">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="597c6-360">AzureRM.HDInsight</span></span>
* <span data-ttu-id="597c6-361">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="597c6-362">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="597c6-362">AzureRM.Insights</span></span>
* <span data-ttu-id="597c6-363">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="597c6-364">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="597c6-364">AzureRM.IotHub</span></span>
* <span data-ttu-id="597c6-365">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="597c6-366">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="597c6-366">AzureRM.KeyVault</span></span>
* <span data-ttu-id="597c6-367">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="597c6-368">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="597c6-368">AzureRM.LogicApp</span></span>
* <span data-ttu-id="597c6-369">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-369">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="597c6-370">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="597c6-370">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="597c6-371">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-371">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="597c6-372">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="597c6-372">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="597c6-373">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-373">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="597c6-374">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="597c6-374">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="597c6-375">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="597c6-376">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="597c6-376">AzureRM.Media</span></span>
* <span data-ttu-id="597c6-377">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-378">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-378">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-379">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="597c6-379">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="597c6-380">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="597c6-380">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="597c6-381">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="597c6-381">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="597c6-382">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="597c6-382">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="597c6-383">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="597c6-383">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="597c6-384">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="597c6-384">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="597c6-385">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="597c6-385">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="597c6-386">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="597c6-386">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="597c6-387">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="597c6-387">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="597c6-388">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="597c6-389">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="597c6-389">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="597c6-390">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-390">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="597c6-391">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="597c6-391">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="597c6-392">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="597c6-393">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="597c6-393">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="597c6-394">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="597c6-395">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="597c6-395">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="597c6-396">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="597c6-397">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="597c6-397">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="597c6-398">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="597c6-398">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="597c6-399">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="597c6-399">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="597c6-400">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="597c6-400">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="597c6-401">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-401">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="597c6-402">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="597c6-402">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="597c6-403">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="597c6-403">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="597c6-404">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="597c6-404">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="597c6-405">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="597c6-405">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="597c6-406">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="597c6-407">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="597c6-407">AzureRM.RedisCache</span></span>
* <span data-ttu-id="597c6-408">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="597c6-409">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="597c6-409">AzureRM.Relay</span></span>
* <span data-ttu-id="597c6-410">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-411">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-411">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-412">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="597c6-412">Support template deployment at subscription scope.</span></span> <span data-ttu-id="597c6-413">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="597c6-413">Add new Cmdlets:</span></span>
    - <span data-ttu-id="597c6-414">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-414">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="597c6-415">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-415">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="597c6-416">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-416">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="597c6-417">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-417">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="597c6-418">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-418">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="597c6-419">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="597c6-419">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="597c6-420">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="597c6-420">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="597c6-421">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="597c6-421">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="597c6-422">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-422">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="597c6-423">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="597c6-424">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="597c6-424">AzureRM.Scheduler</span></span>
* <span data-ttu-id="597c6-425">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-426">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-426">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-427">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="597c6-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="597c6-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="597c6-429">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="597c6-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-430">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-431">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="597c6-432">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-432">AzureRM.Storage</span></span>
* <span data-ttu-id="597c6-433">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="597c6-434">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="597c6-434">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="597c6-435">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="597c6-436">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="597c6-436">AzureRM.Tags</span></span>
* <span data-ttu-id="597c6-437">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="597c6-438">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="597c6-438">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="597c6-439">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-439">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="597c6-440">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="597c6-440">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="597c6-441">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-441">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="597c6-442">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="597c6-442">AzureRM.Websites</span></span>
* <span data-ttu-id="597c6-443">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-443">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="597c6-444">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-444">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="597c6-445">Geral</span><span class="sxs-lookup"><span data-stu-id="597c6-445">General</span></span>
* <span data-ttu-id="597c6-446">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="597c6-446">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="597c6-447">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-447">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-448">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="597c6-448">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="597c6-449">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-449">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="597c6-450">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-450">Azure.Storage</span></span>
* <span data-ttu-id="597c6-451">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="597c6-451">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="597c6-452">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="597c6-452">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="597c6-453">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="597c6-453">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="597c6-454">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-454">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="597c6-455">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="597c6-455">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="597c6-456">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-456">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="597c6-457">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="597c6-457">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="597c6-458">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="597c6-458">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="597c6-459">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="597c6-459">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-460">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-460">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-461">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="597c6-461">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="597c6-462">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="597c6-462">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="597c6-463">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="597c6-463">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="597c6-464">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="597c6-464">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="597c6-465">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="597c6-465">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="597c6-466">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="597c6-466">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="597c6-467">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="597c6-467">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="597c6-468">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="597c6-468">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="597c6-469">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="597c6-469">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="597c6-470">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="597c6-470">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="597c6-471">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="597c6-471">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="597c6-472">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="597c6-472">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="597c6-473">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="597c6-473">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="597c6-474">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-474">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="597c6-475">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="597c6-475">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="597c6-476">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="597c6-476">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="597c6-477">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="597c6-477">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="597c6-478">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="597c6-478">AzureRM.EventHub</span></span>
* <span data-ttu-id="597c6-479">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="597c6-479">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="597c6-480">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="597c6-480">AzureRM.Insights</span></span>
* <span data-ttu-id="597c6-481">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="597c6-481">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="597c6-482">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="597c6-482">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="597c6-483">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="597c6-483">AzureRM.KeyVault</span></span>
* <span data-ttu-id="597c6-484">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-484">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-485">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-485">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-486">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="597c6-486">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-487">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-487">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-488">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="597c6-488">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="597c6-489">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="597c6-489">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-490">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-490">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-491">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="597c6-491">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="597c6-492">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="597c6-492">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="597c6-493">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-493">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-494">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="597c6-494">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="597c6-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="597c6-496">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="597c6-496">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="597c6-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="597c6-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="597c6-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="597c6-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="597c6-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="597c6-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="597c6-500">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="597c6-500">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="597c6-501">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="597c6-501">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="597c6-502">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-502">AzureRM.Storage</span></span>
* <span data-ttu-id="597c6-503">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="597c6-503">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="597c6-504">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="597c6-504">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="597c6-505">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="597c6-505">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="597c6-506">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="597c6-506">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="597c6-507">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="597c6-507">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="597c6-508">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="597c6-508">AzureRM.Tags</span></span>
* <span data-ttu-id="597c6-509">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="597c6-509">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="597c6-510">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-510">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="597c6-511">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-511">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-512">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="597c6-512">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="597c6-513">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-513">Azure.Storage</span></span>
* <span data-ttu-id="597c6-514">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="597c6-514">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="597c6-515">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="597c6-515">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="597c6-516">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="597c6-516">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="597c6-517">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="597c6-517">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="597c6-518">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="597c6-518">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="597c6-519">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="597c6-519">AzureRM.Automation</span></span>
* <span data-ttu-id="597c6-520">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="597c6-520">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-521">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-522">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="597c6-522">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="597c6-523">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="597c6-523">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="597c6-524">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="597c6-524">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="597c6-525">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="597c6-525">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="597c6-526">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="597c6-526">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="597c6-527">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="597c6-527">AzureRM.EventHub</span></span>
* <span data-ttu-id="597c6-528">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="597c6-528">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="597c6-529">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="597c6-529">AzureRM.KeyVault</span></span>
* <span data-ttu-id="597c6-530">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="597c6-530">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="597c6-531">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="597c6-531">AzureRM.LogicApp</span></span>
* <span data-ttu-id="597c6-532">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="597c6-532">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-533">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-534">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="597c6-534">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="597c6-535">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="597c6-535">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="597c6-536">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="597c6-536">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="597c6-537">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="597c6-537">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="597c6-538">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="597c6-538">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="597c6-539">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="597c6-539">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="597c6-540">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="597c6-540">AzureRM.Relay</span></span>
* <span data-ttu-id="597c6-541">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="597c6-541">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-542">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-542">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-543">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="597c6-543">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="597c6-544">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="597c6-544">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="597c6-545">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="597c6-545">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="597c6-546">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="597c6-546">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="597c6-547">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="597c6-547">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-548">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-548">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-549">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="597c6-549">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="597c6-550">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="597c6-550">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="597c6-551">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="597c6-551">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="597c6-552">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="597c6-552">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="597c6-553">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="597c6-553">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="597c6-554">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="597c6-554">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="597c6-555">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="597c6-555">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="597c6-556">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="597c6-556">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="597c6-557">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="597c6-557">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="597c6-558">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="597c6-558">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="597c6-559">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-559">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-560">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="597c6-560">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="597c6-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="597c6-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="597c6-563">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="597c6-563">AzureRM.Websites</span></span>
* <span data-ttu-id="597c6-564">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="597c6-564">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="597c6-565">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="597c6-565">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="597c6-566">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="597c6-566">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="597c6-567">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-567">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="597c6-568">Geral</span><span class="sxs-lookup"><span data-stu-id="597c6-568">General</span></span>
* <span data-ttu-id="597c6-569">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="597c6-569">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="597c6-570">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-570">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-571">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="597c6-571">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-572">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-572">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-573">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="597c6-573">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="597c6-574">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="597c6-574">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="597c6-575">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-575">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="597c6-576">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="597c6-576">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="597c6-577">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-577">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="597c6-578">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="597c6-578">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="597c6-579">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-579">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="597c6-580">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="597c6-580">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="597c6-581">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="597c6-581">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="597c6-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="597c6-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="597c6-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="597c6-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="597c6-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="597c6-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="597c6-585">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="597c6-585">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="597c6-586">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="597c6-586">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="597c6-587">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="597c6-587">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="597c6-588">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="597c6-588">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="597c6-589">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="597c6-589">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="597c6-590">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="597c6-590">AzureRM.EventHub</span></span>
* <span data-ttu-id="597c6-591">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="597c6-591">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="597c6-592">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="597c6-592">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="597c6-593">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="597c6-593">Provided Default Parameter set.</span></span>
* <span data-ttu-id="597c6-594">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="597c6-594">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="597c6-595">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="597c6-595">AzureRM.KeyVault</span></span>
* <span data-ttu-id="597c6-596">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="597c6-596">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-597">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-597">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-598">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="597c6-598">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="597c6-599">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="597c6-599">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="597c6-600">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="597c6-600">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="597c6-601">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="597c6-601">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="597c6-602">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="597c6-602">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="597c6-603">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="597c6-603">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="597c6-604">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="597c6-604">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="597c6-605">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="597c6-605">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="597c6-606">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="597c6-606">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="597c6-607">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="597c6-607">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="597c6-608">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="597c6-608">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="597c6-609">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="597c6-609">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="597c6-610">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="597c6-610">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="597c6-611">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="597c6-611">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-612">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-612">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-613">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="597c6-613">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="597c6-614">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="597c6-614">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="597c6-615">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="597c6-615">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="597c6-616">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="597c6-616">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="597c6-617">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="597c6-617">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="597c6-618">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="597c6-618">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="597c6-619">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="597c6-619">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="597c6-620">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="597c6-620">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="597c6-621">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="597c6-621">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="597c6-622">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="597c6-622">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="597c6-623">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="597c6-623">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="597c6-624">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="597c6-624">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="597c6-625">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="597c6-625">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="597c6-626">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="597c6-626">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="597c6-627">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="597c6-627">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="597c6-628">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-628">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-629">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="597c6-629">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="597c6-630">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="597c6-630">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="597c6-631">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-631">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="597c6-632">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-632">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-633">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="597c6-633">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="597c6-634">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="597c6-634">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="597c6-635">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="597c6-635">Azure.Storage</span></span>
* <span data-ttu-id="597c6-636">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="597c6-636">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-637">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-637">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-638">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="597c6-638">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="597c6-639">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="597c6-639">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="597c6-640">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="597c6-640">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="597c6-641">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="597c6-641">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="597c6-642">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="597c6-642">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="597c6-643">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="597c6-643">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="597c6-644">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="597c6-644">Start-AzureRmVM</span></span>
    - <span data-ttu-id="597c6-645">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="597c6-645">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="597c6-646">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="597c6-646">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="597c6-647">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="597c6-647">Set-AzureRmVM</span></span>
    - <span data-ttu-id="597c6-648">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="597c6-648">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="597c6-649">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-649">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="597c6-650">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="597c6-650">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="597c6-651">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="597c6-651">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="597c6-652">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-652">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="597c6-653">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-653">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="597c6-654">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-654">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="597c6-655">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="597c6-655">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="597c6-656">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="597c6-656">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="597c6-657">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="597c6-657">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="597c6-658">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="597c6-658">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="597c6-659">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="597c6-659">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="597c6-660">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="597c6-660">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="597c6-661">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="597c6-661">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="597c6-662">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="597c6-662">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="597c6-663">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="597c6-663">AzureRM.EventGrid</span></span>
* <span data-ttu-id="597c6-664">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="597c6-664">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="597c6-665">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="597c6-665">AzureRM.KeyVault</span></span>
* <span data-ttu-id="597c6-666">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="597c6-666">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="597c6-667">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="597c6-667">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="597c6-668">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="597c6-668">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="597c6-669">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="597c6-669">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="597c6-670">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="597c6-670">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="597c6-671">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="597c6-671">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="597c6-672">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="597c6-672">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="597c6-673">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="597c6-673">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="597c6-674">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-674">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-675">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="597c6-675">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="597c6-676">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="597c6-676">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="597c6-677">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-677">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="597c6-678">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="597c6-678">AzureRM.Websites</span></span>
* <span data-ttu-id="597c6-679">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="597c6-679">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="597c6-680">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="597c6-680">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="597c6-681">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-681">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="597c6-682">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="597c6-682">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="597c6-683">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="597c6-683">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="597c6-684">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-684">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="597c6-685">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-685">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-686">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="597c6-686">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="597c6-687">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="597c6-687">AzureRM.Compute</span></span>
* <span data-ttu-id="597c6-688">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="597c6-688">VMSS VM Update feature</span></span>
    - <span data-ttu-id="597c6-689">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="597c6-689">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="597c6-690">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="597c6-690">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="597c6-691">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="597c6-691">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="597c6-692">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="597c6-692">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="597c6-693">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="597c6-693">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="597c6-694">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="597c6-694">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="597c6-695">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="597c6-695">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="597c6-696">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="597c6-696">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="597c6-697">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="597c6-697">AzureRM.KeyVault</span></span>
* <span data-ttu-id="597c6-698">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="597c6-698">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="597c6-699">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-699">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-700">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="597c6-700">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="597c6-701">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="597c6-701">AzureRM.Resources</span></span>
* <span data-ttu-id="597c6-702">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="597c6-702">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="597c6-703">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="597c6-703">AzureRM.Scheduler</span></span>
* <span data-ttu-id="597c6-704">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="597c6-704">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="597c6-705">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-705">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-706">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="597c6-706">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="597c6-707">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="597c6-707">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="597c6-708">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="597c6-708">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="597c6-709">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="597c6-709">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="597c6-710">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="597c6-710">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="597c6-711">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="597c6-711">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="597c6-712">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="597c6-712">AzureRM.Websites</span></span>
* <span data-ttu-id="597c6-713">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="597c6-713">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="597c6-714">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="597c6-714">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="597c6-715">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="597c6-715">AzureRM.Profile</span></span>
* <span data-ttu-id="597c6-716">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="597c6-716">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="597c6-717">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="597c6-717">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="597c6-718">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="597c6-718">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="597c6-719">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="597c6-719">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="597c6-720">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="597c6-720">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="597c6-721">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="597c6-721">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="597c6-722">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="597c6-722">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="597c6-723">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="597c6-723">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="597c6-724">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="597c6-724">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="597c6-725">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="597c6-725">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="597c6-726">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="597c6-726">Added support for MSI identity</span></span>
* <span data-ttu-id="597c6-727">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="597c6-727">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="597c6-728">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="597c6-728">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="597c6-729">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-729">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="597c6-730">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="597c6-730">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="597c6-731">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="597c6-731">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="597c6-732">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="597c6-732">AzureRM.Batch</span></span>
* <span data-ttu-id="597c6-733">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="597c6-733">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="597c6-734">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="597c6-734">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="597c6-735">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="597c6-735">AzureRM.Consumption</span></span>
* <span data-ttu-id="597c6-736">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="597c6-736">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="597c6-737">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="597c6-737">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="597c6-738">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="597c6-738">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="597c6-739">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="597c6-739">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="597c6-740">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="597c6-740">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="597c6-741">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="597c6-741">AzureRM.Network</span></span>
* <span data-ttu-id="597c6-742">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="597c6-742">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="597c6-743">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="597c6-743">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="597c6-744">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="597c6-744">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="597c6-745">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="597c6-745">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="597c6-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="597c6-747">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="597c6-747">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="597c6-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="597c6-749">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="597c6-749">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="597c6-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="597c6-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="597c6-751">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="597c6-751">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="597c6-752">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="597c6-752">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="597c6-753">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="597c6-753">AzureRM.Sql</span></span>
* <span data-ttu-id="597c6-754">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="597c6-754">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="597c6-755">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="597c6-755">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="597c6-756">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="597c6-756">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="597c6-757">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="597c6-757">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="597c6-758">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="597c6-758">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="597c6-759">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="597c6-759">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="597c6-760">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="597c6-760">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="597c6-761">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="597c6-761">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="597c6-762">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="597c6-762">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="597c6-763">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="597c6-763">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="597c6-764">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="597c6-764">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="597c6-765">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="597c6-765">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
