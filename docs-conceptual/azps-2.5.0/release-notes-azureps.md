---
ms.openlocfilehash: 77cb28e47d8dddcf3936edff23f794de3b78442b
ms.sourcegitcommit: b02cbcd00748a4a9a4790a5fba229ce53c3bf973
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/09/2019
ms.locfileid: "68861198"
---
## <a name="250---july-2019"></a><span data-ttu-id="a0191-101">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-101">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-102">Az.Accounts</span></span>
* <span data-ttu-id="a0191-103">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a0191-103">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="a0191-104">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-104">Az.ApplicationInsights</span></span>
* <span data-ttu-id="a0191-105">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="a0191-105">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="a0191-106">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-106">Az.Automation</span></span>
* <span data-ttu-id="a0191-107">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="a0191-107">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="a0191-108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a0191-108">Az.CognitiveServices</span></span>
* <span data-ttu-id="a0191-109">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="a0191-109">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-110">Az.Compute</span></span>
* <span data-ttu-id="a0191-111">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="a0191-111">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a0191-112">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a0191-112">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a0191-113">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="a0191-113">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="a0191-114">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="a0191-114">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a0191-115">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a0191-115">Az.DataFactory</span></span>
* <span data-ttu-id="a0191-116">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a0191-116">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="a0191-117">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="a0191-117">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a0191-118">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a0191-118">Az.EventHub</span></span>
* <span data-ttu-id="a0191-119">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="a0191-119">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="a0191-120">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="a0191-120">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a0191-121">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-121">Az.KeyVault</span></span>
* <span data-ttu-id="a0191-122">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="a0191-122">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a0191-123">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a0191-123">Az.LogicApp</span></span>
* <span data-ttu-id="a0191-124">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="a0191-124">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="a0191-125">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="a0191-125">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="a0191-126">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="a0191-126">Az.ManagedServices</span></span>
* <span data-ttu-id="a0191-127">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="a0191-127">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-128">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-128">Az.Network</span></span>
* <span data-ttu-id="a0191-129">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="a0191-129">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="a0191-130">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-130">New cmdlets</span></span>
        - <span data-ttu-id="a0191-131">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a0191-131">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a0191-132">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a0191-132">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a0191-133">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-133">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a0191-134">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-134">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a0191-135">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-135">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a0191-136">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-136">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a0191-137">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="a0191-137">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="a0191-138">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a0191-138">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="a0191-139">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="a0191-139">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="a0191-140">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-140">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="a0191-141">Adicionado parâmetro opcional -PrivateEndpointNetworkPoliciesFlag para indicar a ativação ou desativação da aplicação de políticas de rede no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a0191-141">Added optional parameter -PrivateEndpointNetworkPoliciesFlag to indicate that enable or disable apply network policies on pivate endpoint in this subnet.</span></span>
        - <span data-ttu-id="a0191-142">Adicionado parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag para indicar a ativação ou desativação da aplicação de políticas de rede no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a0191-142">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag to indicate that enable or disable apply network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="a0191-143">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="a0191-143">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="a0191-144">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="a0191-144">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="a0191-145">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="a0191-145">Updated cmdlets</span></span>
        - <span data-ttu-id="a0191-146">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-146">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a0191-147">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-147">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a0191-148">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-148">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="a0191-149">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-149">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a0191-150">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-150">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="a0191-151">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a0191-151">Updated cmdlet:</span></span>
        - <span data-ttu-id="a0191-152">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-152">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="a0191-153">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-153">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="a0191-154">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-154">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="a0191-155">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="a0191-155">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="a0191-156">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="a0191-156">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="a0191-157">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="a0191-157">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a0191-158">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-158">Az.OperationalInsights</span></span>
* <span data-ttu-id="a0191-159">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="a0191-159">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="a0191-160">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="a0191-160">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-161">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-162">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-162">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="a0191-163">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-163">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="a0191-164">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-164">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="a0191-165">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-165">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="a0191-166">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-166">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="a0191-167">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-167">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="a0191-168">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-168">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="a0191-169">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-169">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="a0191-170">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-170">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="a0191-171">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="a0191-171">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-172">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-172">Az.Resources</span></span>
- <span data-ttu-id="a0191-173">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a0191-173">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="a0191-174">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a0191-174">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a0191-175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a0191-175">Az.ServiceBus</span></span>
* <span data-ttu-id="a0191-176">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="a0191-176">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="a0191-177">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="a0191-177">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-178">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-178">Az.Sql</span></span>
* <span data-ttu-id="a0191-179">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="a0191-179">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="a0191-180">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="a0191-180">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="a0191-181">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="a0191-181">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-182">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-182">Az.Storage</span></span>
* <span data-ttu-id="a0191-183">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="a0191-183">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a0191-184">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a0191-184">Az.StorageSync</span></span>
* <span data-ttu-id="a0191-185">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="a0191-185">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="a0191-186">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="a0191-186">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-187">Az.Websites</span></span>
* <span data-ttu-id="a0191-188">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a0191-188">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="a0191-189">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="a0191-189">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="a0191-190">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a0191-190">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="a0191-191">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-191">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-192">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-192">Az.Accounts</span></span>
* <span data-ttu-id="a0191-193">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="a0191-193">Add support for profile cmdlets</span></span>
* <span data-ttu-id="a0191-194">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="a0191-194">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="a0191-195">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="a0191-195">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="a0191-196">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a0191-196">Az.Advisor</span></span>
* <span data-ttu-id="a0191-197">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a0191-197">GA release of Az.Advisor</span></span>
* <span data-ttu-id="a0191-198">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="a0191-198">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a0191-199">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a0191-199">Az.ApiManagement</span></span>
* <span data-ttu-id="a0191-200">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="a0191-200">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="a0191-201">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a0191-201">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="a0191-202">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="a0191-202">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="a0191-203">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="a0191-203">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="a0191-204">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="a0191-204">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="a0191-205">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a0191-205">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="a0191-206">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="a0191-206">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-207">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-207">Az.Automation</span></span>
* <span data-ttu-id="a0191-208">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="a0191-208">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-209">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-209">Az.Compute</span></span>
* <span data-ttu-id="a0191-210">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-210">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a0191-211">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a0191-211">Az.DataFactory</span></span>
* <span data-ttu-id="a0191-212">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="a0191-212">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a0191-213">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a0191-213">Az.EventGrid</span></span>
* <span data-ttu-id="a0191-214">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="a0191-214">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a0191-215">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a0191-215">Az.IotHub</span></span>
* <span data-ttu-id="a0191-216">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="a0191-216">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-217">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-217">Az.Network</span></span>
* <span data-ttu-id="a0191-218">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="a0191-218">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="a0191-219">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="a0191-219">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a0191-220">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-220">Az.PolicyInsights</span></span>
* <span data-ttu-id="a0191-221">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="a0191-221">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="a0191-222">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="a0191-222">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a0191-223">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-223">Az.OperationalInsights</span></span>
* <span data-ttu-id="a0191-224">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="a0191-224">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-225">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-225">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-226">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="a0191-226">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-227">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-227">Az.Resources</span></span>
    - <span data-ttu-id="a0191-228">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="a0191-228">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="a0191-229">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="a0191-229">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="a0191-230">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="a0191-230">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="a0191-231">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="a0191-231">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a0191-232">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a0191-232">Az.ServiceBus</span></span>
