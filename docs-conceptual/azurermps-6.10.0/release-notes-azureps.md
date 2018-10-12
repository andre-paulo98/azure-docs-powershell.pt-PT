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
ms.openlocfilehash: 6a33d1a85fc61d0281bf1183163185b0dc4d3a12
ms.sourcegitcommit: a749eb729f583c9d0dd86141bbd04984d77ae9ab
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/11/2018
ms.locfileid: "48882246"
---
# <a name="release-notes"></a><span data-ttu-id="9a01f-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="9a01f-103">Release notes</span></span>

<span data-ttu-id="9a01f-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="9a01f-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6100---october-2018"></a><span data-ttu-id="9a01f-105">6.10.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-105">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="9a01f-106">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-106">Azure.Storage</span></span>
* <span data-ttu-id="9a01f-107">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="9a01f-107">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="9a01f-108">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="9a01f-108">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="9a01f-109">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="9a01f-109">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="9a01f-110">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-110">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="9a01f-111">Suporte para Get-AzureRmCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="9a01f-111">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-112">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-112">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-113">Correção de Get-AzureRmVM -ResourceGroupName <rg> para devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="9a01f-113">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="9a01f-114">Adição de um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzureRmVmss.</span><span class="sxs-lookup"><span data-stu-id="9a01f-114">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="9a01f-115">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="9a01f-115">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9a01f-116">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9a01f-116">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9a01f-117">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="9a01f-117">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-118">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-118">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-119">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="9a01f-119">Added NetworkProfile functionality.</span></span> <span data-ttu-id="9a01f-120">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="9a01f-120">new cmdlets added</span></span>
    - <span data-ttu-id="9a01f-121">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9a01f-121">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9a01f-122">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9a01f-122">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9a01f-123">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9a01f-123">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9a01f-124">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9a01f-124">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9a01f-125">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-125">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="9a01f-126">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-126">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="9a01f-127">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-127">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="9a01f-128">Adição do cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="9a01f-128">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="9a01f-129">Adição do cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-129">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="9a01f-130">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9a01f-130">AzureRM.RedisCache</span></span>
