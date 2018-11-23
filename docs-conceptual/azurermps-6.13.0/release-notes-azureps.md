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
ms.openlocfilehash: 7f517f0b3768a2075557b131158ee1264ea9ab3f
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/22/2018
ms.locfileid: "52260006"
---
# <a name="release-notes"></a><span data-ttu-id="5598c-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="5598c-103">Release notes</span></span>

<span data-ttu-id="5598c-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="5598c-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6130---november-2018"></a><span data-ttu-id="5598c-105">6.13.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-105">6.13.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-106">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-107">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="5598c-107">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5598c-108">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5598c-108">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5598c-109">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="5598c-109">Update dependencies for type mapping issue</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="5598c-110">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5598c-110">AzureRM.Automation</span></span>
* <span data-ttu-id="5598c-111">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="5598c-111">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="5598c-112">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="5598c-112">Added Update Management cmdlets</span></span>
* <span data-ttu-id="5598c-113">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="5598c-113">Added Source Control cmdlets</span></span>
* <span data-ttu-id="5598c-114">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="5598c-114">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="5598c-115">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="5598c-115">Fixed the DSC Register Node command</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-116">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-117">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="5598c-117">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="5598c-118">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="5598c-118">Update dependencies for type mapping issue</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="5598c-119">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5598c-119">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="5598c-120">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="5598c-120">Update dependencies for type mapping issue</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="5598c-121">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="5598c-121">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="5598c-122">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="5598c-122">update the examples description for marketplace cmdlets</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-123">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-123">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-124">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="5598c-124">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="5598c-125">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="5598c-125">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="5598c-126">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="5598c-126">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="5598c-127">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="5598c-127">Fix issues with memory usage in VirtualNetwork map</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5598c-128">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-128">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5598c-129">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="5598c-129">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="5598c-130">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="5598c-130">Converted policy timezone to uppercase.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="5598c-131">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5598c-131">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="5598c-132">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="5598c-132">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="5598c-133">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="5598c-133">Update dependencies for type mapping issue</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="5598c-134">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="5598c-134">AzureRM.Relay</span></span>
* <span data-ttu-id="5598c-135">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="5598c-135">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-136">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-136">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-137">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="5598c-137">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="5598c-138">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="5598c-138">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="5598c-139">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="5598c-139">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5598c-140">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5598c-140">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5598c-141">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="5598c-141">Add deprecation messages for upcoming breaking changes</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-142">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-142">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-143">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="5598c-143">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="5598c-144">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5598c-144">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5598c-145">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5598c-145">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5598c-146">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5598c-146">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5598c-147">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5598c-147">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5598c-148">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-148">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="5598c-149">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-149">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="5598c-150">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-150">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="5598c-151">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-151">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="5598c-152">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="5598c-152">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="5598c-153">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="5598c-153">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="5598c-154">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="5598c-154">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="5598c-155">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="5598c-155">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="5598c-156">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="5598c-156">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="5598c-157">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="5598c-157">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="5598c-158">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="5598c-158">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="5598c-159">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="5598c-159">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="6120---november-2018"></a><span data-ttu-id="5598c-160">6.12.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-160">6.12.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-161">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-161">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-162">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="5598c-162">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="5598c-163">Mudar o nome do parâmetro TenantId no cmdlet Connect-AzureRmAccount para Tenant e adicionar um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="5598c-163">Rename param TenantId in cmdlet Connect-AzureRmAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="5598c-164">Descrição de TenantId atualizada para Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="5598c-164">Updated TenantId description for Connect-AzureRmAccount</span></span>
* <span data-ttu-id="5598c-165">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="5598c-165">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="5598c-166">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="5598c-166">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="5598c-167">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="5598c-167">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="5598c-168">Corrigido o problema em que "Disconnect-AzureRmAccount" é lançado se não estiver ligado</span><span class="sxs-lookup"><span data-stu-id="5598c-168">Fix issue where 'Disconnect-AzureRmAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a><span data-ttu-id="5598c-169">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5598c-169">AzureRM.Automation</span></span>
* <span data-ttu-id="5598c-170">Foi mudado o nome do ficheiro DLL de cmdlett para Microsoft.Azure.Commands.Automation.dll</span><span class="sxs-lookup"><span data-stu-id="5598c-170">Renamed cmdlet DLL filename to Microsoft.Azure.Commands.Automation.dll</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="5598c-171">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5598c-171">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="5598c-172">Adicionar a operação Get-AzureRmCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="5598c-172">Add Get-AzureRmCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-173">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-173">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-174">Adicionar os cmdlets Add-AzureRmVmssVMDataDisk e Remove-AzureRmVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="5598c-174">Add Add-AzureRmVmssVMDataDisk and Remove-AzureRmVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="5598c-175">Get-AzureRmVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="5598c-175">Get-AzureRmVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="5598c-176">Corrigidos os valores de opção SetAzureRmVMChefExtension -BootstrapOptions e -JsonAttribute no formato json.</span><span class="sxs-lookup"><span data-stu-id="5598c-176">Fixed SetAzureRmVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5598c-177">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5598c-177">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5598c-178">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="5598c-178">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="5598c-179">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="5598c-179">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5598c-180">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5598c-180">AzureRM.Insights</span></span>
* <span data-ttu-id="5598c-181">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="5598c-181">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="5598c-182">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="5598c-182">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="5598c-183">Corrigido o problema n.º 7513 [Insights] Set-AzureRMDiagnosticSetting requer especificação explícita das categorias durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="5598c-183">Fixed issue #7513 [Insights] Set-AzureRMDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="5598c-184">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="5598c-184">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-185">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-185">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-186">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="5598c-186">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="5598c-187">Get-AzureRmExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="5598c-187">Get-AzureRmExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="5598c-188">Get-AzureRmExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="5598c-188">Get-AzureRmExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="5598c-189">Get-AzureRmExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="5598c-189">Get-AzureRmExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="5598c-190">Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="5598c-190">Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="5598c-191">Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="5598c-191">Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="5598c-192">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="5598c-192">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="5598c-193">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5598c-193">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="5598c-194">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="5598c-194">Added policy remediation cmdlets</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5598c-195">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-195">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5598c-196">Foi adicionado suporte para as partilhas de ficheiro do Azure nos serviços de recuperação.</span><span class="sxs-lookup"><span data-stu-id="5598c-196">Added support for azure file shares in recovery services.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-197">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-197">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-198">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="5598c-198">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="5598c-199">Permitir a listagem de recursos a utilizar o parâmetro "-ResourceId" para "-GetAzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="5598c-199">Allow listing resources using the '-ResourceId' parameter for 'Get-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-200">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-200">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-201">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="5598c-201">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5598c-202">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5598c-202">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5598c-203">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="5598c-203">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="5598c-204">Correção de "Add-AzureRmServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="5598c-204">Fix 'Add-AzureRmServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="5598c-205">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="5598c-205">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="5598c-206">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="5598c-206">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="5598c-207">Corrigir "Update-AzureRmServiceFabricDurability" para atualizar a configuração do cluster antes de iniciar a operação de VMSS CreateOrUpdate.</span><span class="sxs-lookup"><span data-stu-id="5598c-207">Fix 'Update-AzureRmServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="6110---october-2018"></a><span data-ttu-id="5598c-208">6.11.0 - outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-208">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-209">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-209">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-210">Corrigir o problema do Get-AzureRmSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="5598c-210">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="5598c-211">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="5598c-211">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="5598c-212">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-212">AzureRM.Backup</span></span>
* <span data-ttu-id="5598c-213">Cmdlets do Azure Backup preteridos.</span><span class="sxs-lookup"><span data-stu-id="5598c-213">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-214">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-214">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-215">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais as redes aceleradas vão ser ativadas quando a utilizar o simples conjunto de parâmetros para "New-AzureRmVm"</span><span class="sxs-lookup"><span data-stu-id="5598c-215">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="5598c-216">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5598c-216">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5598c-217">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5598c-217">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5598c-218">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="5598c-218">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="5598c-219">Get-AzureRmDataLakeStoreVirtualNetworkRule: obtém ou listas a regra de rede virtual do Azure Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5598c-219">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="5598c-220">Add-AzureRmDataLakeStoreVirtualNetworkRule: adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5598c-220">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="5598c-221">Set-AzureRmDataLakeStoreVirtualNetworkRule: modifica a regra especificada de rede virtual na conta do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5598c-221">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="5598c-222">Remove-AzureRmDataLakeStoreVirtualNetworkRule: elimina uma regra de rede virtual do Azure Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5598c-222">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-223">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-223">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-224">Atualizar o cmdlet Test-AzureRmNetworkWatcherConnectivity, passar o valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="5598c-224">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="5598c-225">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5598c-225">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-226">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-226">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-227">Corrigir o problema em que Get-AzureRMRoleDefinition lança uma exceção ininteligível (quando o perfil predefinido não tem subscrição e não é especificado um âmbito) ao adicionar uma exceção significativa no cenário.</span><span class="sxs-lookup"><span data-stu-id="5598c-227">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="5598c-228">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="5598c-228">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="5598c-229">6.10.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-229">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="5598c-230">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-230">Azure.Storage</span></span>
* <span data-ttu-id="5598c-231">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="5598c-231">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="5598c-232">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="5598c-232">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="5598c-233">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="5598c-233">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="5598c-234">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5598c-234">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="5598c-235">Suporte para Get-AzureRmCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="5598c-235">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-236">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-236">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-237">Correção de Get-AzureRmVM -ResourceGroupName <rg> para devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="5598c-237">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="5598c-238">Adição de um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzureRmVmss.</span><span class="sxs-lookup"><span data-stu-id="5598c-238">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="5598c-239">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="5598c-239">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5598c-240">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5598c-240">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5598c-241">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="5598c-241">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-242">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-242">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-243">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="5598c-243">Added NetworkProfile functionality.</span></span> <span data-ttu-id="5598c-244">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="5598c-244">new cmdlets added</span></span>
    - <span data-ttu-id="5598c-245">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5598c-245">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5598c-246">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5598c-246">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5598c-247">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5598c-247">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5598c-248">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5598c-248">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5598c-249">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-249">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="5598c-250">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-250">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="5598c-251">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-251">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="5598c-252">Adição do cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="5598c-252">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="5598c-253">Adição do cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-253">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="5598c-254">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5598c-254">AzureRM.RedisCache</span></span>