* <span data-ttu-id="a0191-233">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="a0191-233">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-234">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-234">Az.Sql</span></span>
* <span data-ttu-id="a0191-235">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="a0191-235">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="a0191-236">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="a0191-236">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="a0191-237">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a0191-237">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a0191-238">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a0191-238">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a0191-239">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a0191-239">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a0191-240">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a0191-240">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="a0191-241">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a0191-241">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="a0191-242">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a0191-242">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="a0191-243">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="a0191-243">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-244">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-244">Az.Storage</span></span>
* <span data-ttu-id="a0191-245">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="a0191-245">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="a0191-246">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a0191-246">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="a0191-247">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="a0191-247">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="a0191-248">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="a0191-248">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="a0191-249">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-249">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="a0191-250">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-250">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="a0191-251">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-251">Set-AzStorageAccount</span></span>
* <span data-ttu-id="a0191-252">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="a0191-252">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="a0191-253">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a0191-253">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="a0191-254">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a0191-254">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a0191-255">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a0191-255">Az.StorageSync</span></span>
* <span data-ttu-id="a0191-256">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="a0191-256">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="a0191-257">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-257">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-258">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-258">Az.Accounts</span></span>
* <span data-ttu-id="a0191-259">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="a0191-259">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="a0191-260">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="a0191-260">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="a0191-261">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a0191-261">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="a0191-262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="a0191-262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="a0191-263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="a0191-263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-264">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-264">Az.Compute</span></span>
* <span data-ttu-id="a0191-265">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="a0191-265">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="a0191-266">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="a0191-266">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="a0191-267">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="a0191-267">Az.Dns</span></span>
* <span data-ttu-id="a0191-268">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="a0191-268">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a0191-269">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a0191-269">Az.EventGrid</span></span>
* <span data-ttu-id="a0191-270">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="a0191-270">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="a0191-271">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a0191-271">New cmdlets:</span></span>
    - <span data-ttu-id="a0191-272">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a0191-272">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a0191-273">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a0191-273">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a0191-274">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a0191-274">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a0191-275">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0191-275">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="a0191-276">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a0191-276">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a0191-277">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a0191-277">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a0191-278">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="a0191-278">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="a0191-279">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a0191-279">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a0191-280">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="a0191-280">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="a0191-281">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a0191-281">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="a0191-282">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="a0191-282">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="a0191-283">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a0191-283">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="a0191-284">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="a0191-284">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="a0191-285">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="a0191-285">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="a0191-286">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="a0191-286">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="a0191-287">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="a0191-287">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="a0191-288">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="a0191-288">Updated cmdlets:</span></span>
    - <span data-ttu-id="a0191-289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="a0191-289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="a0191-290">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a0191-290">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="a0191-291">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a0191-291">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="a0191-292">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="a0191-292">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="a0191-293">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a0191-293">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="a0191-294">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="a0191-294">Event subscription expiration date,</span></span>
            - <span data-ttu-id="a0191-295">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="a0191-295">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="a0191-296">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="a0191-296">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="a0191-297">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="a0191-297">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="a0191-298">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="a0191-298">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="a0191-299">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="a0191-299">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="a0191-300">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="a0191-300">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="a0191-301">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a0191-301">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="a0191-302">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a0191-302">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a0191-303">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a0191-303">Az.FrontDoor</span></span>
* <span data-ttu-id="a0191-304">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="a0191-304">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="a0191-305">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="a0191-305">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="a0191-306">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="a0191-306">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="a0191-307">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="a0191-307">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-308">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-308">Az.Network</span></span>
* <span data-ttu-id="a0191-309">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a0191-309">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="a0191-310">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-310">New cmdlets</span></span>
        - <span data-ttu-id="a0191-311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="a0191-311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="a0191-312">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="a0191-312">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="a0191-313">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-313">New cmdlets</span></span> 
        - <span data-ttu-id="a0191-314">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="a0191-314">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="a0191-315">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a0191-315">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="a0191-316">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-316">New cmdlets</span></span> 
        - <span data-ttu-id="a0191-317">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a0191-317">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="a0191-318">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a0191-318">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a0191-319">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a0191-319">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a0191-320">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-320">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="a0191-321">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-321">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="a0191-322">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a0191-322">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="a0191-323">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-323">New cmdlets</span></span>
        - <span data-ttu-id="a0191-324">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a0191-324">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a0191-325">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a0191-325">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a0191-326">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a0191-326">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a0191-327">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-327">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="a0191-328">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a0191-328">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="a0191-329">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="a0191-329">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="a0191-330">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="a0191-330">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="a0191-331">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a0191-331">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="a0191-332">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a0191-332">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="a0191-333">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="a0191-333">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="a0191-334">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-334">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="a0191-335">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="a0191-335">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="a0191-336">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-336">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="a0191-337">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="a0191-337">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="a0191-338">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-338">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="a0191-339">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-339">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="a0191-340">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="a0191-340">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="a0191-341">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a0191-341">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="a0191-342">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="a0191-342">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="a0191-343">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="a0191-343">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="a0191-344">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a0191-344">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="a0191-345">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="a0191-345">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="a0191-346">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="a0191-346">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="a0191-347">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="a0191-347">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="a0191-348">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-348">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="a0191-349">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-349">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="a0191-350">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-350">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a0191-351">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-351">Az.OperationalInsights</span></span>
* <span data-ttu-id="a0191-352">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="a0191-352">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-353">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-353">Az.Resources</span></span>
* <span data-ttu-id="a0191-354">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="a0191-354">Support for additional Template Export options</span></span>
    - <span data-ttu-id="a0191-355">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a0191-355">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="a0191-356">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a0191-356">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="a0191-357">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="a0191-357">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a0191-358">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a0191-358">Az.ServiceFabric</span></span>