* <span data-ttu-id="9a01f-131">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="9a01f-131">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="9a01f-132">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="9a01f-132">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-133">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-133">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-134">Adição do parâmetro -Mode em falta a Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9a01f-134">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="9a01f-135">Correção do erro de commandlet Get-AzureRmProviderOperation para as operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="9a01f-135">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-136">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-136">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-137">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="9a01f-137">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9a01f-138">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-138">AzureRM.Storage</span></span>
* <span data-ttu-id="9a01f-139">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="9a01f-139">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="9a01f-140">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="9a01f-140">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-141">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-141">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-142">Novo Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="9a01f-142">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="9a01f-143">Novos Cmdlets New-AzureRMWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="9a01f-143">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="9a01f-144">6.9.0 - setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-144">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9a01f-145">Geral</span><span class="sxs-lookup"><span data-stu-id="9a01f-145">General</span></span>
* <span data-ttu-id="9a01f-146">AzureRM.SignalR foi adicionado ao módulo de rollup AzureRM</span><span class="sxs-lookup"><span data-stu-id="9a01f-146">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-147">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-147">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-148">Alterações menores ao código comum do armazenamento</span><span class="sxs-lookup"><span data-stu-id="9a01f-148">Minor changes to the storage common code</span></span>
* <span data-ttu-id="9a01f-149">Ficheiros de ajuda atualizados para incluírem todos os tipos de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9a01f-149">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="9a01f-150">-ServicePrincipal alterado para non-mandatory no conjunto de parâmetros ServicePrincipalCertificateWithSubscriptionId</span><span class="sxs-lookup"><span data-stu-id="9a01f-150">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="9a01f-151">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-151">Azure.Storage</span></span>
* <span data-ttu-id="9a01f-152">Suporte para a criação de Contexto de Armazenamento com OAuth.</span><span class="sxs-lookup"><span data-stu-id="9a01f-152">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="9a01f-153">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="9a01f-153">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="9a01f-154">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="9a01f-154">AzureRM.Cdn</span></span>
* <span data-ttu-id="9a01f-155">Standard_Microsoft adicionado ao sku de preços de Cdn.</span><span class="sxs-lookup"><span data-stu-id="9a01f-155">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-156">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-156">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-157">Dependências no Cofre de Chaves e no Armazenamento movidas para as dependências comuns</span><span class="sxs-lookup"><span data-stu-id="9a01f-157">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="9a01f-158">Adicionado suporte para mais tamanhos de máquinas virtuais para cmdlets do AEM</span><span class="sxs-lookup"><span data-stu-id="9a01f-158">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="9a01f-159">Adicionado o parâmetro PublicIPPrefix a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-159">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="9a01f-160">Adicionado o parâmetro ResourceId ao cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="9a01f-160">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="9a01f-161">Adicionado o cmdlet Invoke-AzureRmVmssVMRunCommand cmdlet</span><span class="sxs-lookup"><span data-stu-id="9a01f-161">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="9a01f-162">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="9a01f-162">AzureRM.Dns</span></span>
* <span data-ttu-id="9a01f-163">Suporte adicionado para registo de alias durante a criação de registo dns</span><span class="sxs-lookup"><span data-stu-id="9a01f-163">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9a01f-164">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9a01f-164">AzureRM.Insights</span></span>
* <span data-ttu-id="9a01f-165">Corrigidos os problemas n.º 6833 e 7102 (Área Definições de Diagnóstico)</span><span class="sxs-lookup"><span data-stu-id="9a01f-165">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="9a01f-166">Problemas com o nome predefinido, ou seja, “serviço”, durante a criação e listagem/obtenção das definições de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="9a01f-166">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="9a01f-167">Problemas ao criar definições de diagnóstico com categorias</span><span class="sxs-lookup"><span data-stu-id="9a01f-167">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="9a01f-168">Adicionada mensagem de preterição aos parâmetros time grains das métricas</span><span class="sxs-lookup"><span data-stu-id="9a01f-168">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="9a01f-169">Os parâmetros timegrains ainda são aceites (esta não é uma alteração interruptiva), mas são ignorados no back-end, uma vez que apenas PT1M é válido</span><span class="sxs-lookup"><span data-stu-id="9a01f-169">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-170">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-170">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-171">Alterações aos cmdlets LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="9a01f-171">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="9a01f-172">LoadBalancerInboundNatPoolConfig: parâmetros IdleTimeoutInMinutes, EnableFloatingIp e EnableTcpReset adicionados</span><span class="sxs-lookup"><span data-stu-id="9a01f-172">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="9a01f-173">LoadBalancerInboundNatRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-173">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="9a01f-174">LoadBalancerRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-174">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="9a01f-175">LoadBalancerProbeConfig: suporte para o valor "Https" para o parâmetro Protocol adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-175">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="9a01f-176">Adicionados comandos novos para o sub-recurso OutboundRule de LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="9a01f-176">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="9a01f-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9a01f-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9a01f-179">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-179">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9a01f-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9a01f-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="9a01f-182">Adicionada propriedade HostedWorkloads nova para PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="9a01f-182">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="9a01f-183">Adicionados cmdlets novos para a funcionalidade: Azure Firewall através de ARM</span><span class="sxs-lookup"><span data-stu-id="9a01f-183">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="9a01f-184">Get-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-184">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="9a01f-185">Set-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-185">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="9a01f-186">New-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-186">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="9a01f-187">Remove-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-187">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="9a01f-188">New-AzureRmFirewallApplicationRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-188">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="9a01f-189">New-AzureRmFirewallApplicationRule adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-189">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="9a01f-190">New-AzureRmFirewallNatRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-190">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="9a01f-191">New-AzureRmFirewallNatRule adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-191">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="9a01f-192">New-AzureRmFirewallNetworkRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-192">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="9a01f-193">New-AzureRmFirewallNetworkRule adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-193">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="9a01f-194">Adicionado suporte para o certificado de raiz fidedigna e configuração de dimensionamento automático no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="9a01f-194">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="9a01f-195">Novos cmdlets adicionados:</span><span class="sxs-lookup"><span data-stu-id="9a01f-195">New Cmdlets added:</span></span>
      - <span data-ttu-id="9a01f-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9a01f-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9a01f-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9a01f-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9a01f-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9a01f-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="9a01f-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="9a01f-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="9a01f-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="9a01f-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="9a01f-206">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9a01f-206">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="9a01f-207">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9a01f-207">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="9a01f-208">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="9a01f-208">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="9a01f-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="9a01f-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="9a01f-210">Cmdlets atualizados com parâmetro opcional -AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-210">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="9a01f-211">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9a01f-211">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="9a01f-212">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9a01f-212">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="9a01f-213">Adicionado cmdlet para Ponto Final da Interface Get-AzureInterfaceEndpoint</span><span class="sxs-lookup"><span data-stu-id="9a01f-213">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="9a01f-214">Adicionado suporte para vários prefixos de endereços numa sub-rede.</span><span class="sxs-lookup"><span data-stu-id="9a01f-214">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="9a01f-215">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="9a01f-215">Updated cmdlets:</span></span>
  - <span data-ttu-id="9a01f-216">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-216">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9a01f-217">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-217">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9a01f-218">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-218">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9a01f-219">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-219">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9a01f-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="9a01f-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="9a01f-222">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-222">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="9a01f-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="9a01f-224">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-224">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="9a01f-225">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-225">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="9a01f-226">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-226">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="9a01f-227">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-227">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="9a01f-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="9a01f-229">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-229">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="9a01f-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="9a01f-231">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-231">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="9a01f-232">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-232">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="9a01f-233">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-233">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="9a01f-234">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="9a01f-234">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="9a01f-235">Adição de cmdlets para delegação de sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-235">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="9a01f-236">New-AzureRmDelegation: cria uma delegação nova, que pode ser adicionada a uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-236">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="9a01f-237">Remove-AzureRmDelegation: recebe uma sub-rede e remove o nome da delegação especificado dessa sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-237">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="9a01f-238">Add-AzureRmDelegation: recebe uma sub-rede e adiciona o nome de serviço especificado como delegação a essa sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-238">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="9a01f-239">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="9a01f-239">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="9a01f-240">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="9a01f-240">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9a01f-241">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9a01f-241">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="9a01f-242">Suporte para discos geridos</span><span class="sxs-lookup"><span data-stu-id="9a01f-242">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="9a01f-243">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9a01f-243">AzureRM.RedisCache</span></span>