* <span data-ttu-id="5598c-255">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="5598c-255">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="5598c-256">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="5598c-256">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-257">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-257">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-258">Adição do parâmetro -Mode em falta a Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="5598c-258">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="5598c-259">Correção do erro de commandlet Get-AzureRmProviderOperation para as operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="5598c-259">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-260">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-260">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-261">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="5598c-261">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5598c-262">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-262">AzureRM.Storage</span></span>
* <span data-ttu-id="5598c-263">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="5598c-263">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="5598c-264">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="5598c-264">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-265">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-265">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-266">Novo Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="5598c-266">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="5598c-267">Novos Cmdlets New-AzureRMWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="5598c-267">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="5598c-268">6.9.0 - setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-268">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5598c-269">Geral</span><span class="sxs-lookup"><span data-stu-id="5598c-269">General</span></span>
* <span data-ttu-id="5598c-270">AzureRM.SignalR foi adicionado ao módulo de rollup AzureRM</span><span class="sxs-lookup"><span data-stu-id="5598c-270">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5598c-271">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-271">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-272">Alterações menores ao código comum do armazenamento</span><span class="sxs-lookup"><span data-stu-id="5598c-272">Minor changes to the storage common code</span></span>
* <span data-ttu-id="5598c-273">Ficheiros de ajuda atualizados para incluírem todos os tipos de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5598c-273">Updated help files to include full parameter types.</span></span>
* <span data-ttu-id="5598c-274">-ServicePrincipal alterado para non-mandatory no conjunto de parâmetros ServicePrincipalCertificateWithSubscriptionId</span><span class="sxs-lookup"><span data-stu-id="5598c-274">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="5598c-275">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-275">Azure.Storage</span></span>
* <span data-ttu-id="5598c-276">Suporte para a criação de Contexto de Armazenamento com OAuth.</span><span class="sxs-lookup"><span data-stu-id="5598c-276">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="5598c-277">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="5598c-277">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="5598c-278">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="5598c-278">AzureRM.Cdn</span></span>
* <span data-ttu-id="5598c-279">Standard_Microsoft adicionado ao sku de preços de Cdn.</span><span class="sxs-lookup"><span data-stu-id="5598c-279">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-280">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-280">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-281">Dependências no Cofre de Chaves e no Armazenamento movidas para as dependências comuns</span><span class="sxs-lookup"><span data-stu-id="5598c-281">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="5598c-282">Adicionado suporte para mais tamanhos de máquinas virtuais para cmdlets do AEM</span><span class="sxs-lookup"><span data-stu-id="5598c-282">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="5598c-283">Adicionado o parâmetro PublicIPPrefix a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-283">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="5598c-284">Adicionado o parâmetro ResourceId ao cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="5598c-284">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="5598c-285">Adicionado o cmdlet Invoke-AzureRmVmssVMRunCommand cmdlet</span><span class="sxs-lookup"><span data-stu-id="5598c-285">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="5598c-286">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="5598c-286">AzureRM.Dns</span></span>
* <span data-ttu-id="5598c-287">Suporte adicionado para registo de alias durante a criação de registo dns</span><span class="sxs-lookup"><span data-stu-id="5598c-287">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5598c-288">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5598c-288">AzureRM.Insights</span></span>
* <span data-ttu-id="5598c-289">Corrigidos os problemas n.º 6833 e 7102 (Área Definições de Diagnóstico)</span><span class="sxs-lookup"><span data-stu-id="5598c-289">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="5598c-290">Problemas com o nome predefinido, ou seja, “serviço”, durante a criação e listagem/obtenção das definições de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="5598c-290">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="5598c-291">Problemas ao criar definições de diagnóstico com categorias</span><span class="sxs-lookup"><span data-stu-id="5598c-291">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="5598c-292">Adicionada mensagem de preterição aos parâmetros time grains das métricas</span><span class="sxs-lookup"><span data-stu-id="5598c-292">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="5598c-293">Os parâmetros timegrains ainda são aceites (esta não é uma alteração interruptiva), mas são ignorados no back-end, uma vez que apenas PT1M é válido</span><span class="sxs-lookup"><span data-stu-id="5598c-293">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-294">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-295">Alterações aos cmdlets LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="5598c-295">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="5598c-296">LoadBalancerInboundNatPoolConfig: parâmetros IdleTimeoutInMinutes, EnableFloatingIp e EnableTcpReset adicionados</span><span class="sxs-lookup"><span data-stu-id="5598c-296">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="5598c-297">LoadBalancerInboundNatRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-297">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="5598c-298">LoadBalancerRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-298">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="5598c-299">LoadBalancerProbeConfig: suporte para o valor "Https" para o parâmetro Protocol adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-299">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="5598c-300">Adicionados comandos novos para o sub-recurso OutboundRule de LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="5598c-300">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="5598c-301">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-301">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5598c-302">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-302">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5598c-303">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-303">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5598c-304">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-304">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5598c-305">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-305">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="5598c-306">Adicionada propriedade HostedWorkloads nova para PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="5598c-306">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="5598c-307">Adicionados cmdlets novos para a funcionalidade: Azure Firewall através de ARM</span><span class="sxs-lookup"><span data-stu-id="5598c-307">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="5598c-308">Get-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-308">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="5598c-309">Set-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-309">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="5598c-310">New-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-310">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="5598c-311">Remove-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-311">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="5598c-312">New-AzureRmFirewallApplicationRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-312">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="5598c-313">New-AzureRmFirewallApplicationRule adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-313">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="5598c-314">New-AzureRmFirewallNatRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-314">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="5598c-315">New-AzureRmFirewallNatRule adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-315">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="5598c-316">New-AzureRmFirewallNetworkRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-316">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="5598c-317">New-AzureRmFirewallNetworkRule adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-317">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="5598c-318">Adicionado suporte para o certificado de raiz fidedigna e configuração de dimensionamento automático no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="5598c-318">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="5598c-319">Novos cmdlets adicionados:</span><span class="sxs-lookup"><span data-stu-id="5598c-319">New Cmdlets added:</span></span>
      - <span data-ttu-id="5598c-320">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-320">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5598c-321">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-321">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5598c-322">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-322">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5598c-323">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-323">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5598c-324">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-324">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5598c-325">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-325">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="5598c-326">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-326">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="5598c-327">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-327">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="5598c-328">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-328">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="5598c-329">Cmdlets updated with optonal parameter -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-329">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="5598c-330">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5598c-330">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="5598c-331">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5598c-331">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="5598c-332">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="5598c-332">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="5598c-333">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="5598c-333">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="5598c-334">Cmdlets atualizados com parâmetro opcional -AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-334">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="5598c-335">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5598c-335">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="5598c-336">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5598c-336">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="5598c-337">Adicionado cmdlet para Ponto Final da Interface Get-AzureInterfaceEndpoint</span><span class="sxs-lookup"><span data-stu-id="5598c-337">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="5598c-338">Adicionado suporte para vários prefixos de endereços numa sub-rede.</span><span class="sxs-lookup"><span data-stu-id="5598c-338">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="5598c-339">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="5598c-339">Updated cmdlets:</span></span>
  - <span data-ttu-id="5598c-340">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-340">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5598c-341">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-341">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5598c-342">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-342">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5598c-343">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-343">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5598c-344">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-344">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="5598c-345">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-345">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="5598c-346">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-346">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="5598c-347">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-347">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="5598c-348">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-348">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="5598c-349">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-349">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="5598c-350">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-350">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="5598c-351">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-351">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="5598c-352">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-352">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="5598c-353">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-353">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="5598c-354">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-354">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="5598c-355">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-355">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="5598c-356">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-356">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="5598c-357">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-357">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="5598c-358">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="5598c-358">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="5598c-359">Adição de cmdlets para delegação de sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-359">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="5598c-360">New-AzureRmDelegation: cria uma delegação nova, que pode ser adicionada a uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-360">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="5598c-361">Remove-AzureRmDelegation: recebe uma sub-rede e remove o nome da delegação especificado dessa sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-361">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="5598c-362">Add-AzureRmDelegation: recebe uma sub-rede e adiciona o nome de serviço especificado como delegação a essa sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-362">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="5598c-363">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="5598c-363">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="5598c-364">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="5598c-364">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="5598c-365">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5598c-365">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="5598c-366">Suporte para discos geridos</span><span class="sxs-lookup"><span data-stu-id="5598c-366">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="5598c-367">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5598c-367">AzureRM.RedisCache</span></span>