* <span data-ttu-id="a0191-359">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="a0191-359">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-360">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-360">Az.Sql</span></span>
* <span data-ttu-id="a0191-361">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a0191-361">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="a0191-362">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a0191-362">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="a0191-363">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="a0191-363">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="a0191-364">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a0191-364">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a0191-365">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a0191-365">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a0191-366">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a0191-366">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a0191-367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="a0191-367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="a0191-368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="a0191-368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-369">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-369">Az.Storage</span></span>
* <span data-ttu-id="a0191-370">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a0191-370">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="a0191-371">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-371">New-AzStorageAccount</span></span>
* <span data-ttu-id="a0191-372">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="a0191-372">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="a0191-373">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-373">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-374">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-374">Az.Websites</span></span>
* <span data-ttu-id="a0191-375">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="a0191-375">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="a0191-376">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="a0191-376">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="a0191-377">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-377">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="a0191-378">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a0191-378">Az.Cdn</span></span>
* <span data-ttu-id="a0191-379">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="a0191-379">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-380">Az.Compute</span></span>
* <span data-ttu-id="a0191-381">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="a0191-381">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="a0191-382">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="a0191-382">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a0191-383">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a0191-383">Az.EventHub</span></span>
* <span data-ttu-id="a0191-384">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="a0191-384">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="a0191-385">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="a0191-385">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-386">Az.Network</span></span>
* <span data-ttu-id="a0191-387">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="a0191-387">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="a0191-388">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="a0191-388">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a0191-389">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-389">Az.PolicyInsights</span></span>
* <span data-ttu-id="a0191-390">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="a0191-390">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-391">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-392">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="a0191-392">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a0191-393">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a0191-393">Az.ServiceBus</span></span>
* <span data-ttu-id="a0191-394">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="a0191-394">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a0191-395">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a0191-395">Az.ServiceFabric</span></span>
* <span data-ttu-id="a0191-396">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="a0191-396">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="a0191-397">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0191-397">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-398">Az.Sql</span></span>
* <span data-ttu-id="a0191-399">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="a0191-399">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="a0191-400">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-400">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="a0191-401">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a0191-401">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="a0191-402">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="a0191-402">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-403">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-403">Az.Websites</span></span>
* <span data-ttu-id="a0191-404">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="a0191-404">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="a0191-405">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-405">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="a0191-406">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a0191-406">Az.ApiManagement</span></span>
* <span data-ttu-id="a0191-407">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="a0191-407">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="a0191-408">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="a0191-408">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="a0191-409">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a0191-409">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="a0191-410">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="a0191-410">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="a0191-411">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-411">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="a0191-412">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="a0191-412">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="a0191-413">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a0191-413">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="a0191-414">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a0191-414">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="a0191-415">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a0191-415">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="a0191-416">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="a0191-416">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="a0191-417">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="a0191-417">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="a0191-418">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="a0191-418">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="a0191-419">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="a0191-419">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="a0191-420">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="a0191-420">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="a0191-421">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="a0191-421">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="a0191-422">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="a0191-422">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="a0191-423">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="a0191-423">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="a0191-424">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="a0191-424">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="a0191-425">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="a0191-425">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="a0191-426">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="a0191-426">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="a0191-427">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="a0191-427">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="a0191-428">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="a0191-428">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="a0191-429">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="a0191-429">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="a0191-430">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a0191-430">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="a0191-431">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="a0191-431">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="a0191-432">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="a0191-432">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="a0191-433">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="a0191-433">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="a0191-434">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="a0191-434">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="a0191-435">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="a0191-435">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="a0191-436">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="a0191-436">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="a0191-437">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="a0191-437">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="a0191-438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="a0191-438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="a0191-439">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="a0191-439">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="a0191-440">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a0191-440">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a0191-441">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="a0191-441">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="a0191-442">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="a0191-442">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="a0191-443">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="a0191-443">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="a0191-444">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="a0191-444">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="a0191-445">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="a0191-445">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="a0191-446">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a0191-446">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="a0191-447">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="a0191-447">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="a0191-448">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a0191-448">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="a0191-449">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="a0191-449">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="a0191-450">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="a0191-450">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="a0191-451">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a0191-451">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a0191-452">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="a0191-452">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="a0191-453">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a0191-453">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="a0191-454">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="a0191-454">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="a0191-455">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="a0191-455">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="a0191-456">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="a0191-456">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="a0191-457">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="a0191-457">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="a0191-458">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="a0191-458">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="a0191-459">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="a0191-459">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="a0191-460">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="a0191-460">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="a0191-461">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="a0191-461">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="a0191-462">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="a0191-462">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="a0191-463">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a0191-463">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="a0191-464">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a0191-464">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="a0191-465">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a0191-465">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="a0191-466">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="a0191-466">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="a0191-467">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a0191-467">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="a0191-468">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a0191-468">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="a0191-469">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a0191-469">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="a0191-470">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="a0191-470">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="a0191-471">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="a0191-471">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="a0191-472">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="a0191-472">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="a0191-473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="a0191-473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="a0191-474">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="a0191-474">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="a0191-475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="a0191-475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="a0191-476">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a0191-476">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="a0191-477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="a0191-477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="a0191-478">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="a0191-478">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="a0191-479">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="a0191-479">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="a0191-480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="a0191-480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="a0191-481">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="a0191-481">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="a0191-482">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a0191-482">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="a0191-483">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="a0191-483">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-484">Az.Automation</span></span>
* <span data-ttu-id="a0191-485">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="a0191-485">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="a0191-486">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="a0191-486">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="a0191-487">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="a0191-487">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="a0191-488">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="a0191-488">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="a0191-489">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="a0191-489">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="a0191-490">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="a0191-490">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="a0191-491">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="a0191-491">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-492">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-492">Az.Compute</span></span>
* <span data-ttu-id="a0191-493">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="a0191-493">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="a0191-494">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="a0191-494">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-495">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-496">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-496">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a0191-497">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a0191-497">Az.Monitor</span></span>
* <span data-ttu-id="a0191-498">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="a0191-498">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-499">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-499">Az.Network</span></span>
* <span data-ttu-id="a0191-500">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="a0191-500">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="a0191-501">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a0191-501">Updated cmdlet:</span></span>
        - <span data-ttu-id="a0191-502">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="a0191-502">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="a0191-503">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a0191-503">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-504">Az.Resources</span></span>
* <span data-ttu-id="a0191-505">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="a0191-505">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-506">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-506">Az.Sql</span></span>
* <span data-ttu-id="a0191-507">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="a0191-507">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="a0191-508">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-508">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-509">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-509">Az.Accounts</span></span>
* <span data-ttu-id="a0191-510">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="a0191-510">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a0191-511">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a0191-511">Az.CognitiveServices</span></span>
* <span data-ttu-id="a0191-512">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="a0191-512">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="a0191-513">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="a0191-513">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-514">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-514">Az.Compute</span></span>
* <span data-ttu-id="a0191-515">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="a0191-515">Proximity placement group feature.</span></span>
    - <span data-ttu-id="a0191-516">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="a0191-516">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="a0191-517">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-517">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="a0191-518">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="a0191-518">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="a0191-519">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="a0191-519">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="a0191-520">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a0191-520">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="a0191-521">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a0191-521">Breaking changes</span></span>
    - <span data-ttu-id="a0191-522">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="a0191-522">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="a0191-523">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="a0191-523">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="a0191-524">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="a0191-524">Az.DeploymentManager</span></span>
* <span data-ttu-id="a0191-525">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-525">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="a0191-526">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="a0191-526">Az.Dns</span></span>
* <span data-ttu-id="a0191-527">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="a0191-527">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="a0191-528">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="a0191-528">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="a0191-529">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="a0191-529">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a0191-530">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a0191-530">Az.FrontDoor</span></span>
* <span data-ttu-id="a0191-531">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="a0191-531">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="a0191-532">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="a0191-532">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="a0191-533">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a0191-533">Az.HDInsight</span></span>
* <span data-ttu-id="a0191-534">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a0191-534">Removed two cmdlets:</span></span>
    - <span data-ttu-id="a0191-535">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a0191-535">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="a0191-536">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a0191-536">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="a0191-537">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a0191-537">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="a0191-538">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="a0191-538">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="a0191-539">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="a0191-539">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="a0191-540">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="a0191-540">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a0191-541">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a0191-541">Az.Monitor</span></span>