* <span data-ttu-id="9a01f-244">Dependência de informações atualizada</span><span class="sxs-lookup"><span data-stu-id="9a01f-244">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-245">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-246">New-AzureRmResourceGroupDeployment atualizado com parâmetro novo RollbackAction</span><span class="sxs-lookup"><span data-stu-id="9a01f-246">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="9a01f-247">Adicionado suporte para OnErrorDeployment com o parâmetro novo.</span><span class="sxs-lookup"><span data-stu-id="9a01f-247">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="9a01f-248">Suporte para identidades geridas nas atribuições de políticas.</span><span class="sxs-lookup"><span data-stu-id="9a01f-248">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="9a01f-249">Os parâmetros com valores predefinidos já não são necessários ao atribuir uma política com “New-AzureRmPolicyAssignment”</span><span class="sxs-lookup"><span data-stu-id="9a01f-249">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="9a01f-250">Adicionado cmdlet novo Get-AzureRmPolicyAlias para obter aliases de políticas</span><span class="sxs-lookup"><span data-stu-id="9a01f-250">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-251">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-251">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-252">Problema n.º 7161 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-252">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="9a01f-253">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="9a01f-253">AzureRM.SignalR</span></span>
* <span data-ttu-id="9a01f-254">Nomes dos SKUs atualizados para Free_F1 e Standard_S1</span><span class="sxs-lookup"><span data-stu-id="9a01f-254">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="9a01f-255">Adicionado campo de versão ao objeto PSSignalRResource e cadeia de ligação ao objeto PSSignalRKeys.</span><span class="sxs-lookup"><span data-stu-id="9a01f-255">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9a01f-256">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-256">AzureRM.Storage</span></span>
* <span data-ttu-id="9a01f-257">Suporte para política Imutabilidade em AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-257">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="9a01f-258">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="9a01f-258">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="9a01f-259">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9a01f-259">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9a01f-260">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9a01f-260">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9a01f-261">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9a01f-261">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9a01f-262">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9a01f-262">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9a01f-263">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="9a01f-263">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="9a01f-264">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="9a01f-264">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="9a01f-265">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-265">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="9a01f-266">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-266">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="9a01f-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="9a01f-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-269">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-269">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-270">Adicionados dois cmdlets novos: Get-AzureRmDeletedWebApp e Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="9a01f-270">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="9a01f-271">O comutador New-AzureRmAppServicePlan -HyperV é adicionado para criar o plano do serviço de aplicações com contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="9a01f-271">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="9a01f-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - parâmetros novos (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) adicionados para criar e gerir a aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="9a01f-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="9a01f-273">6.8.1 - Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-273">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9a01f-274">Geral</span><span class="sxs-lookup"><span data-stu-id="9a01f-274">General</span></span>
* <span data-ttu-id="9a01f-275">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="9a01f-275">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="9a01f-276">Assemblagens de runtime comum atualizadas</span><span class="sxs-lookup"><span data-stu-id="9a01f-276">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9a01f-277">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9a01f-277">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9a01f-278">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="9a01f-278">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="9a01f-279">Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-279">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="9a01f-280">Agora, os cmdlets Import-AzureRmApiManagementApi e \*-AzureRmApiManagementCertificate identificam caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="9a01f-280">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="9a01f-281">Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-281">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="9a01f-282">O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="9a01f-282">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="9a01f-283">Corrigido com a atualização para 4.0.4-nuget de pré-visualização</span><span class="sxs-lookup"><span data-stu-id="9a01f-283">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="9a01f-284">Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-284">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="9a01f-285">Foi corrigido o filtro de Odata para procurar por nome de produto</span><span class="sxs-lookup"><span data-stu-id="9a01f-285">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="9a01f-286">Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-286">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="9a01f-287">Foi corrigido o filtro de Odata para procurar por nome na API</span><span class="sxs-lookup"><span data-stu-id="9a01f-287">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="9a01f-288">Foi adicionado suporte para o logger de AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="9a01f-288">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-289">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-289">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-290">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="9a01f-290">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="9a01f-291">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="9a01f-291">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="9a01f-292">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="9a01f-292">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="9a01f-293">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="9a01f-293">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-294">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-295">Representação de saída de cmdlet predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="9a01f-295">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="9a01f-296">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="9a01f-296">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="9a01f-297">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="9a01f-297">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="9a01f-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-298">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-299">Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9a01f-299">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-300">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-301">Problemas corrigidos</span><span class="sxs-lookup"><span data-stu-id="9a01f-301">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a01f-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a01f-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a01f-303">Suporte adicionado para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="9a01f-303">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="9a01f-304">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="9a01f-304">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="9a01f-305">Suporte adicionado para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-305">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="9a01f-306">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="9a01f-306">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="9a01f-307">Suporte adicionado para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="9a01f-307">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="9a01f-308">Suporte adicionado para intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="9a01f-308">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="9a01f-309">Suporte adicionado para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="9a01f-309">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="9a01f-310">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-310">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9a01f-311">Geral</span><span class="sxs-lookup"><span data-stu-id="9a01f-311">General</span></span>
* <span data-ttu-id="9a01f-312">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="9a01f-312">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-313">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-314">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="9a01f-314">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-315">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-315">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-316">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="9a01f-316">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="9a01f-317">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="9a01f-317">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="9a01f-318">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="9a01f-318">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="9a01f-319">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="9a01f-319">AzureRM.IotHub</span></span>
* <span data-ttu-id="9a01f-320">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="9a01f-320">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-321">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-321">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-322">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="9a01f-322">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="9a01f-323">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="9a01f-323">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="9a01f-324">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="9a01f-324">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-325">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-325">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-326">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9a01f-326">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-327">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-327">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-328">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="9a01f-328">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a01f-329">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a01f-329">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a01f-330">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="9a01f-330">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="9a01f-331">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="9a01f-331">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="9a01f-332">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-332">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="9a01f-333">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="9a01f-333">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="9a01f-334">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="9a01f-334">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="9a01f-335">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="9a01f-335">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="9a01f-336">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="9a01f-336">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-337">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-337">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-338">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="9a01f-338">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="9a01f-339">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-339">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-340">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-340">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-341">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-341">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9a01f-342">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="9a01f-342">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="9a01f-343">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="9a01f-343">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="9a01f-344">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="9a01f-344">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="9a01f-345">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-345">Azure.Storage</span></span>
* <span data-ttu-id="9a01f-346">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="9a01f-346">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="9a01f-347">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="9a01f-347">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9a01f-348">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-348">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9a01f-349">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-349">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="9a01f-350">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-350">Azure.AnalysisServices</span></span>
* <span data-ttu-id="9a01f-351">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-351">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9a01f-352">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9a01f-352">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9a01f-353">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="9a01f-354">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="9a01f-354">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="9a01f-355">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="9a01f-356">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="9a01f-356">AzureRM.Automation</span></span>
* <span data-ttu-id="9a01f-357">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="9a01f-358">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="9a01f-358">AzureRM.Backup</span></span>
* <span data-ttu-id="9a01f-359">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="9a01f-360">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="9a01f-360">AzureRM.Batch</span></span>
* <span data-ttu-id="9a01f-361">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="9a01f-362">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="9a01f-362">AzureRM.Billing</span></span>
* <span data-ttu-id="9a01f-363">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="9a01f-364">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="9a01f-364">AzureRM.Cdn</span></span>
* <span data-ttu-id="9a01f-365">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="9a01f-366">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-366">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="9a01f-367">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-368">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-368">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-369">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-369">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9a01f-370">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-370">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="9a01f-371">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="9a01f-371">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="9a01f-372">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="9a01f-372">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="9a01f-373">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="9a01f-373">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="9a01f-374">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9a01f-374">AzureRM.Consumption</span></span>
* <span data-ttu-id="9a01f-375">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="9a01f-376">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="9a01f-376">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="9a01f-377">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="9a01f-378">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="9a01f-378">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="9a01f-379">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-379">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="9a01f-380">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="9a01f-380">AzureRM.DataFactories</span></span>
* <span data-ttu-id="9a01f-381">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-381">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9a01f-382">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9a01f-382">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9a01f-383">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-383">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="9a01f-384">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9a01f-384">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="9a01f-385">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-385">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9a01f-386">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9a01f-386">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9a01f-387">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="9a01f-387">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="9a01f-388">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="9a01f-388">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="9a01f-389">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-389">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9a01f-390">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a01f-390">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="9a01f-391">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="9a01f-391">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="9a01f-392">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="9a01f-393">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="9a01f-393">AzureRM.Dns</span></span>
* <span data-ttu-id="9a01f-394">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="9a01f-395">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9a01f-395">AzureRM.EventGrid</span></span>
* <span data-ttu-id="9a01f-396">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9a01f-397">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9a01f-397">AzureRM.EventHub</span></span>
* <span data-ttu-id="9a01f-398">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="9a01f-399">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="9a01f-399">AzureRM.HDInsight</span></span>
* <span data-ttu-id="9a01f-400">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9a01f-401">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9a01f-401">AzureRM.Insights</span></span>
* <span data-ttu-id="9a01f-402">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="9a01f-403">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="9a01f-403">AzureRM.IotHub</span></span>
* <span data-ttu-id="9a01f-404">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a01f-405">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a01f-405">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a01f-406">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="9a01f-407">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9a01f-407">AzureRM.LogicApp</span></span>
* <span data-ttu-id="9a01f-408">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="9a01f-409">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="9a01f-409">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="9a01f-410">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="9a01f-411">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="9a01f-411">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="9a01f-412">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-412">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="9a01f-413">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="9a01f-413">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="9a01f-414">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-414">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="9a01f-415">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="9a01f-415">AzureRM.Media</span></span>
* <span data-ttu-id="9a01f-416">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-416">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-417">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-417">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-418">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="9a01f-418">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="9a01f-419">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="9a01f-419">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="9a01f-420">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="9a01f-420">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="9a01f-421">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="9a01f-421">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="9a01f-422">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="9a01f-422">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="9a01f-423">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="9a01f-423">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="9a01f-424">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="9a01f-424">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="9a01f-425">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="9a01f-425">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="9a01f-426">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="9a01f-426">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="9a01f-427">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="9a01f-428">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9a01f-428">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="9a01f-429">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="9a01f-430">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9a01f-430">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="9a01f-431">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="9a01f-432">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="9a01f-432">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="9a01f-433">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="9a01f-434">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-434">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="9a01f-435">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9a01f-436">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9a01f-436">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9a01f-437">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="9a01f-437">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="9a01f-438">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="9a01f-438">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="9a01f-439">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="9a01f-439">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="9a01f-440">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-440">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9a01f-441">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="9a01f-441">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="9a01f-442">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="9a01f-442">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="9a01f-443">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="9a01f-443">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9a01f-444">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9a01f-444">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="9a01f-445">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-445">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="9a01f-446">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9a01f-446">AzureRM.RedisCache</span></span>
* <span data-ttu-id="9a01f-447">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-447">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="9a01f-448">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="9a01f-448">AzureRM.Relay</span></span>
* <span data-ttu-id="9a01f-449">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-449">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-450">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-450">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-451">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="9a01f-451">Support template deployment at subscription scope.</span></span> <span data-ttu-id="9a01f-452">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9a01f-452">Add new Cmdlets:</span></span>
    - <span data-ttu-id="9a01f-453">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-453">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="9a01f-454">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-454">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="9a01f-455">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-455">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="9a01f-456">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-456">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="9a01f-457">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-457">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="9a01f-458">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="9a01f-458">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="9a01f-459">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="9a01f-459">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="9a01f-460">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="9a01f-460">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="9a01f-461">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-461">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="9a01f-462">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-462">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="9a01f-463">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="9a01f-463">AzureRM.Scheduler</span></span>