* <span data-ttu-id="5598c-368">Dependência de informações atualizada</span><span class="sxs-lookup"><span data-stu-id="5598c-368">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-369">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-369">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-370">New-AzureRmResourceGroupDeployment atualizado com parâmetro novo RollbackAction</span><span class="sxs-lookup"><span data-stu-id="5598c-370">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="5598c-371">Adicionado suporte para OnErrorDeployment com o parâmetro novo.</span><span class="sxs-lookup"><span data-stu-id="5598c-371">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="5598c-372">Suporte para identidades geridas nas atribuições de políticas.</span><span class="sxs-lookup"><span data-stu-id="5598c-372">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="5598c-373">Os parâmetros com valores predefinidos já não são necessários ao atribuir uma política com “New-AzureRmPolicyAssignment”</span><span class="sxs-lookup"><span data-stu-id="5598c-373">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="5598c-374">Adicionado cmdlet novo Get-AzureRmPolicyAlias para obter aliases de políticas</span><span class="sxs-lookup"><span data-stu-id="5598c-374">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-375">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-375">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-376">Problema n.º 7161 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-376">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="5598c-377">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="5598c-377">AzureRM.SignalR</span></span>
* <span data-ttu-id="5598c-378">Nomes dos SKUs atualizados para Free_F1 e Standard_S1</span><span class="sxs-lookup"><span data-stu-id="5598c-378">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="5598c-379">Adicionado campo de versão ao objeto PSSignalRResource e cadeia de ligação ao objeto PSSignalRKeys.</span><span class="sxs-lookup"><span data-stu-id="5598c-379">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5598c-380">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-380">AzureRM.Storage</span></span>
* <span data-ttu-id="5598c-381">Suporte para política Imutabilidade em AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-381">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="5598c-382">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="5598c-382">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="5598c-383">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5598c-383">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5598c-384">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5598c-384">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5598c-385">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5598c-385">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5598c-386">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5598c-386">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5598c-387">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="5598c-387">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="5598c-388">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="5598c-388">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="5598c-389">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-389">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="5598c-390">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-390">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="5598c-391">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-391">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="5598c-392">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-392">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-393">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-393">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-394">Adicionados dois cmdlets novos: Get-AzureRmDeletedWebApp e Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="5598c-394">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="5598c-395">O comutador New-AzureRmAppServicePlan -HyperV é adicionado para criar o plano do serviço de aplicações com contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="5598c-395">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="5598c-396">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - parâmetros novos (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) adicionados para criar e gerir a aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="5598c-396">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="5598c-397">6.8.1 - Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-397">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5598c-398">Geral</span><span class="sxs-lookup"><span data-stu-id="5598c-398">General</span></span>
* <span data-ttu-id="5598c-399">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5598c-399">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="5598c-400">Assemblagens de runtime comum atualizadas</span><span class="sxs-lookup"><span data-stu-id="5598c-400">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5598c-401">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5598c-401">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5598c-402">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5598c-402">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="5598c-403">Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-403">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="5598c-404">Agora, os cmdlets Import-AzureRmApiManagementApi e \*-AzureRmApiManagementCertificate identificam caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="5598c-404">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="5598c-405">Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-405">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="5598c-406">O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="5598c-406">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="5598c-407">Corrigido com a atualização para 4.0.4-nuget de pré-visualização</span><span class="sxs-lookup"><span data-stu-id="5598c-407">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="5598c-408">Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-408">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="5598c-409">Foi corrigido o filtro de Odata para procurar por nome de produto</span><span class="sxs-lookup"><span data-stu-id="5598c-409">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="5598c-410">Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-410">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="5598c-411">Foi corrigido o filtro de Odata para procurar por nome na API</span><span class="sxs-lookup"><span data-stu-id="5598c-411">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="5598c-412">Foi adicionado suporte para o logger de AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="5598c-412">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="5598c-413">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-413">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-414">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="5598c-414">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="5598c-415">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="5598c-415">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="5598c-416">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5598c-416">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="5598c-417">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="5598c-417">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-418">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-418">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-419">Representação de saída de cmdlet predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="5598c-419">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="5598c-420">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5598c-420">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="5598c-421">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="5598c-421">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="5598c-422">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-422">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-423">Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5598c-423">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-424">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-424">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-425">Problemas corrigidos</span><span class="sxs-lookup"><span data-stu-id="5598c-425">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5598c-426">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5598c-426">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5598c-427">Suporte adicionado para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="5598c-427">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="5598c-428">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="5598c-428">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="5598c-429">Suporte adicionado para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-429">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="5598c-430">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="5598c-430">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="5598c-431">Suporte adicionado para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5598c-431">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="5598c-432">Suporte adicionado para intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5598c-432">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="5598c-433">Suporte adicionado para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="5598c-433">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="5598c-434">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-434">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5598c-435">Geral</span><span class="sxs-lookup"><span data-stu-id="5598c-435">General</span></span>
* <span data-ttu-id="5598c-436">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5598c-436">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5598c-437">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-437">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-438">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="5598c-438">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-439">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-439">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-440">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="5598c-440">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="5598c-441">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="5598c-441">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="5598c-442">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="5598c-442">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="5598c-443">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="5598c-443">AzureRM.IotHub</span></span>
* <span data-ttu-id="5598c-444">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="5598c-444">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-445">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-445">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-446">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="5598c-446">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="5598c-447">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5598c-447">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="5598c-448">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="5598c-448">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-449">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-449">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-450">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5598c-450">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-451">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-451">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-452">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="5598c-452">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5598c-453">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5598c-453">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5598c-454">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="5598c-454">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="5598c-455">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="5598c-455">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="5598c-456">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="5598c-456">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="5598c-457">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="5598c-457">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="5598c-458">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5598c-458">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="5598c-459">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5598c-459">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="5598c-460">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="5598c-460">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-461">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-461">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-462">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="5598c-462">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="5598c-463">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-463">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-464">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-464">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-465">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-465">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5598c-466">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="5598c-466">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="5598c-467">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="5598c-467">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="5598c-468">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="5598c-468">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="5598c-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-469">Azure.Storage</span></span>
* <span data-ttu-id="5598c-470">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="5598c-470">Remove the 5TB limitation for Azure File Share quota</span></span>
* <span data-ttu-id="5598c-471">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="5598c-471">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5598c-472">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5598c-472">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5598c-473">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-473">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="5598c-474">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5598c-474">Azure.AnalysisServices</span></span>
* <span data-ttu-id="5598c-475">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-475">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5598c-476">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5598c-476">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5598c-477">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-477">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="5598c-478">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="5598c-478">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="5598c-479">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-479">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="5598c-480">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5598c-480">AzureRM.Automation</span></span>
* <span data-ttu-id="5598c-481">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-481">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="5598c-482">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-482">AzureRM.Backup</span></span>
* <span data-ttu-id="5598c-483">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="5598c-484">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="5598c-484">AzureRM.Batch</span></span>
* <span data-ttu-id="5598c-485">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="5598c-486">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="5598c-486">AzureRM.Billing</span></span>
* <span data-ttu-id="5598c-487">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-487">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="5598c-488">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="5598c-488">AzureRM.Cdn</span></span>
* <span data-ttu-id="5598c-489">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-489">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="5598c-490">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5598c-490">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="5598c-491">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-491">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-492">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-492">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-493">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-493">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5598c-494">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-494">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="5598c-495">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="5598c-495">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="5598c-496">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="5598c-496">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="5598c-497">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="5598c-497">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="5598c-498">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="5598c-498">AzureRM.Consumption</span></span>
* <span data-ttu-id="5598c-499">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-499">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="5598c-500">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5598c-500">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="5598c-501">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-501">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="5598c-502">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="5598c-502">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="5598c-503">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-503">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="5598c-504">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="5598c-504">AzureRM.DataFactories</span></span>
* <span data-ttu-id="5598c-505">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-505">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5598c-506">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5598c-506">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5598c-507">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-507">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="5598c-508">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="5598c-508">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="5598c-509">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-509">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5598c-510">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5598c-510">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5598c-511">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="5598c-511">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="5598c-512">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="5598c-512">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="5598c-513">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-513">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5598c-514">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5598c-514">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="5598c-515">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="5598c-515">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="5598c-516">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-516">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="5598c-517">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="5598c-517">AzureRM.Dns</span></span>
* <span data-ttu-id="5598c-518">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-518">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="5598c-519">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5598c-519">AzureRM.EventGrid</span></span>
* <span data-ttu-id="5598c-520">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-520">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5598c-521">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5598c-521">AzureRM.EventHub</span></span>
* <span data-ttu-id="5598c-522">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-522">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="5598c-523">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5598c-523">AzureRM.HDInsight</span></span>
* <span data-ttu-id="5598c-524">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-524">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5598c-525">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5598c-525">AzureRM.Insights</span></span>
* <span data-ttu-id="5598c-526">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-526">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="5598c-527">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="5598c-527">AzureRM.IotHub</span></span>
* <span data-ttu-id="5598c-528">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-528">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5598c-529">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5598c-529">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5598c-530">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-530">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="5598c-531">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5598c-531">AzureRM.LogicApp</span></span>
* <span data-ttu-id="5598c-532">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-532">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="5598c-533">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="5598c-533">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="5598c-534">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-534">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="5598c-535">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="5598c-535">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="5598c-536">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-536">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="5598c-537">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="5598c-537">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="5598c-538">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-538">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="5598c-539">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="5598c-539">AzureRM.Media</span></span>
* <span data-ttu-id="5598c-540">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-540">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-541">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-541">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-542">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="5598c-542">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="5598c-543">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="5598c-543">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="5598c-544">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="5598c-544">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="5598c-545">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="5598c-545">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="5598c-546">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="5598c-546">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="5598c-547">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="5598c-547">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="5598c-548">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="5598c-548">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="5598c-549">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="5598c-549">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="5598c-550">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="5598c-550">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="5598c-551">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-551">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="5598c-552">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5598c-552">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="5598c-553">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-553">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="5598c-554">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5598c-554">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="5598c-555">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-555">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="5598c-556">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5598c-556">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="5598c-557">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-557">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="5598c-558">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5598c-558">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="5598c-559">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-559">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5598c-560">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-560">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5598c-561">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="5598c-561">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="5598c-562">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="5598c-562">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="5598c-563">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="5598c-563">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="5598c-564">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-564">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5598c-565">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="5598c-565">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="5598c-566">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="5598c-566">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="5598c-567">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="5598c-567">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="5598c-568">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5598c-568">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="5598c-569">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-569">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="5598c-570">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5598c-570">AzureRM.RedisCache</span></span>
* <span data-ttu-id="5598c-571">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-571">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="5598c-572">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="5598c-572">AzureRM.Relay</span></span>
* <span data-ttu-id="5598c-573">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-573">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-574">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-574">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-575">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="5598c-575">Support template deployment at subscription scope.</span></span> <span data-ttu-id="5598c-576">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5598c-576">Add new Cmdlets:</span></span>
    - <span data-ttu-id="5598c-577">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-577">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="5598c-578">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-578">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="5598c-579">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-579">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="5598c-580">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-580">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="5598c-581">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-581">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="5598c-582">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="5598c-582">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="5598c-583">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="5598c-583">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="5598c-584">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="5598c-584">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="5598c-585">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-585">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="5598c-586">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-586">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="5598c-587">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="5598c-587">AzureRM.Scheduler</span></span>