* <span data-ttu-id="a0191-542">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="a0191-542">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="a0191-543">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="a0191-543">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="a0191-544">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="a0191-544">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="a0191-545">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="a0191-545">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="a0191-546">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="a0191-546">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="a0191-547">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="a0191-547">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="a0191-548">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="a0191-548">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="a0191-549">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a0191-549">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a0191-550">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a0191-550">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a0191-551">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a0191-551">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a0191-552">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a0191-552">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a0191-553">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a0191-553">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a0191-554">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="a0191-554">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="a0191-555">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="a0191-555">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-556">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-556">Az.Network</span></span>
* <span data-ttu-id="a0191-557">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="a0191-557">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="a0191-558">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-558">New cmdlets</span></span>
        - <span data-ttu-id="a0191-559">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-559">New-AzNatGateway</span></span>
        - <span data-ttu-id="a0191-560">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-560">Get-AzNatGateway</span></span>
        - <span data-ttu-id="a0191-561">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-561">Set-AzNatGateway</span></span>
        - <span data-ttu-id="a0191-562">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-562">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="a0191-563">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="a0191-563">Updated cmdlets</span></span>
        - <span data-ttu-id="a0191-564">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="a0191-564">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="a0191-565">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="a0191-565">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="a0191-566">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-566">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="a0191-567">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-567">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="a0191-568">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a0191-568">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a0191-569">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-569">Az.PolicyInsights</span></span>
* <span data-ttu-id="a0191-570">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="a0191-570">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="a0191-571">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="a0191-571">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="a0191-572">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="a0191-572">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-573">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-573">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-574">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="a0191-574">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="a0191-575">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a0191-575">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="a0191-576">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a0191-576">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="a0191-577">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a0191-577">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="a0191-578">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="a0191-578">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="a0191-579">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="a0191-579">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="a0191-580">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a0191-580">Az.Relay</span></span>
* <span data-ttu-id="a0191-581">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="a0191-581">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a0191-582">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a0191-582">Az.ServiceBus</span></span>
* <span data-ttu-id="a0191-583">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="a0191-583">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-584">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-584">Az.Storage</span></span>
* <span data-ttu-id="a0191-585">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="a0191-585">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="a0191-586">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="a0191-586">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="a0191-587">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="a0191-587">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="a0191-588">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-588">New-AzStorageAccount</span></span>
* <span data-ttu-id="a0191-589">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="a0191-589">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="a0191-590">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-590">New-AzStorageAccount</span></span>
    - <span data-ttu-id="a0191-591">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-591">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="a0191-592">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-592">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-593">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-593">Az.Websites</span></span>
* <span data-ttu-id="a0191-594">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a0191-594">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="a0191-595">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="a0191-595">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="a0191-596">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-596">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a0191-597">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a0191-597">Highlights since the last major release</span></span>
* <span data-ttu-id="a0191-598">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a0191-598">General availability of `Az` module</span></span>
* <span data-ttu-id="a0191-599">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a0191-599">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a0191-600">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a0191-600">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a0191-601">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-601">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a0191-602">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a0191-602">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a0191-603">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-603">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a0191-604">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a0191-604">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a0191-605">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-605">Az.Accounts</span></span>
* <span data-ttu-id="a0191-606">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="a0191-606">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a0191-607">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a0191-607">Az.Batch</span></span>
* <span data-ttu-id="a0191-608">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-608">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a0191-609">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a0191-609">Az.Cdn</span></span>
* <span data-ttu-id="a0191-610">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-610">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a0191-611">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a0191-611">Az.CognitiveServices</span></span>
* <span data-ttu-id="a0191-612">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-612">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-613">Az.Compute</span></span>
* <span data-ttu-id="a0191-614">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="a0191-614">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="a0191-615">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-615">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a0191-616">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a0191-616">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a0191-617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a0191-617">Az.DataFactory</span></span>
* <span data-ttu-id="a0191-618">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="a0191-618">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-619">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-619">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-620">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-620">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a0191-621">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a0191-621">Az.EventGrid</span></span>
* <span data-ttu-id="a0191-622">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="a0191-622">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a0191-623">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a0191-623">Az.EventHub</span></span>
* <span data-ttu-id="a0191-624">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="a0191-624">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="a0191-625">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a0191-625">Az.HDInsight</span></span>
* <span data-ttu-id="a0191-626">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-626">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a0191-627">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a0191-627">Az.IotHub</span></span>
* <span data-ttu-id="a0191-628">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-628">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a0191-629">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-629">Az.KeyVault</span></span>
* <span data-ttu-id="a0191-630">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-630">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a0191-631">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a0191-631">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="a0191-632">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a0191-632">Az.MachineLearning</span></span>
* <span data-ttu-id="a0191-633">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-633">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="a0191-634">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a0191-634">Az.Media</span></span>
* <span data-ttu-id="a0191-635">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-635">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a0191-636">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a0191-636">Az.Monitor</span></span>
  * <span data-ttu-id="a0191-637">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="a0191-637">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="a0191-638">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="a0191-638">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="a0191-639">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="a0191-639">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="a0191-640">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a0191-640">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="a0191-641">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a0191-641">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="a0191-642">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a0191-642">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="a0191-643">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="a0191-643">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-644">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-644">Az.Network</span></span>
* <span data-ttu-id="a0191-645">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-645">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a0191-646">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a0191-646">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="a0191-647">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="a0191-647">Az.NotificationHubs</span></span>
* <span data-ttu-id="a0191-648">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-648">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a0191-649">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-649">Az.OperationalInsights</span></span>
* <span data-ttu-id="a0191-650">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-650">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="a0191-651">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a0191-651">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="a0191-652">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-652">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-653">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-653">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-654">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-654">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a0191-655">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-655">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="a0191-656">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="a0191-656">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="a0191-657">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="a0191-657">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a0191-658">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a0191-658">Az.RedisCache</span></span>
* <span data-ttu-id="a0191-659">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-659">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-660">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-660">Az.Resources</span></span>
* <span data-ttu-id="a0191-661">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a0191-661">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-662">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-662">Az.Sql</span></span>
* <span data-ttu-id="a0191-663">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="a0191-663">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="a0191-664">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-664">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a0191-665">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="a0191-665">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="a0191-666">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="a0191-666">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="a0191-667">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="a0191-667">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="a0191-668">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="a0191-668">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="a0191-669">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a0191-669">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-670">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-670">Az.Websites</span></span>
* <span data-ttu-id="a0191-671">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="a0191-671">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="a0191-672">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a0191-672">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a0191-673">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="a0191-673">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="a0191-674">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="a0191-674">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="a0191-675">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-675">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a0191-676">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a0191-676">Highlights since the last major release</span></span>
* <span data-ttu-id="a0191-677">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a0191-677">General availability of `Az` module</span></span>
* <span data-ttu-id="a0191-678">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a0191-678">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a0191-679">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a0191-679">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a0191-680">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-680">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a0191-681">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a0191-681">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a0191-682">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-682">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a0191-683">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a0191-683">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a0191-684">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-684">Az.Accounts</span></span>
* <span data-ttu-id="a0191-685">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="a0191-685">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a0191-686">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a0191-686">Az.AnalysisServices</span></span>
* <span data-ttu-id="a0191-687">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="a0191-687">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="a0191-688">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="a0191-688">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-689">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-689">Az.Automation</span></span>
* <span data-ttu-id="a0191-690">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="a0191-690">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="a0191-691">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="a0191-691">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="a0191-692">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="a0191-692">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-693">Az.Compute</span></span>
* <span data-ttu-id="a0191-694">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-694">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a0191-695">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="a0191-695">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="a0191-696">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-696">Az.ContainerInstance</span></span>
* <span data-ttu-id="a0191-697">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="a0191-697">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a0191-698">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a0191-698">Az.DataFactory</span></span>
* <span data-ttu-id="a0191-699">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="a0191-699">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="a0191-700">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0191-700">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-701">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-701">Az.Resources</span></span>
* <span data-ttu-id="a0191-702">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="a0191-702">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="a0191-703">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a0191-703">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="a0191-704">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="a0191-704">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="a0191-705">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a0191-705">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="a0191-706">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="a0191-706">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="a0191-707">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a0191-707">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-708">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-708">Az.Sql</span></span>
* <span data-ttu-id="a0191-709">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="a0191-709">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-710">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-710">Az.Storage</span></span>
* <span data-ttu-id="a0191-711">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-711">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="a0191-712">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a0191-712">New-AzStorageContext</span></span>
* <span data-ttu-id="a0191-713">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="a0191-713">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="a0191-714">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a0191-714">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a0191-715">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a0191-715">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a0191-716">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-716">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="a0191-717">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-717">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="a0191-718">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="a0191-718">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="a0191-719">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a0191-719">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a0191-720">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a0191-720">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a0191-721">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a0191-721">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="a0191-722">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a0191-722">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="a0191-723">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-723">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a0191-724">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a0191-724">Highlights since the last major release</span></span>
* <span data-ttu-id="a0191-725">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a0191-725">General availability of `Az` module</span></span>
* <span data-ttu-id="a0191-726">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a0191-726">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a0191-727">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a0191-727">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a0191-728">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-728">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a0191-729">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a0191-729">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a0191-730">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-730">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a0191-731">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a0191-731">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-732">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-732">Az.Automation</span></span>
* <span data-ttu-id="a0191-733">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="a0191-733">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="a0191-734">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="a0191-734">Dynamic grouping</span></span>
    * <span data-ttu-id="a0191-735">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="a0191-735">Pre-Post script</span></span>
    * <span data-ttu-id="a0191-736">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="a0191-736">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-737">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-737">Az.Compute</span></span>