* <span data-ttu-id="9a01f-464">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-464">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-465">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-465">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-466">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9a01f-467">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9a01f-467">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9a01f-468">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-469">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-469">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-470">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9a01f-471">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-471">AzureRM.Storage</span></span>
* <span data-ttu-id="9a01f-472">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-472">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="9a01f-473">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="9a01f-473">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="9a01f-474">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-474">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="9a01f-475">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9a01f-475">AzureRM.Tags</span></span>
* <span data-ttu-id="9a01f-476">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-476">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a01f-477">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a01f-477">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a01f-478">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-478">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="9a01f-479">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="9a01f-479">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="9a01f-480">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-480">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-481">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-481">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-482">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-482">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="9a01f-483">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-483">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9a01f-484">Geral</span><span class="sxs-lookup"><span data-stu-id="9a01f-484">General</span></span>
* <span data-ttu-id="9a01f-485">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="9a01f-485">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-486">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-486">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-487">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="9a01f-487">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="9a01f-488">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-488">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9a01f-489">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-489">Azure.Storage</span></span>
* <span data-ttu-id="9a01f-490">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="9a01f-490">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="9a01f-491">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="9a01f-491">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9a01f-492">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9a01f-492">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9a01f-493">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-493">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="9a01f-494">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="9a01f-494">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="9a01f-495">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-495">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="9a01f-496">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="9a01f-496">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="9a01f-497">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="9a01f-497">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="9a01f-498">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="9a01f-498">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-499">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-499">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-500">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="9a01f-500">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="9a01f-501">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="9a01f-501">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="9a01f-502">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="9a01f-502">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="9a01f-503">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="9a01f-503">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="9a01f-504">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="9a01f-504">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="9a01f-505">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="9a01f-505">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="9a01f-506">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="9a01f-506">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="9a01f-507">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="9a01f-507">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="9a01f-508">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="9a01f-508">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="9a01f-509">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="9a01f-509">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9a01f-510">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9a01f-510">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9a01f-511">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="9a01f-511">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="9a01f-512">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="9a01f-512">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="9a01f-513">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-513">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="9a01f-514">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="9a01f-514">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9a01f-515">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9a01f-515">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9a01f-516">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="9a01f-516">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9a01f-517">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9a01f-517">AzureRM.EventHub</span></span>
* <span data-ttu-id="9a01f-518">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="9a01f-518">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9a01f-519">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9a01f-519">AzureRM.Insights</span></span>
* <span data-ttu-id="9a01f-520">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="9a01f-520">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="9a01f-521">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="9a01f-521">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a01f-522">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a01f-522">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a01f-523">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-523">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-524">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-524">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-525">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="9a01f-525">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-526">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-526">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-527">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="9a01f-527">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="9a01f-528">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="9a01f-528">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-529">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-529">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-530">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="9a01f-530">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="9a01f-531">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="9a01f-531">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-532">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-532">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-533">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9a01f-533">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="9a01f-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="9a01f-535">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9a01f-535">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="9a01f-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="9a01f-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="9a01f-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="9a01f-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="9a01f-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="9a01f-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="9a01f-539">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="9a01f-539">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="9a01f-540">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="9a01f-540">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9a01f-541">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-541">AzureRM.Storage</span></span>
* <span data-ttu-id="9a01f-542">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="9a01f-542">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="9a01f-543">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="9a01f-543">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="9a01f-544">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9a01f-544">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="9a01f-545">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9a01f-545">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="9a01f-546">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9a01f-546">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="9a01f-547">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9a01f-547">AzureRM.Tags</span></span>
* <span data-ttu-id="9a01f-548">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="9a01f-548">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="9a01f-549">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-549">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-550">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-550">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-551">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="9a01f-551">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9a01f-552">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-552">Azure.Storage</span></span>
* <span data-ttu-id="9a01f-553">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="9a01f-553">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="9a01f-554">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="9a01f-554">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="9a01f-555">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="9a01f-555">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9a01f-556">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-556">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9a01f-557">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="9a01f-557">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="9a01f-558">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="9a01f-558">AzureRM.Automation</span></span>
* <span data-ttu-id="9a01f-559">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="9a01f-559">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-560">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-560">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-561">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="9a01f-561">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="9a01f-562">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="9a01f-562">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="9a01f-563">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="9a01f-563">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="9a01f-564">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="9a01f-564">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="9a01f-565">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="9a01f-565">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9a01f-566">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9a01f-566">AzureRM.EventHub</span></span>
* <span data-ttu-id="9a01f-567">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="9a01f-567">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a01f-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a01f-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a01f-569">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="9a01f-569">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="9a01f-570">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9a01f-570">AzureRM.LogicApp</span></span>
* <span data-ttu-id="9a01f-571">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="9a01f-571">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-572">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-572">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-573">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="9a01f-573">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="9a01f-574">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="9a01f-574">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="9a01f-575">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="9a01f-575">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="9a01f-576">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="9a01f-576">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="9a01f-577">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="9a01f-577">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="9a01f-578">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="9a01f-578">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="9a01f-579">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="9a01f-579">AzureRM.Relay</span></span>
* <span data-ttu-id="9a01f-580">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="9a01f-580">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-581">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-581">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-582">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="9a01f-582">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="9a01f-583">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="9a01f-583">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="9a01f-584">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9a01f-584">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="9a01f-585">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="9a01f-585">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="9a01f-586">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="9a01f-586">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-587">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-587">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-588">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="9a01f-588">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="9a01f-589">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="9a01f-589">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="9a01f-590">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9a01f-590">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9a01f-591">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9a01f-591">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9a01f-592">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9a01f-592">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9a01f-593">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9a01f-593">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9a01f-594">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9a01f-594">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="9a01f-595">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="9a01f-595">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9a01f-596">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9a01f-596">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9a01f-597">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="9a01f-597">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-598">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-598">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-599">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="9a01f-599">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="9a01f-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="9a01f-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-602">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-602">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-603">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="9a01f-603">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="9a01f-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="9a01f-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="9a01f-605">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="9a01f-605">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="9a01f-606">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-606">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9a01f-607">Geral</span><span class="sxs-lookup"><span data-stu-id="9a01f-607">General</span></span>
* <span data-ttu-id="9a01f-608">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="9a01f-608">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-609">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-609">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-610">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="9a01f-610">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-611">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-611">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-612">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="9a01f-612">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="9a01f-613">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="9a01f-613">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="9a01f-614">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-614">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="9a01f-615">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="9a01f-615">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="9a01f-616">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-616">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="9a01f-617">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-617">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="9a01f-618">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-618">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="9a01f-619">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9a01f-619">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="9a01f-620">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="9a01f-620">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="9a01f-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a01f-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9a01f-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a01f-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9a01f-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a01f-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9a01f-624">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9a01f-624">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9a01f-625">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="9a01f-625">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="9a01f-626">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="9a01f-626">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9a01f-627">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="9a01f-627">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="9a01f-628">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="9a01f-628">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9a01f-629">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9a01f-629">AzureRM.EventHub</span></span>
* <span data-ttu-id="9a01f-630">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="9a01f-630">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="9a01f-631">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="9a01f-631">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="9a01f-632">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="9a01f-632">Provided Default Parameter set.</span></span>
* <span data-ttu-id="9a01f-633">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9a01f-633">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a01f-634">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a01f-634">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a01f-635">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="9a01f-635">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-636">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-636">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-637">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="9a01f-637">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="9a01f-638">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="9a01f-638">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="9a01f-639">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="9a01f-639">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9a01f-640">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="9a01f-640">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9a01f-641">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9a01f-641">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9a01f-642">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9a01f-642">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9a01f-643">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9a01f-643">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9a01f-644">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="9a01f-644">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="9a01f-645">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="9a01f-645">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="9a01f-646">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="9a01f-646">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9a01f-647">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9a01f-647">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9a01f-648">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="9a01f-648">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="9a01f-649">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="9a01f-649">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="9a01f-650">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="9a01f-650">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-651">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-651">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-652">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="9a01f-652">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="9a01f-653">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a01f-653">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="9a01f-654">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a01f-654">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="9a01f-655">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="9a01f-655">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="9a01f-656">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9a01f-656">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="9a01f-657">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a01f-657">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9a01f-658">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="9a01f-658">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9a01f-659">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="9a01f-659">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="9a01f-660">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a01f-660">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9a01f-661">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="9a01f-661">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9a01f-662">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="9a01f-662">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="9a01f-663">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="9a01f-663">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="9a01f-664">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="9a01f-664">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="9a01f-665">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a01f-665">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a01f-666">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9a01f-666">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-667">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-668">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="9a01f-668">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="9a01f-669">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="9a01f-669">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="9a01f-670">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-670">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-671">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-671">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-672">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="9a01f-672">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="9a01f-673">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="9a01f-673">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9a01f-674">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a01f-674">Azure.Storage</span></span>
* <span data-ttu-id="9a01f-675">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="9a01f-675">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-676">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-676">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-677">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="9a01f-677">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="9a01f-678">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="9a01f-678">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="9a01f-679">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9a01f-679">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9a01f-680">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9a01f-680">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9a01f-681">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="9a01f-681">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="9a01f-682">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="9a01f-682">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="9a01f-683">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a01f-683">Start-AzureRmVM</span></span>
    - <span data-ttu-id="9a01f-684">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a01f-684">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="9a01f-685">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a01f-685">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="9a01f-686">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a01f-686">Set-AzureRmVM</span></span>
    - <span data-ttu-id="9a01f-687">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="9a01f-687">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="9a01f-688">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-688">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="9a01f-689">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="9a01f-689">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="9a01f-690">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="9a01f-690">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="9a01f-691">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-691">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="9a01f-692">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-692">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="9a01f-693">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-693">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="9a01f-694">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a01f-694">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="9a01f-695">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="9a01f-695">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="9a01f-696">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9a01f-696">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9a01f-697">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="9a01f-697">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="9a01f-698">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9a01f-698">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9a01f-699">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="9a01f-699">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="9a01f-700">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="9a01f-700">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="9a01f-701">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="9a01f-701">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="9a01f-702">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9a01f-702">AzureRM.EventGrid</span></span>