* <span data-ttu-id="5598c-588">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-588">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-589">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-589">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-590">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-590">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5598c-591">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5598c-591">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5598c-592">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-592">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-593">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-593">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-594">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-594">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5598c-595">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-595">AzureRM.Storage</span></span>
* <span data-ttu-id="5598c-596">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-596">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="5598c-597">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="5598c-597">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="5598c-598">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-598">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="5598c-599">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="5598c-599">AzureRM.Tags</span></span>
* <span data-ttu-id="5598c-600">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-600">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5598c-601">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5598c-601">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5598c-602">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-602">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="5598c-603">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="5598c-603">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="5598c-604">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-604">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-605">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-605">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-606">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-606">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="5598c-607">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-607">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5598c-608">Geral</span><span class="sxs-lookup"><span data-stu-id="5598c-608">General</span></span>
* <span data-ttu-id="5598c-609">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="5598c-609">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5598c-610">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-610">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-611">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="5598c-611">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="5598c-612">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-612">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5598c-613">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-613">Azure.Storage</span></span>
* <span data-ttu-id="5598c-614">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="5598c-614">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="5598c-615">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5598c-615">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5598c-616">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5598c-616">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5598c-617">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-617">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="5598c-618">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="5598c-618">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="5598c-619">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-619">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="5598c-620">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="5598c-620">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="5598c-621">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="5598c-621">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="5598c-622">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="5598c-622">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-623">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-623">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-624">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="5598c-624">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="5598c-625">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="5598c-625">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="5598c-626">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="5598c-626">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="5598c-627">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="5598c-627">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="5598c-628">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="5598c-628">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="5598c-629">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="5598c-629">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="5598c-630">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="5598c-630">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="5598c-631">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="5598c-631">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="5598c-632">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="5598c-632">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="5598c-633">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="5598c-633">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5598c-634">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5598c-634">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5598c-635">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="5598c-635">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="5598c-636">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="5598c-636">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="5598c-637">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-637">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="5598c-638">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="5598c-638">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5598c-639">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5598c-639">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5598c-640">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="5598c-640">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5598c-641">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5598c-641">AzureRM.EventHub</span></span>
* <span data-ttu-id="5598c-642">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="5598c-642">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5598c-643">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5598c-643">AzureRM.Insights</span></span>
* <span data-ttu-id="5598c-644">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="5598c-644">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="5598c-645">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="5598c-645">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5598c-646">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5598c-646">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5598c-647">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-647">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-648">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-648">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-649">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="5598c-649">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-650">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-650">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-651">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="5598c-651">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="5598c-652">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="5598c-652">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-653">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-653">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-654">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="5598c-654">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="5598c-655">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="5598c-655">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="5598c-656">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-656">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-657">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5598c-657">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="5598c-658">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-658">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="5598c-659">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5598c-659">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="5598c-660">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="5598c-660">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="5598c-661">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="5598c-661">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="5598c-662">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="5598c-662">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="5598c-663">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="5598c-663">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="5598c-664">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="5598c-664">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5598c-665">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-665">AzureRM.Storage</span></span>
* <span data-ttu-id="5598c-666">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="5598c-666">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="5598c-667">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="5598c-667">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="5598c-668">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5598c-668">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="5598c-669">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5598c-669">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="5598c-670">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5598c-670">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="5598c-671">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="5598c-671">AzureRM.Tags</span></span>
* <span data-ttu-id="5598c-672">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="5598c-672">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="5598c-673">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-673">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-674">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-674">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-675">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="5598c-675">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5598c-676">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-676">Azure.Storage</span></span>
* <span data-ttu-id="5598c-677">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="5598c-677">Support Upload Blob or File with write only Sas token</span></span>
* <span data-ttu-id="5598c-678">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5598c-678">Set-AzureStorageBlobContent</span></span>
* <span data-ttu-id="5598c-679">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5598c-679">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5598c-680">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5598c-680">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5598c-681">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="5598c-681">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="5598c-682">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5598c-682">AzureRM.Automation</span></span>
* <span data-ttu-id="5598c-683">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="5598c-683">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-684">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-684">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-685">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="5598c-685">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="5598c-686">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="5598c-686">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="5598c-687">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="5598c-687">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="5598c-688">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="5598c-688">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="5598c-689">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="5598c-689">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5598c-690">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5598c-690">AzureRM.EventHub</span></span>
* <span data-ttu-id="5598c-691">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="5598c-691">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5598c-692">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5598c-692">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5598c-693">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5598c-693">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="5598c-694">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5598c-694">AzureRM.LogicApp</span></span>
* <span data-ttu-id="5598c-695">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="5598c-695">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-696">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-696">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-697">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="5598c-697">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="5598c-698">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="5598c-698">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="5598c-699">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="5598c-699">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="5598c-700">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="5598c-700">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="5598c-701">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="5598c-701">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="5598c-702">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="5598c-702">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="5598c-703">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="5598c-703">AzureRM.Relay</span></span>
* <span data-ttu-id="5598c-704">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="5598c-704">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-705">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-705">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-706">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="5598c-706">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="5598c-707">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="5598c-707">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="5598c-708">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5598c-708">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="5598c-709">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="5598c-709">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="5598c-710">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="5598c-710">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-711">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-711">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-712">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="5598c-712">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="5598c-713">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="5598c-713">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="5598c-714">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5598c-714">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5598c-715">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5598c-715">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5598c-716">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5598c-716">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5598c-717">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5598c-717">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5598c-718">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5598c-718">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="5598c-719">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="5598c-719">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5598c-720">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5598c-720">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5598c-721">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="5598c-721">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-722">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-722">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-723">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="5598c-723">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="5598c-724">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-724">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="5598c-725">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-725">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-726">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-726">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-727">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="5598c-727">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="5598c-728">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="5598c-728">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="5598c-729">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="5598c-729">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="5598c-730">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-730">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5598c-731">Geral</span><span class="sxs-lookup"><span data-stu-id="5598c-731">General</span></span>
* <span data-ttu-id="5598c-732">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="5598c-732">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5598c-733">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-733">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-734">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="5598c-734">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-735">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-735">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-736">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="5598c-736">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="5598c-737">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="5598c-737">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="5598c-738">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-738">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="5598c-739">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="5598c-739">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="5598c-740">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-740">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="5598c-741">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="5598c-741">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="5598c-742">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-742">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="5598c-743">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="5598c-743">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="5598c-744">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="5598c-744">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="5598c-745">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5598c-745">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="5598c-746">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5598c-746">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="5598c-747">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5598c-747">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5598c-748">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5598c-748">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5598c-749">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="5598c-749">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="5598c-750">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="5598c-750">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="5598c-751">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="5598c-751">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="5598c-752">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="5598c-752">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5598c-753">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5598c-753">AzureRM.EventHub</span></span>
* <span data-ttu-id="5598c-754">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="5598c-754">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="5598c-755">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="5598c-755">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="5598c-756">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="5598c-756">Provided Default Parameter set.</span></span>
* <span data-ttu-id="5598c-757">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="5598c-757">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5598c-758">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5598c-758">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5598c-759">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="5598c-759">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-760">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-760">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-761">Apresentação de novos SKUs para VirtualNetworkGateways com redundância entre zonas</span><span class="sxs-lookup"><span data-stu-id="5598c-761">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="5598c-762">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="5598c-762">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="5598c-763">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="5598c-763">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="5598c-764">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="5598c-764">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="5598c-765">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="5598c-765">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5598c-766">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="5598c-766">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5598c-767">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="5598c-767">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5598c-768">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="5598c-768">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="5598c-769">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="5598c-769">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="5598c-770">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="5598c-770">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5598c-771">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-771">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5598c-772">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="5598c-772">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="5598c-773">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="5598c-773">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="5598c-774">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="5598c-774">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-775">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-775">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-776">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="5598c-776">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="5598c-777">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5598c-777">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="5598c-778">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5598c-778">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="5598c-779">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="5598c-779">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="5598c-780">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="5598c-780">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="5598c-781">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5598c-781">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="5598c-782">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="5598c-782">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="5598c-783">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="5598c-783">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="5598c-784">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5598c-784">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="5598c-785">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="5598c-785">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="5598c-786">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="5598c-786">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="5598c-787">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="5598c-787">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="5598c-788">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="5598c-788">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="5598c-789">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5598c-789">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5598c-790">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="5598c-790">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-791">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-791">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-792">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="5598c-792">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="5598c-793">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="5598c-793">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="5598c-794">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-794">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-795">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-795">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-796">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="5598c-796">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="5598c-797">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="5598c-797">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5598c-798">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5598c-798">Azure.Storage</span></span>
* <span data-ttu-id="5598c-799">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="5598c-799">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-800">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-800">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-801">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="5598c-801">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="5598c-802">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="5598c-802">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="5598c-803">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="5598c-803">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="5598c-804">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="5598c-804">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="5598c-805">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="5598c-805">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="5598c-806">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="5598c-806">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="5598c-807">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5598c-807">Start-AzureRmVM</span></span>
    - <span data-ttu-id="5598c-808">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5598c-808">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="5598c-809">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5598c-809">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="5598c-810">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5598c-810">Set-AzureRmVM</span></span>
    - <span data-ttu-id="5598c-811">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="5598c-811">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="5598c-812">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-812">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="5598c-813">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="5598c-813">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="5598c-814">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="5598c-814">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="5598c-815">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-815">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="5598c-816">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-816">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="5598c-817">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-817">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="5598c-818">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5598c-818">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="5598c-819">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="5598c-819">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="5598c-820">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="5598c-820">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="5598c-821">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="5598c-821">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="5598c-822">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="5598c-822">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="5598c-823">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="5598c-823">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="5598c-824">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="5598c-824">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="5598c-825">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="5598c-825">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="5598c-826">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5598c-826">AzureRM.EventGrid</span></span>