* <span data-ttu-id="a0191-738">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="a0191-738">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="a0191-739">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="a0191-739">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a0191-740">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-740">Az.KeyVault</span></span>
* <span data-ttu-id="a0191-741">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-741">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-742">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-742">Az.Network</span></span>
* <span data-ttu-id="a0191-743">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a0191-743">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="a0191-744">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a0191-744">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-745">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-745">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-746">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="a0191-746">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="a0191-747">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="a0191-747">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-748">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-748">Az.Resources</span></span>
* <span data-ttu-id="a0191-749">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a0191-749">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="a0191-750">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="a0191-750">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-751">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-751">Az.Sql</span></span>
* <span data-ttu-id="a0191-752">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="a0191-752">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-753">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-753">Az.Storage</span></span>
* <span data-ttu-id="a0191-754">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a0191-754">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="a0191-755">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-755">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a0191-756">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-756">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a0191-757">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-757">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a0191-758">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="a0191-758">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="a0191-759">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="a0191-759">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="a0191-760">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a0191-760">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-761">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-761">Az.Websites</span></span>
* <span data-ttu-id="a0191-762">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="a0191-762">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="a0191-763">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-763">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-764">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-764">Az.Accounts</span></span>
* <span data-ttu-id="a0191-765">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="a0191-765">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="a0191-766">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-766">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-767">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-767">Az.Automation</span></span>
* <span data-ttu-id="a0191-768">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-768">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="a0191-769">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="a0191-769">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="a0191-770">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="a0191-770">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a0191-771">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a0191-771">Az.Cdn</span></span>
* <span data-ttu-id="a0191-772">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="a0191-772">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-773">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-773">Az.Compute</span></span>
* <span data-ttu-id="a0191-774">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="a0191-774">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a0191-775">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a0191-775">Az.DataFactory</span></span>
* <span data-ttu-id="a0191-776">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="a0191-776">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a0191-777">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a0191-777">Az.LogicApp</span></span>
* <span data-ttu-id="a0191-778">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="a0191-778">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-779">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-779">Az.Network</span></span>
* <span data-ttu-id="a0191-780">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="a0191-780">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-781">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-781">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-782">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-782">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="a0191-783">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="a0191-783">SDK Update</span></span>
* <span data-ttu-id="a0191-784">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a0191-784">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="a0191-785">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a0191-785">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-786">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-786">Az.Resources</span></span>
* <span data-ttu-id="a0191-787">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="a0191-787">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="a0191-788">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="a0191-788">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="a0191-789">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="a0191-789">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="a0191-790">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="a0191-790">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="a0191-791">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="a0191-791">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="a0191-792">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="a0191-792">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-793">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-793">Az.Sql</span></span>
* <span data-ttu-id="a0191-794">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a0191-794">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="a0191-795">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a0191-795">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-796">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-796">Az.Storage</span></span>
* <span data-ttu-id="a0191-797">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-797">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="a0191-798">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-798">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="a0191-799">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a0191-799">Az.AnalysisServices</span></span>
* <span data-ttu-id="a0191-800">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="a0191-800">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-801">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-801">Az.Automation</span></span>
* <span data-ttu-id="a0191-802">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-802">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="a0191-803">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-803">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="a0191-804">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-804">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a0191-805">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a0191-805">Az.CognitiveServices</span></span>
* <span data-ttu-id="a0191-806">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a0191-806">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-807">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-807">Az.Compute</span></span>
* <span data-ttu-id="a0191-808">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="a0191-808">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="a0191-809">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="a0191-809">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="a0191-810">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a0191-810">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="a0191-811">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="a0191-811">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-812">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-812">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-813">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="a0191-813">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a0191-814">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a0191-814">Az.EventHub</span></span>
* <span data-ttu-id="a0191-815">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="a0191-815">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="a0191-816">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-816">Az.KeyVault</span></span>
* <span data-ttu-id="a0191-817">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a0191-817">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a0191-818">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a0191-818">Az.LogicApp</span></span>
* <span data-ttu-id="a0191-819">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a0191-819">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="a0191-820">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="a0191-820">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="a0191-821">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a0191-821">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="a0191-822">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a0191-822">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a0191-823">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a0191-823">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a0191-824">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a0191-824">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a0191-825">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a0191-825">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="a0191-826">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a0191-826">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="a0191-827">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-827">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a0191-828">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-828">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a0191-829">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-829">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a0191-830">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-830">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="a0191-831">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a0191-831">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a0191-832">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a0191-832">Az.Monitor</span></span>
* <span data-ttu-id="a0191-833">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="a0191-833">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-834">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-834">Az.Network</span></span>
* <span data-ttu-id="a0191-835">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="a0191-835">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a0191-836">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-836">Az.OperationalInsights</span></span>
* <span data-ttu-id="a0191-837">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="a0191-837">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="a0191-838">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a0191-838">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="a0191-839">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="a0191-839">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="a0191-840">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-840">Az.Resources</span></span>
* <span data-ttu-id="a0191-841">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a0191-841">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a0191-842">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a0191-842">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="a0191-843">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="a0191-843">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="a0191-844">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="a0191-844">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-845">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-845">Az.Sql</span></span>
* <span data-ttu-id="a0191-846">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="a0191-846">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="a0191-847">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="a0191-847">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-848">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-848">Az.Websites</span></span>
* <span data-ttu-id="a0191-849">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="a0191-849">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="a0191-850">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-850">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-851">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-851">Az.Accounts</span></span>
* <span data-ttu-id="a0191-852">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a0191-852">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a0191-853">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a0191-853">Az.AnalysisServices</span></span>
<span data-ttu-id="a0191-854">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="a0191-854">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-855">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-855">Az.Compute</span></span>
* <span data-ttu-id="a0191-856">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="a0191-856">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="a0191-857">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="a0191-857">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="a0191-858">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a0191-858">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-859">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-859">Az.RecoveryServices</span></span>
<span data-ttu-id="a0191-860">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="a0191-860">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-861">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-861">Az.Resources</span></span>
* <span data-ttu-id="a0191-862">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="a0191-862">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="a0191-863">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a0191-863">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a0191-864">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="a0191-864">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="a0191-865">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a0191-865">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-866">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-866">Az.Sql</span></span>
* <span data-ttu-id="a0191-867">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a0191-867">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="a0191-868">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="a0191-868">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="a0191-869">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="a0191-869">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="a0191-870">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-870">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-871">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-871">Az.Accounts</span></span>
* <span data-ttu-id="a0191-872">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="a0191-872">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a0191-873">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a0191-873">Az.AnalysisServices</span></span>
* <span data-ttu-id="a0191-874">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a0191-874">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-875">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-875">Az.RecoveryServices</span></span>
* <span data-ttu-id="a0191-876">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a0191-876">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="a0191-877">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-877">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-878">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-878">Az.Accounts</span></span>
* <span data-ttu-id="a0191-879">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a0191-879">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a0191-880">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-880">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a0191-881">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="a0191-881">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="a0191-882">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a0191-882">Az.Aks</span></span>
* <span data-ttu-id="a0191-883">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-883">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a0191-884">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-884">Az.Automation</span></span>
* <span data-ttu-id="a0191-885">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="a0191-885">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="a0191-886">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-886">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a0191-887">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a0191-887">Az.Cdn</span></span>
* <span data-ttu-id="a0191-888">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-888">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-889">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-889">Az.Compute</span></span>
* <span data-ttu-id="a0191-890">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="a0191-890">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="a0191-891">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a0191-891">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="a0191-892">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a0191-892">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a0191-893">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a0191-893">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a0191-894">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-894">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a0191-895">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a0191-895">Az.DataFactory</span></span>
* <span data-ttu-id="a0191-896">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="a0191-896">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-897">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-897">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-898">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="a0191-898">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="a0191-899">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="a0191-899">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="a0191-900">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-900">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a0191-901">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a0191-901">Az.IotHub</span></span>
* <span data-ttu-id="a0191-902">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="a0191-902">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a0191-903">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-903">Az.KeyVault</span></span>
* <span data-ttu-id="a0191-904">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-904">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-905">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-905">Az.Network</span></span>
* <span data-ttu-id="a0191-906">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-906">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-907">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-907">Az.Resources</span></span>
* <span data-ttu-id="a0191-908">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="a0191-908">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="a0191-909">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="a0191-909">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="a0191-910">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="a0191-910">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="a0191-911">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="a0191-911">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="a0191-912">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="a0191-912">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="a0191-913">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a0191-913">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="a0191-914">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="a0191-914">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a0191-915">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a0191-915">Az.ServiceFabric</span></span>
* <span data-ttu-id="a0191-916">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="a0191-916">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="a0191-917">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="a0191-917">Fix some error messages.</span></span>
* <span data-ttu-id="a0191-918">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="a0191-918">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="a0191-919">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="a0191-919">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a0191-920">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a0191-920">Az.SignalR</span></span>
* <span data-ttu-id="a0191-921">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-921">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-922">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-922">Az.Sql</span></span>
* <span data-ttu-id="a0191-923">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-923">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a0191-924">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="a0191-924">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="a0191-925">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="a0191-925">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="a0191-926">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="a0191-926">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-927">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-927">Az.Storage</span></span>
* <span data-ttu-id="a0191-928">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-928">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a0191-929">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="a0191-929">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="a0191-930">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="a0191-930">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="a0191-931">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="a0191-931">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="a0191-932">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a0191-932">Az.TrafficManager</span></span>
* <span data-ttu-id="a0191-933">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-933">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-934">Az.Websites</span></span>
* <span data-ttu-id="a0191-935">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a0191-935">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a0191-936">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="a0191-936">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="a0191-937">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="a0191-937">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="a0191-938">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a0191-938">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a0191-939">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-939">Az.Accounts</span></span>
* <span data-ttu-id="a0191-940">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="a0191-940">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-941">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-941">Az.Compute</span></span>
* <span data-ttu-id="a0191-942">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="a0191-942">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="a0191-943">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a0191-943">Updated the description of ID in help files</span></span>
* <span data-ttu-id="a0191-944">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-944">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-945">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-945">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-946">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="a0191-946">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="a0191-947">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="a0191-947">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a0191-948">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a0191-948">Az.EventGrid</span></span>
* <span data-ttu-id="a0191-949">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="a0191-949">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="a0191-950">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a0191-950">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="a0191-951">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a0191-951">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a0191-952">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a0191-952">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a0191-953">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a0191-953">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a0191-954">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a0191-954">Dead letter endpoint.</span></span>
    - <span data-ttu-id="a0191-955">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a0191-955">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a0191-956">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a0191-956">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a0191-957">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a0191-957">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a0191-958">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a0191-958">Dead letter endpoint.</span></span>