* <span data-ttu-id="9a01f-703">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="9a01f-703">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a01f-704">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a01f-704">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a01f-705">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="9a01f-705">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="9a01f-706">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9a01f-706">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="9a01f-707">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="9a01f-707">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="9a01f-708">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="9a01f-708">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="9a01f-709">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="9a01f-709">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9a01f-710">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9a01f-710">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9a01f-711">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="9a01f-711">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="9a01f-712">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="9a01f-712">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-713">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-713">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-714">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="9a01f-714">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a01f-715">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a01f-715">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a01f-716">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-716">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-717">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-717">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-718">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="9a01f-718">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="9a01f-719">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="9a01f-719">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="9a01f-720">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-720">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="9a01f-721">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9a01f-721">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="9a01f-722">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="9a01f-722">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="9a01f-723">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-723">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-724">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-724">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-725">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="9a01f-725">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a01f-726">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a01f-726">AzureRM.Compute</span></span>
* <span data-ttu-id="9a01f-727">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="9a01f-727">VMSS VM Update feature</span></span>
    - <span data-ttu-id="9a01f-728">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="9a01f-728">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="9a01f-729">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="9a01f-729">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9a01f-730">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9a01f-730">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9a01f-731">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="9a01f-731">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="9a01f-732">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="9a01f-732">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="9a01f-733">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="9a01f-733">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="9a01f-734">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="9a01f-734">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="9a01f-735">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="9a01f-735">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="9a01f-736">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a01f-736">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a01f-737">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="9a01f-737">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-738">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-738">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-739">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="9a01f-739">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a01f-740">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a01f-740">AzureRM.Resources</span></span>