* <span data-ttu-id="5598c-827">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="5598c-827">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5598c-828">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5598c-828">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5598c-829">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="5598c-829">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="5598c-830">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5598c-830">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="5598c-831">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="5598c-831">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="5598c-832">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="5598c-832">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="5598c-833">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="5598c-833">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5598c-834">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5598c-834">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5598c-835">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="5598c-835">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="5598c-836">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="5598c-836">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-837">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-837">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-838">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="5598c-838">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5598c-839">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5598c-839">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5598c-840">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-840">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-841">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-841">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-842">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="5598c-842">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="5598c-843">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="5598c-843">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="5598c-844">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-844">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="5598c-845">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5598c-845">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="5598c-846">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="5598c-846">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="5598c-847">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-847">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-848">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-848">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-849">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="5598c-849">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5598c-850">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5598c-850">AzureRM.Compute</span></span>
* <span data-ttu-id="5598c-851">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="5598c-851">VMSS VM Update feature</span></span>
    - <span data-ttu-id="5598c-852">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="5598c-852">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="5598c-853">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="5598c-853">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5598c-854">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5598c-854">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5598c-855">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="5598c-855">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="5598c-856">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="5598c-856">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="5598c-857">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="5598c-857">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="5598c-858">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="5598c-858">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="5598c-859">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="5598c-859">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="5598c-860">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5598c-860">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5598c-861">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="5598c-861">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="5598c-862">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-862">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-863">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="5598c-863">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5598c-864">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5598c-864">AzureRM.Resources</span></span>