* <span data-ttu-id="a0191-959">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="a0191-959">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="a0191-960">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a0191-960">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a0191-961">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a0191-961">Az.IotHub</span></span>
* <span data-ttu-id="a0191-962">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="a0191-962">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a0191-963">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a0191-963">Az.LogicApp</span></span>
* <span data-ttu-id="a0191-964">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="a0191-964">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-965">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-965">Az.Resources</span></span>
* <span data-ttu-id="a0191-966">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a0191-966">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="a0191-967">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="a0191-967">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="a0191-968">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a0191-968">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a0191-969">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="a0191-969">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="a0191-970">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="a0191-970">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="a0191-971">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="a0191-971">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a0191-972">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a0191-972">Az.SignalR</span></span>
* <span data-ttu-id="a0191-973">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-973">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-974">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-974">Az.Sql</span></span>
* <span data-ttu-id="a0191-975">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="a0191-975">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a0191-976">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-976">Az.Storage</span></span>
* <span data-ttu-id="a0191-977">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="a0191-977">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="a0191-978">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a0191-978">New-AzStorageContext</span></span>
* <span data-ttu-id="a0191-979">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="a0191-979">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="a0191-980">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a0191-980">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-981">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-981">Az.Websites</span></span>
* <span data-ttu-id="a0191-982">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="a0191-982">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="a0191-983">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-983">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="a0191-984">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-984">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="a0191-985">Geral</span><span class="sxs-lookup"><span data-stu-id="a0191-985">General</span></span>