* <span data-ttu-id="9a01f-741">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="9a01f-741">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="9a01f-742">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="9a01f-742">AzureRM.Scheduler</span></span>
* <span data-ttu-id="9a01f-743">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="9a01f-743">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="9a01f-744">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-744">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-745">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="9a01f-745">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="9a01f-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a01f-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9a01f-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9a01f-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9a01f-748">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9a01f-748">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9a01f-749">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9a01f-749">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9a01f-750">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a01f-750">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a01f-751">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a01f-751">AzureRM.Websites</span></span>
* <span data-ttu-id="9a01f-752">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="9a01f-752">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="9a01f-753">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="9a01f-753">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a01f-754">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a01f-754">AzureRM.Profile</span></span>
* <span data-ttu-id="9a01f-755">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="9a01f-755">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9a01f-756">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9a01f-756">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9a01f-757">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="9a01f-757">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9a01f-758">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9a01f-758">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9a01f-759">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="9a01f-759">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="9a01f-760">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9a01f-760">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="9a01f-761">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="9a01f-761">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="9a01f-762">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="9a01f-762">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="9a01f-763">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="9a01f-763">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="9a01f-764">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="9a01f-764">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="9a01f-765">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="9a01f-765">Added support for MSI identity</span></span>
* <span data-ttu-id="9a01f-766">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="9a01f-766">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="9a01f-767">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9a01f-767">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="9a01f-768">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-768">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="9a01f-769">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9a01f-769">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="9a01f-770">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9a01f-770">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="9a01f-771">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="9a01f-771">AzureRM.Batch</span></span>
* <span data-ttu-id="9a01f-772">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="9a01f-772">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="9a01f-773">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="9a01f-773">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="9a01f-774">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9a01f-774">AzureRM.Consumption</span></span>
* <span data-ttu-id="9a01f-775">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="9a01f-775">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9a01f-776">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9a01f-776">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9a01f-777">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="9a01f-777">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9a01f-778">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a01f-778">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="9a01f-779">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a01f-779">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="9a01f-780">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a01f-780">AzureRM.Network</span></span>
* <span data-ttu-id="9a01f-781">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="9a01f-781">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="9a01f-782">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="9a01f-782">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="9a01f-783">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a01f-783">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="9a01f-784">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9a01f-784">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="9a01f-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9a01f-786">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9a01f-786">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="9a01f-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9a01f-788">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="9a01f-788">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="9a01f-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9a01f-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9a01f-790">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9a01f-790">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9a01f-791">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="9a01f-791">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a01f-792">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a01f-792">AzureRM.Sql</span></span>
* <span data-ttu-id="9a01f-793">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="9a01f-793">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="9a01f-794">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="9a01f-794">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="9a01f-795">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="9a01f-795">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="9a01f-796">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="9a01f-796">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="9a01f-797">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="9a01f-797">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="9a01f-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a01f-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9a01f-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9a01f-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9a01f-800">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9a01f-800">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9a01f-801">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9a01f-801">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9a01f-802">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a01f-802">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a01f-803">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a01f-803">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a01f-804">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="9a01f-804">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