* <span data-ttu-id="5598c-865">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="5598c-865">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="5598c-866">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="5598c-866">AzureRM.Scheduler</span></span>
* <span data-ttu-id="5598c-867">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="5598c-867">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="5598c-868">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-868">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-869">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="5598c-869">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="5598c-870">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-870">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="5598c-871">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="5598c-871">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="5598c-872">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="5598c-872">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="5598c-873">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="5598c-873">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="5598c-874">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-874">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5598c-875">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5598c-875">AzureRM.Websites</span></span>
* <span data-ttu-id="5598c-876">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="5598c-876">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="5598c-877">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="5598c-877">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5598c-878">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5598c-878">AzureRM.Profile</span></span>
* <span data-ttu-id="5598c-879">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="5598c-879">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5598c-880">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5598c-880">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5598c-881">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="5598c-881">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5598c-882">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5598c-882">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5598c-883">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="5598c-883">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="5598c-884">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5598c-884">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="5598c-885">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="5598c-885">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="5598c-886">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="5598c-886">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="5598c-887">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="5598c-887">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="5598c-888">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="5598c-888">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="5598c-889">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="5598c-889">Added support for MSI identity</span></span>
* <span data-ttu-id="5598c-890">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="5598c-890">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="5598c-891">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="5598c-891">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="5598c-892">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-892">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="5598c-893">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="5598c-893">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="5598c-894">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="5598c-894">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="5598c-895">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="5598c-895">AzureRM.Batch</span></span>
* <span data-ttu-id="5598c-896">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="5598c-896">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="5598c-897">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="5598c-897">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="5598c-898">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="5598c-898">AzureRM.Consumption</span></span>
* <span data-ttu-id="5598c-899">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5598c-899">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5598c-900">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5598c-900">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5598c-901">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="5598c-901">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="5598c-902">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5598c-902">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="5598c-903">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5598c-903">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="5598c-904">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5598c-904">AzureRM.Network</span></span>
* <span data-ttu-id="5598c-905">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="5598c-905">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="5598c-906">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="5598c-906">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="5598c-907">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="5598c-907">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="5598c-908">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5598c-908">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="5598c-909">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-909">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="5598c-910">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5598c-910">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="5598c-911">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-911">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="5598c-912">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="5598c-912">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="5598c-913">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5598c-913">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5598c-914">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5598c-914">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5598c-915">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="5598c-915">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5598c-916">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5598c-916">AzureRM.Sql</span></span>
* <span data-ttu-id="5598c-917">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="5598c-917">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="5598c-918">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="5598c-918">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="5598c-919">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="5598c-919">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="5598c-920">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="5598c-920">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="5598c-921">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="5598c-921">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="5598c-922">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-922">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="5598c-923">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="5598c-923">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="5598c-924">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="5598c-924">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="5598c-925">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="5598c-925">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="5598c-926">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5598c-926">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5598c-927">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5598c-927">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5598c-928">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="5598c-928">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>