- <span data-ttu-id="a0191-986">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="a0191-986">General Availability of Az Module</span></span>
- <span data-ttu-id="a0191-987">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="a0191-987">Online help for each module</span></span>
- <span data-ttu-id="a0191-988">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="a0191-988">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="a0191-989">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="a0191-989">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="a0191-990">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-990">Az.Accounts</span></span>
- <span data-ttu-id="a0191-991">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a0191-991">Changed from Az.Profile</span></span>
- <span data-ttu-id="a0191-992">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="a0191-992">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a0191-993">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a0191-993">Az.ApiManagement</span></span>
- <span data-ttu-id="a0191-994">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="a0191-994">Fixes for #7002</span></span>
- <span data-ttu-id="a0191-995">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-995">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="a0191-996">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a0191-996">Az.Batch</span></span>
- <span data-ttu-id="a0191-997">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="a0191-997">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="a0191-998">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="a0191-998">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="a0191-999">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-999">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="a0191-1000">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a0191-1000">Az.Billing</span></span>
- <span data-ttu-id="a0191-1001">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1001">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="a0191-1002">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="a0191-1002">Az.CognitivServices</span></span>
- <span data-ttu-id="a0191-1003">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-1003">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="a0191-1004">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="a0191-1004">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a0191-1005">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-1005">Az.ContainerInstance</span></span>
- <span data-ttu-id="a0191-1006">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="a0191-1006">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="a0191-1007">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a0191-1007">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="a0191-1008">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1008">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a0191-1009">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-1009">Az.DataLakeStore</span></span>
- <span data-ttu-id="a0191-1010">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1010">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="a0191-1011">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a0191-1011">Az.Monitor</span></span>
- <span data-ttu-id="a0191-1012">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1012">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="a0191-1013">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0191-1013">Az.KeyVault</span></span>
- <span data-ttu-id="a0191-1014">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="a0191-1014">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="a0191-1015">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a0191-1015">Az.MachineLearning</span></span>
- <span data-ttu-id="a0191-1016">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="a0191-1016">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="a0191-1017">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a0191-1017">Az.Media</span></span>
- <span data-ttu-id="a0191-1018">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="a0191-1018">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a0191-1019">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-1019">Az.Network</span></span>
<span data-ttu-id="a0191-1020">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a0191-1020">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="a0191-1021">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a0191-1021">New cmdlets added:</span></span>
        - <span data-ttu-id="a0191-1022">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1022">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a0191-1023">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1023">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a0191-1024">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1024">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a0191-1025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a0191-1026">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1026">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a0191-1027">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="a0191-1027">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="a0191-1028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="a0191-1029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0191-1029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="a0191-1030">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a0191-1030">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="a0191-1031">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a0191-1031">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="a0191-1032">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a0191-1032">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a0191-1033">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a0191-1033">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a0191-1034">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-1034">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="a0191-1035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-1035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="a0191-1036">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="a0191-1036">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="a0191-1037">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a0191-1037">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="a0191-1038">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a0191-1038">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a0191-1039">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a0191-1039">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a0191-1040">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a0191-1040">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="a0191-1041">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="a0191-1041">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="a0191-1042">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1042">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="a0191-1043">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-1043">Az.OperationalInsights</span></span>
- <span data-ttu-id="a0191-1044">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1044">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="a0191-1045">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a0191-1045">Az.Profile</span></span>
- <span data-ttu-id="a0191-1046">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a0191-1046">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-1047">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-1047">Az.RecoveryServices</span></span>
- <span data-ttu-id="a0191-1048">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1048">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="a0191-1049">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-1049">Az.Resources</span></span>
- <span data-ttu-id="a0191-1050">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1050">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a0191-1051">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a0191-1051">Az.ServiceFabric</span></span>
- <span data-ttu-id="a0191-1052">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="a0191-1052">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="a0191-1053">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1053">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="a0191-1054">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="a0191-1054">Az.SIgnalR</span></span>
- <span data-ttu-id="a0191-1055">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="a0191-1055">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="a0191-1056">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-1056">Az.Sql</span></span>
- <span data-ttu-id="a0191-1057">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="a0191-1057">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="a0191-1058">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="a0191-1058">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="a0191-1059">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1059">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="a0191-1060">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-1060">Az.Storage</span></span>
- <span data-ttu-id="a0191-1061">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1061">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a0191-1062">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-1062">Az.Websites</span></span>
- <span data-ttu-id="a0191-1063">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a0191-1063">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="a0191-1064">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-1064">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="a0191-1065">Geral</span><span class="sxs-lookup"><span data-stu-id="a0191-1065">General</span></span>

* <span data-ttu-id="a0191-1066">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a0191-1066">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="a0191-1067">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-1067">Az.Compute</span></span>

* <span data-ttu-id="a0191-1068">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="a0191-1068">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a0191-1069">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-1069">Az.DataLakeStore</span></span>

* <span data-ttu-id="a0191-1070">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="a0191-1070">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="a0191-1071">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a0191-1071">Az.FrontDoor</span></span>

* <span data-ttu-id="a0191-1072">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="a0191-1072">Fixed some broken links</span></span>
    - <span data-ttu-id="a0191-1073">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="a0191-1073">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="a0191-1074">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="a0191-1074">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a0191-1075">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a0191-1075">Az.RecoveryServices</span></span>

* <span data-ttu-id="a0191-1076">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0191-1076">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="a0191-1077">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="a0191-1077">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="a0191-1078">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-1078">Az.Resources</span></span>

* <span data-ttu-id="a0191-1079">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="a0191-1079">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="a0191-1080">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="a0191-1080">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="a0191-1081">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-1081">Az.Sql</span></span>

* <span data-ttu-id="a0191-1082">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a0191-1082">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="a0191-1083">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="a0191-1083">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="a0191-1084">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="a0191-1084">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="a0191-1085">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-1085">Az.Storage</span></span>

* <span data-ttu-id="a0191-1086">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a0191-1086">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="a0191-1087">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="a0191-1087">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="a0191-1088">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a0191-1088">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a0191-1089">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="a0191-1089">Support Static Website configuration</span></span>
    - <span data-ttu-id="a0191-1090">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a0191-1090">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="a0191-1091">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a0191-1091">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a0191-1092">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-1092">Az.Websites</span></span>

* <span data-ttu-id="a0191-1093">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a0191-1093">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="a0191-1094">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="a0191-1094">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="a0191-1095">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0191-1095">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="a0191-1096">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-1096">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a0191-1097">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a0191-1097">Az.ApiManagement</span></span>
* <span data-ttu-id="a0191-1098">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a0191-1098">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="a0191-1099">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a0191-1099">Az.Automation</span></span>
* <span data-ttu-id="a0191-1100">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="a0191-1100">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="a0191-1101">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="a0191-1101">Added Update Management cmdlets</span></span>
* <span data-ttu-id="a0191-1102">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="a0191-1102">Added Source Control cmdlets</span></span>
* <span data-ttu-id="a0191-1103">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="a0191-1103">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="a0191-1104">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="a0191-1104">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="a0191-1105">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-1105">Az.Compute</span></span>
* <span data-ttu-id="a0191-1106">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="a0191-1106">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="a0191-1107">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a0191-1107">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a0191-1108">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-1108">Az.ContainerInstance</span></span>
* <span data-ttu-id="a0191-1109">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a0191-1109">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="a0191-1110">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a0191-1110">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a0191-1111">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="a0191-1111">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a0191-1112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-1112">Az.Network</span></span>
* <span data-ttu-id="a0191-1113">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="a0191-1113">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="a0191-1114">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="a0191-1114">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="a0191-1115">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="a0191-1115">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="a0191-1116">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="a0191-1116">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="a0191-1117">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a0191-1117">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a0191-1118">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="a0191-1118">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="a0191-1119">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0191-1119">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="a0191-1120">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a0191-1120">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a0191-1121">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a0191-1121">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="a0191-1122">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a0191-1122">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="a0191-1123">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a0191-1123">Az.Relay</span></span>
* <span data-ttu-id="a0191-1124">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="a0191-1124">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="a0191-1125">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-1125">Az.Resources</span></span>
* <span data-ttu-id="a0191-1126">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="a0191-1126">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="a0191-1127">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="a0191-1127">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="a0191-1128">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="a0191-1128">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a0191-1129">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a0191-1129">Az.ServiceFabric</span></span>
* <span data-ttu-id="a0191-1130">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a0191-1130">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="a0191-1131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-1131">Az.Sql</span></span>
* <span data-ttu-id="a0191-1132">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-1132">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="a0191-1133">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-1133">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a0191-1134">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-1134">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a0191-1135">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-1135">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a0191-1136">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a0191-1136">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a0191-1137">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a0191-1137">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a0191-1138">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a0191-1138">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a0191-1139">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a0191-1139">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a0191-1140">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a0191-1140">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="a0191-1141">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="a0191-1141">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="a0191-1142">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a0191-1142">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="a0191-1143">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="a0191-1143">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="a0191-1144">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a0191-1144">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a0191-1145">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a0191-1145">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a0191-1146">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a0191-1146">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="a0191-1147">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a0191-1147">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="a0191-1148">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="a0191-1148">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="a0191-1149">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-1149">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a0191-1150">Geral</span><span class="sxs-lookup"><span data-stu-id="a0191-1150">General</span></span>
* <span data-ttu-id="a0191-1151">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="a0191-1151">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="a0191-1152">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a0191-1152">Az.Profile</span></span>
* <span data-ttu-id="a0191-1153">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a0191-1153">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="a0191-1154">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="a0191-1154">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="a0191-1155">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="a0191-1155">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="a0191-1156">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="a0191-1156">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="a0191-1157">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="a0191-1157">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="a0191-1158">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="a0191-1158">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="a0191-1159">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="a0191-1159">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="a0191-1160">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a0191-1160">Az.CognitiveServices</span></span>
* <span data-ttu-id="a0191-1161">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="a0191-1161">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-1162">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-1162">Az.Compute</span></span>
* <span data-ttu-id="a0191-1163">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="a0191-1163">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="a0191-1164">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="a0191-1164">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="a0191-1165">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="a0191-1165">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-1166">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-1166">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-1167">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="a0191-1167">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="a0191-1168">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="a0191-1168">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="a0191-1169">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="a0191-1169">Az.Insights</span></span>
* <span data-ttu-id="a0191-1170">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="a0191-1170">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="a0191-1171">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="a0191-1171">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="a0191-1172">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="a0191-1172">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="a0191-1173">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="a0191-1173">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-1174">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-1174">Az.Network</span></span>
* <span data-ttu-id="a0191-1175">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="a0191-1175">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="a0191-1176">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="a0191-1176">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="a0191-1177">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="a0191-1177">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="a0191-1178">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a0191-1178">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="a0191-1179">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="a0191-1179">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="a0191-1180">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="a0191-1180">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="a0191-1181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a0191-1181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a0191-1182">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a0191-1182">Az.PolicyInsights</span></span>
* <span data-ttu-id="a0191-1183">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="a0191-1183">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-1184">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-1184">Az.Resources</span></span>
* <span data-ttu-id="a0191-1185">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="a0191-1185">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="a0191-1186">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a0191-1186">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a0191-1187">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a0191-1187">Az.ServiceBus</span></span>
* <span data-ttu-id="a0191-1188">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="a0191-1188">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a0191-1189">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a0191-1189">Az.ServiceFabric</span></span>
* <span data-ttu-id="a0191-1190">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="a0191-1190">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="a0191-1191">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="a0191-1191">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="a0191-1192">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="a0191-1192">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="a0191-1193">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="a0191-1193">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="a0191-1194">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="a0191-1194">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="a0191-1195">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-1195">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="a0191-1196">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a0191-1196">Az.Profile</span></span>
* <span data-ttu-id="a0191-1197">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="a0191-1197">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="a0191-1198">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a0191-1198">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-1199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-1199">Az.Compute</span></span>
* <span data-ttu-id="a0191-1200">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="a0191-1200">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="a0191-1201">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a0191-1201">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a0191-1202">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a0191-1202">Az.DataLakeStore</span></span>
* <span data-ttu-id="a0191-1203">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a0191-1203">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="a0191-1204">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0191-1204">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="a0191-1205">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a0191-1205">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a0191-1206">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="a0191-1206">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a0191-1207">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0191-1207">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-1208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-1208">Az.Network</span></span>
* <span data-ttu-id="a0191-1209">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="a0191-1209">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="a0191-1210">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a0191-1210">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-1211">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-1211">Az.Resources</span></span>
* <span data-ttu-id="a0191-1212">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="a0191-1212">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="a0191-1213">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="a0191-1213">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="a0191-1214">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-1214">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="a0191-1215">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a0191-1215">Azure.Storage</span></span>
* <span data-ttu-id="a0191-1216">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="a0191-1216">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="a0191-1217">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a0191-1217">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="a0191-1218">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a0191-1218">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a0191-1219">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="a0191-1219">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="a0191-1220">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="a0191-1220">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="a0191-1221">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a0191-1221">Az.CognitiveServices</span></span>
* <span data-ttu-id="a0191-1222">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="a0191-1222">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a0191-1223">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a0191-1223">Az.Compute</span></span>
* <span data-ttu-id="a0191-1224">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="a0191-1224">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="a0191-1225">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="a0191-1225">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="a0191-1226">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="a0191-1226">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="a0191-1227">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a0191-1227">Az.DataFactoryV2</span></span>
* <span data-ttu-id="a0191-1228">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="a0191-1228">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a0191-1229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a0191-1229">Az.Network</span></span>
* <span data-ttu-id="a0191-1230">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="a0191-1230">Added NetworkProfile functionality.</span></span> <span data-ttu-id="a0191-1231">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="a0191-1231">new cmdlets added</span></span>
    - <span data-ttu-id="a0191-1232">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a0191-1232">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="a0191-1233">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a0191-1233">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="a0191-1234">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a0191-1234">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="a0191-1235">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a0191-1235">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="a0191-1236">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-1236">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="a0191-1237">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-1237">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="a0191-1238">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="a0191-1238">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="a0191-1239">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="a0191-1239">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="a0191-1240">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="a0191-1240">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a0191-1241">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a0191-1241">Az.RedisCache</span></span>
* <span data-ttu-id="a0191-1242">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="a0191-1242">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="a0191-1243">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="a0191-1243">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="a0191-1244">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a0191-1244">Az.Resources</span></span>
* <span data-ttu-id="a0191-1245">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a0191-1245">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a0191-1246">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="a0191-1246">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="a0191-1247">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a0191-1247">Az.Sql</span></span>
* <span data-ttu-id="a0191-1248">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="a0191-1248">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a0191-1249">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a0191-1249">Az.Websites</span></span>
* <span data-ttu-id="a0191-1250">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="a0191-1250">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="a0191-1251">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="a0191-1251">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="a0191-1252">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a0191-1252">0.2.0 - September 2018</span></span>
 <span data-ttu-id="a0191-1253">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a0191-1253">Initial Release</span></span>