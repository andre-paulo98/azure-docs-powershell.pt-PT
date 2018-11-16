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
ms.openlocfilehash: 8a7b184ed06eb078956229fa67d02840014e3aaf
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574537"
---
# <a name="release-notes"></a><span data-ttu-id="7c912-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="7c912-103">Release notes</span></span>

<span data-ttu-id="7c912-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="7c912-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6120---november-2018"></a><span data-ttu-id="7c912-105">6.12.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-105">6.12.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-106">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-107">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="7c912-107">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="7c912-108">Mudar o nome do parâmetro TenantId no cmdlet Connect-AzureRmAccount para Tenant e adicionar um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="7c912-108">Rename param TenantId in cmdlet Connect-AzureRmAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="7c912-109">Descrição de TenantId atualizada para Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="7c912-109">Updated TenantId description for Connect-AzureRmAccount</span></span>
* <span data-ttu-id="7c912-110">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="7c912-110">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="7c912-111">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="7c912-111">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="7c912-112">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="7c912-112">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="7c912-113">Corrigido o problema em que "Disconnect-AzureRmAccount" é lançado se não estiver ligado</span><span class="sxs-lookup"><span data-stu-id="7c912-113">Fix issue where 'Disconnect-AzureRmAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a><span data-ttu-id="7c912-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="7c912-114">AzureRM.Automation</span></span>
* <span data-ttu-id="7c912-115">Foi mudado o nome do ficheiro DLL de cmdlett para Microsoft.Azure.Commands.Automation.dll</span><span class="sxs-lookup"><span data-stu-id="7c912-115">Renamed cmdlet DLL filename to Microsoft.Azure.Commands.Automation.dll</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="7c912-116">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7c912-116">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="7c912-117">Adicionar a operação Get-AzureRmCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="7c912-117">Add Get-AzureRmCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-118">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-118">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-119">Adicionar os cmdlets Add-AzureRmVmssVMDataDisk e Remove-AzureRmVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="7c912-119">Add Add-AzureRmVmssVMDataDisk and Remove-AzureRmVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="7c912-120">Get-AzureRmVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="7c912-120">Get-AzureRmVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="7c912-121">Corrigidos os valores de opção SetAzureRmVMChefExtension -BootstrapOptions e -JsonAttribute no formato json.</span><span class="sxs-lookup"><span data-stu-id="7c912-121">Fixed SetAzureRmVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7c912-122">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c912-122">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c912-123">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="7c912-123">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="7c912-124">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="7c912-124">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="7c912-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7c912-125">AzureRM.Insights</span></span>
* <span data-ttu-id="7c912-126">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="7c912-126">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="7c912-127">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="7c912-127">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="7c912-128">Corrigido o problema n.º 7513 [Insights] Set-AzureRMDiagnosticSetting requer especificação explícita das categorias durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="7c912-128">Fixed issue #7513 [Insights] Set-AzureRMDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="7c912-129">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="7c912-129">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-130">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-130">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-131">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="7c912-131">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="7c912-132">Get-AzureRmExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="7c912-132">Get-AzureRmExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="7c912-133">Get-AzureRmExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="7c912-133">Get-AzureRmExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="7c912-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7c912-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="7c912-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="7c912-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="7c912-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="7c912-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="7c912-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7c912-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="7c912-138">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7c912-138">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="7c912-139">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="7c912-139">Added policy remediation cmdlets</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7c912-140">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7c912-140">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7c912-141">Foi adicionado suporte para as partilhas de ficheiro do Azure nos serviços de recuperação.</span><span class="sxs-lookup"><span data-stu-id="7c912-141">Added support for azure file shares in recovery services.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-142">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-142">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-143">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="7c912-143">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="7c912-144">Permitir a listagem de recursos a utilizar o parâmetro "-ResourceId" para "-GetAzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="7c912-144">Allow listing resources using the '-ResourceId' parameter for 'Get-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-145">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-145">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-146">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="7c912-146">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7c912-147">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7c912-147">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7c912-148">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="7c912-148">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="7c912-149">Correção de "Add-AzureRmServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="7c912-149">Fix 'Add-AzureRmServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="7c912-150">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="7c912-150">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="7c912-151">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="7c912-151">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="7c912-152">Corrigir "Update-AzureRmServiceFabricDurability" para atualizar a configuração do cluster antes de iniciar a operação de VMSS CreateOrUpdate.</span><span class="sxs-lookup"><span data-stu-id="7c912-152">Fix 'Update-AzureRmServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="6110---october-2018"></a><span data-ttu-id="7c912-153">6.11.0 - outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-153">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-154">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-154">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-155">Corrigir o problema do Get-AzureRmSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="7c912-155">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="7c912-156">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="7c912-156">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="7c912-157">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="7c912-157">AzureRM.Backup</span></span>
* <span data-ttu-id="7c912-158">Cmdlets do Azure Backup preteridos.</span><span class="sxs-lookup"><span data-stu-id="7c912-158">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-159">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-159">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-160">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais as redes aceleradas vão ser ativadas quando a utilizar o simples conjunto de parâmetros para "New-AzureRmVm"</span><span class="sxs-lookup"><span data-stu-id="7c912-160">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="7c912-161">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7c912-161">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7c912-162">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c912-162">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c912-163">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="7c912-163">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="7c912-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: obtém ou listas a regra de rede virtual do Azure Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7c912-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="7c912-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7c912-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="7c912-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: modifica a regra especificada de rede virtual na conta do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7c912-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="7c912-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: elimina uma regra de rede virtual do Azure Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7c912-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-168">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-168">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-169">Atualizar o cmdlet Test-AzureRmNetworkWatcherConnectivity, passar o valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="7c912-169">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="7c912-170">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7c912-170">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-171">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-171">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-172">Corrigir o problema em que Get-AzureRMRoleDefinition lança uma exceção ininteligível (quando o perfil predefinido não tem subscrição e não é especificado um âmbito) ao adicionar uma exceção significativa no cenário.</span><span class="sxs-lookup"><span data-stu-id="7c912-172">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="7c912-173">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="7c912-173">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="7c912-174">6.10.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-174">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="7c912-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-175">Azure.Storage</span></span>
* <span data-ttu-id="7c912-176">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="7c912-176">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="7c912-177">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="7c912-177">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="7c912-178">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="7c912-178">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="7c912-179">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7c912-179">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="7c912-180">Suporte para Get-AzureRmCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="7c912-180">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-181">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-181">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-182">Correção de Get-AzureRmVM -ResourceGroupName <rg> para devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="7c912-182">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="7c912-183">Adição de um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzureRmVmss.</span><span class="sxs-lookup"><span data-stu-id="7c912-183">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="7c912-184">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="7c912-184">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7c912-185">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7c912-185">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7c912-186">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="7c912-186">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-187">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-187">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-188">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="7c912-188">Added NetworkProfile functionality.</span></span> <span data-ttu-id="7c912-189">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="7c912-189">new cmdlets added</span></span>
    - <span data-ttu-id="7c912-190">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7c912-190">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="7c912-191">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7c912-191">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="7c912-192">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7c912-192">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="7c912-193">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7c912-193">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="7c912-194">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-194">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="7c912-195">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-195">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="7c912-196">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-196">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="7c912-197">Adição do cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="7c912-197">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="7c912-198">Adição do cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-198">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="7c912-199">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7c912-199">AzureRM.RedisCache</span></span>
* <span data-ttu-id="7c912-200">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="7c912-200">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="7c912-201">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="7c912-201">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-202">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-202">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-203">Adição do parâmetro -Mode em falta a Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="7c912-203">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="7c912-204">Correção do erro de commandlet Get-AzureRmProviderOperation para as operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="7c912-204">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7c912-205">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-205">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-206">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="7c912-206">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="7c912-207">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-207">AzureRM.Storage</span></span>
* <span data-ttu-id="7c912-208">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="7c912-208">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="7c912-209">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="7c912-209">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-210">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-210">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-211">Novo Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="7c912-211">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="7c912-212">Novos Cmdlets New-AzureRMWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="7c912-212">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="7c912-213">6.9.0 - setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-213">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7c912-214">Geral</span><span class="sxs-lookup"><span data-stu-id="7c912-214">General</span></span>
* <span data-ttu-id="7c912-215">AzureRM.SignalR foi adicionado ao módulo de rollup AzureRM</span><span class="sxs-lookup"><span data-stu-id="7c912-215">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7c912-216">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-216">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-217">Alterações menores ao código comum do armazenamento</span><span class="sxs-lookup"><span data-stu-id="7c912-217">Minor changes to the storage common code</span></span>
* <span data-ttu-id="7c912-218">Ficheiros de ajuda atualizados para incluírem todos os tipos de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7c912-218">Updated help files to include full parameter types.</span></span>
* <span data-ttu-id="7c912-219">-ServicePrincipal alterado para non-mandatory no conjunto de parâmetros ServicePrincipalCertificateWithSubscriptionId</span><span class="sxs-lookup"><span data-stu-id="7c912-219">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="7c912-220">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-220">Azure.Storage</span></span>
* <span data-ttu-id="7c912-221">Suporte para a criação de Contexto de Armazenamento com OAuth.</span><span class="sxs-lookup"><span data-stu-id="7c912-221">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="7c912-222">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="7c912-222">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="7c912-223">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="7c912-223">AzureRM.Cdn</span></span>
* <span data-ttu-id="7c912-224">Standard_Microsoft adicionado ao sku de preços de Cdn.</span><span class="sxs-lookup"><span data-stu-id="7c912-224">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-225">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-226">Dependências no Cofre de Chaves e no Armazenamento movidas para as dependências comuns</span><span class="sxs-lookup"><span data-stu-id="7c912-226">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="7c912-227">Adicionado suporte para mais tamanhos de máquinas virtuais para cmdlets do AEM</span><span class="sxs-lookup"><span data-stu-id="7c912-227">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="7c912-228">Adicionado o parâmetro PublicIPPrefix a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-228">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="7c912-229">Adicionado o parâmetro ResourceId ao cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="7c912-229">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="7c912-230">Adicionado o cmdlet Invoke-AzureRmVmssVMRunCommand cmdlet</span><span class="sxs-lookup"><span data-stu-id="7c912-230">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="7c912-231">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="7c912-231">AzureRM.Dns</span></span>
* <span data-ttu-id="7c912-232">Suporte adicionado para registo de alias durante a criação de registo dns</span><span class="sxs-lookup"><span data-stu-id="7c912-232">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="7c912-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7c912-233">AzureRM.Insights</span></span>
* <span data-ttu-id="7c912-234">Corrigidos os problemas n.º 6833 e 7102 (Área Definições de Diagnóstico)</span><span class="sxs-lookup"><span data-stu-id="7c912-234">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="7c912-235">Problemas com o nome predefinido, ou seja, “serviço”, durante a criação e listagem/obtenção das definições de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7c912-235">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="7c912-236">Problemas ao criar definições de diagnóstico com categorias</span><span class="sxs-lookup"><span data-stu-id="7c912-236">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="7c912-237">Adicionada mensagem de preterição aos parâmetros time grains das métricas</span><span class="sxs-lookup"><span data-stu-id="7c912-237">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="7c912-238">Os parâmetros timegrains ainda são aceites (esta não é uma alteração interruptiva), mas são ignorados no back-end, uma vez que apenas PT1M é válido</span><span class="sxs-lookup"><span data-stu-id="7c912-238">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-239">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-239">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-240">Alterações aos cmdlets LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="7c912-240">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="7c912-241">LoadBalancerInboundNatPoolConfig: parâmetros IdleTimeoutInMinutes, EnableFloatingIp e EnableTcpReset adicionados</span><span class="sxs-lookup"><span data-stu-id="7c912-241">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="7c912-242">LoadBalancerInboundNatRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-242">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="7c912-243">LoadBalancerRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-243">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="7c912-244">LoadBalancerProbeConfig: suporte para o valor "Https" para o parâmetro Protocol adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-244">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="7c912-245">Adicionados comandos novos para o sub-recurso OutboundRule de LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="7c912-245">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="7c912-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="7c912-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="7c912-248">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-248">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="7c912-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="7c912-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="7c912-251">Adicionada propriedade HostedWorkloads nova para PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="7c912-251">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="7c912-252">Adicionados cmdlets novos para a funcionalidade: Azure Firewall através de ARM</span><span class="sxs-lookup"><span data-stu-id="7c912-252">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="7c912-253">Get-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-253">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="7c912-254">Set-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-254">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="7c912-255">New-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-255">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="7c912-256">Remove-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-256">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="7c912-257">New-AzureRmFirewallApplicationRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-257">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="7c912-258">New-AzureRmFirewallApplicationRule adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-258">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="7c912-259">New-AzureRmFirewallNatRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-259">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="7c912-260">New-AzureRmFirewallNatRule adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-260">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="7c912-261">New-AzureRmFirewallNetworkRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-261">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="7c912-262">New-AzureRmFirewallNetworkRule adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-262">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="7c912-263">Adicionado suporte para o certificado de raiz fidedigna e configuração de dimensionamento automático no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="7c912-263">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="7c912-264">Novos cmdlets adicionados:</span><span class="sxs-lookup"><span data-stu-id="7c912-264">New Cmdlets added:</span></span>
      - <span data-ttu-id="7c912-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="7c912-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="7c912-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="7c912-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="7c912-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="7c912-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="7c912-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="7c912-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="7c912-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="7c912-274">Cmdlets updated with optonal parameter -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-274">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="7c912-275">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="7c912-275">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="7c912-276">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="7c912-276">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="7c912-277">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="7c912-277">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="7c912-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="7c912-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="7c912-279">Cmdlets atualizados com parâmetro opcional -AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-279">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="7c912-280">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="7c912-280">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="7c912-281">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="7c912-281">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="7c912-282">Adicionado cmdlet para Ponto Final da Interface Get-AzureInterfaceEndpoint</span><span class="sxs-lookup"><span data-stu-id="7c912-282">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="7c912-283">Adicionado suporte para vários prefixos de endereços numa sub-rede.</span><span class="sxs-lookup"><span data-stu-id="7c912-283">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="7c912-284">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="7c912-284">Updated cmdlets:</span></span>
  - <span data-ttu-id="7c912-285">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-285">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="7c912-286">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-286">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="7c912-287">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-287">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="7c912-288">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-288">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="7c912-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="7c912-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="7c912-291">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-291">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="7c912-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="7c912-293">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-293">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="7c912-294">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-294">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="7c912-295">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-295">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="7c912-296">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-296">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="7c912-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="7c912-298">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-298">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="7c912-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="7c912-300">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-300">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="7c912-301">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-301">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="7c912-302">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-302">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="7c912-303">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="7c912-303">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="7c912-304">Adição de cmdlets para delegação de sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-304">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="7c912-305">New-AzureRmDelegation: cria uma delegação nova, que pode ser adicionada a uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-305">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="7c912-306">Remove-AzureRmDelegation: recebe uma sub-rede e remove o nome da delegação especificado dessa sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-306">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="7c912-307">Add-AzureRmDelegation: recebe uma sub-rede e adiciona o nome de serviço especificado como delegação a essa sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-307">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="7c912-308">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="7c912-308">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="7c912-309">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="7c912-309">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="7c912-310">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="7c912-310">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="7c912-311">Suporte para discos geridos</span><span class="sxs-lookup"><span data-stu-id="7c912-311">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="7c912-312">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7c912-312">AzureRM.RedisCache</span></span>
* <span data-ttu-id="7c912-313">Dependência de informações atualizada</span><span class="sxs-lookup"><span data-stu-id="7c912-313">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-314">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-314">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-315">New-AzureRmResourceGroupDeployment atualizado com parâmetro novo RollbackAction</span><span class="sxs-lookup"><span data-stu-id="7c912-315">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="7c912-316">Adicionado suporte para OnErrorDeployment com o parâmetro novo.</span><span class="sxs-lookup"><span data-stu-id="7c912-316">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="7c912-317">Suporte para identidades geridas nas atribuições de políticas.</span><span class="sxs-lookup"><span data-stu-id="7c912-317">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="7c912-318">Os parâmetros com valores predefinidos já não são necessários ao atribuir uma política com “New-AzureRmPolicyAssignment”</span><span class="sxs-lookup"><span data-stu-id="7c912-318">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="7c912-319">Adicionado cmdlet novo Get-AzureRmPolicyAlias para obter aliases de políticas</span><span class="sxs-lookup"><span data-stu-id="7c912-319">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-320">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-320">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-321">Problema n.º 7161 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-321">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="7c912-322">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="7c912-322">AzureRM.SignalR</span></span>
* <span data-ttu-id="7c912-323">Nomes dos SKUs atualizados para Free_F1 e Standard_S1</span><span class="sxs-lookup"><span data-stu-id="7c912-323">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="7c912-324">Adicionado campo de versão ao objeto PSSignalRResource e cadeia de ligação ao objeto PSSignalRKeys.</span><span class="sxs-lookup"><span data-stu-id="7c912-324">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="7c912-325">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-325">AzureRM.Storage</span></span>
* <span data-ttu-id="7c912-326">Suporte para política Imutabilidade em AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-326">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="7c912-327">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="7c912-327">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="7c912-328">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="7c912-328">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="7c912-329">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="7c912-329">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="7c912-330">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="7c912-330">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="7c912-331">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="7c912-331">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="7c912-332">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="7c912-332">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="7c912-333">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="7c912-333">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="7c912-334">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-334">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="7c912-335">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-335">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="7c912-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="7c912-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-338">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-338">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-339">Adicionados dois cmdlets novos: Get-AzureRmDeletedWebApp e Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="7c912-339">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="7c912-340">O comutador New-AzureRmAppServicePlan -HyperV é adicionado para criar o plano do serviço de aplicações com contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="7c912-340">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="7c912-341">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - parâmetros novos (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) adicionados para criar e gerir a aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="7c912-341">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="7c912-342">6.8.1 - Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-342">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7c912-343">Geral</span><span class="sxs-lookup"><span data-stu-id="7c912-343">General</span></span>
* <span data-ttu-id="7c912-344">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7c912-344">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="7c912-345">Assemblagens de runtime comum atualizadas</span><span class="sxs-lookup"><span data-stu-id="7c912-345">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7c912-346">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7c912-346">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7c912-347">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7c912-347">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="7c912-348">Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-348">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="7c912-349">Agora, os cmdlets Import-AzureRmApiManagementApi e \*-AzureRmApiManagementCertificate identificam caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="7c912-349">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="7c912-350">Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-350">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="7c912-351">O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="7c912-351">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="7c912-352">Corrigido com a atualização para 4.0.4-nuget de pré-visualização</span><span class="sxs-lookup"><span data-stu-id="7c912-352">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="7c912-353">Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-353">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="7c912-354">Foi corrigido o filtro de Odata para procurar por nome de produto</span><span class="sxs-lookup"><span data-stu-id="7c912-354">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="7c912-355">Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-355">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="7c912-356">Foi corrigido o filtro de Odata para procurar por nome na API</span><span class="sxs-lookup"><span data-stu-id="7c912-356">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="7c912-357">Foi adicionado suporte para o logger de AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="7c912-357">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="7c912-358">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-358">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-359">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="7c912-359">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="7c912-360">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="7c912-360">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="7c912-361">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7c912-361">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="7c912-362">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="7c912-362">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-363">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-363">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-364">Representação de saída de cmdlet predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="7c912-364">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="7c912-365">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7c912-365">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="7c912-366">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="7c912-366">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="7c912-367">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-367">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-368">Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7c912-368">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-369">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-369">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-370">Problemas corrigidos</span><span class="sxs-lookup"><span data-stu-id="7c912-370">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7c912-371">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7c912-371">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7c912-372">Suporte adicionado para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="7c912-372">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="7c912-373">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="7c912-373">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="7c912-374">Suporte adicionado para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-374">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="7c912-375">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="7c912-375">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="7c912-376">Suporte adicionado para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7c912-376">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="7c912-377">Suporte adicionado para intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7c912-377">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="7c912-378">Suporte adicionado para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="7c912-378">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="7c912-379">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-379">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7c912-380">Geral</span><span class="sxs-lookup"><span data-stu-id="7c912-380">General</span></span>
* <span data-ttu-id="7c912-381">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7c912-381">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7c912-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-382">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-383">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="7c912-383">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-384">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-384">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-385">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="7c912-385">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="7c912-386">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="7c912-386">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="7c912-387">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="7c912-387">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="7c912-388">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="7c912-388">AzureRM.IotHub</span></span>
* <span data-ttu-id="7c912-389">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="7c912-389">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-390">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-390">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-391">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="7c912-391">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="7c912-392">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7c912-392">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="7c912-393">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="7c912-393">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-394">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-394">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-395">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7c912-395">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-396">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-396">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-397">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="7c912-397">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7c912-398">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7c912-398">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7c912-399">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="7c912-399">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="7c912-400">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="7c912-400">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="7c912-401">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="7c912-401">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="7c912-402">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="7c912-402">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="7c912-403">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7c912-403">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="7c912-404">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7c912-404">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="7c912-405">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="7c912-405">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-406">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-406">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-407">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="7c912-407">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="7c912-408">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-408">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-409">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-409">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-410">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7c912-411">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="7c912-411">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="7c912-412">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="7c912-412">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="7c912-413">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="7c912-413">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="7c912-414">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-414">Azure.Storage</span></span>
* <span data-ttu-id="7c912-415">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="7c912-415">Remove the 5TB limitation for Azure File Share quota</span></span>
* <span data-ttu-id="7c912-416">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="7c912-416">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="7c912-417">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7c912-417">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="7c912-418">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-418">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="7c912-419">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7c912-419">Azure.AnalysisServices</span></span>
* <span data-ttu-id="7c912-420">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-420">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7c912-421">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7c912-421">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7c912-422">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-422">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="7c912-423">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="7c912-423">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="7c912-424">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-424">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="7c912-425">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="7c912-425">AzureRM.Automation</span></span>
* <span data-ttu-id="7c912-426">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-426">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="7c912-427">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="7c912-427">AzureRM.Backup</span></span>
* <span data-ttu-id="7c912-428">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-428">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="7c912-429">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="7c912-429">AzureRM.Batch</span></span>
* <span data-ttu-id="7c912-430">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-430">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="7c912-431">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="7c912-431">AzureRM.Billing</span></span>
* <span data-ttu-id="7c912-432">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-432">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="7c912-433">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="7c912-433">AzureRM.Cdn</span></span>
* <span data-ttu-id="7c912-434">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-434">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="7c912-435">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7c912-435">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="7c912-436">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-436">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-437">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-437">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-438">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-438">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7c912-439">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-439">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="7c912-440">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="7c912-440">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="7c912-441">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="7c912-441">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="7c912-442">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="7c912-442">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="7c912-443">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="7c912-443">AzureRM.Consumption</span></span>
* <span data-ttu-id="7c912-444">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-444">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="7c912-445">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7c912-445">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="7c912-446">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-446">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="7c912-447">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="7c912-447">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="7c912-448">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="7c912-449">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="7c912-449">AzureRM.DataFactories</span></span>
* <span data-ttu-id="7c912-450">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7c912-451">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7c912-451">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7c912-452">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="7c912-453">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7c912-453">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="7c912-454">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7c912-455">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c912-455">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c912-456">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="7c912-456">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="7c912-457">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="7c912-457">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="7c912-458">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-458">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7c912-459">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7c912-459">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="7c912-460">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="7c912-460">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="7c912-461">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-461">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="7c912-462">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="7c912-462">AzureRM.Dns</span></span>
* <span data-ttu-id="7c912-463">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-463">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="7c912-464">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7c912-464">AzureRM.EventGrid</span></span>
* <span data-ttu-id="7c912-465">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-465">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7c912-466">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7c912-466">AzureRM.EventHub</span></span>
* <span data-ttu-id="7c912-467">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-467">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="7c912-468">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7c912-468">AzureRM.HDInsight</span></span>
* <span data-ttu-id="7c912-469">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-469">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="7c912-470">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7c912-470">AzureRM.Insights</span></span>
* <span data-ttu-id="7c912-471">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-471">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="7c912-472">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="7c912-472">AzureRM.IotHub</span></span>
* <span data-ttu-id="7c912-473">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-473">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7c912-474">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c912-474">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c912-475">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-475">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="7c912-476">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7c912-476">AzureRM.LogicApp</span></span>
* <span data-ttu-id="7c912-477">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-477">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="7c912-478">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7c912-478">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="7c912-479">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-479">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="7c912-480">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="7c912-480">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="7c912-481">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-481">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="7c912-482">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="7c912-482">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="7c912-483">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="7c912-484">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="7c912-484">AzureRM.Media</span></span>
* <span data-ttu-id="7c912-485">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-486">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-486">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-487">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="7c912-487">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="7c912-488">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="7c912-488">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="7c912-489">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="7c912-489">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="7c912-490">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="7c912-490">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="7c912-491">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="7c912-491">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="7c912-492">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="7c912-492">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="7c912-493">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="7c912-493">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="7c912-494">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="7c912-494">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="7c912-495">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="7c912-495">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="7c912-496">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-496">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="7c912-497">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7c912-497">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="7c912-498">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-498">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="7c912-499">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7c912-499">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="7c912-500">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-500">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="7c912-501">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7c912-501">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="7c912-502">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-502">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="7c912-503">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7c912-503">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="7c912-504">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-504">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7c912-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7c912-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7c912-506">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="7c912-506">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="7c912-507">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="7c912-507">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="7c912-508">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="7c912-508">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="7c912-509">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-509">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7c912-510">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="7c912-510">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="7c912-511">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="7c912-511">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="7c912-512">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="7c912-512">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="7c912-513">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="7c912-513">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="7c912-514">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-514">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="7c912-515">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7c912-515">AzureRM.RedisCache</span></span>
* <span data-ttu-id="7c912-516">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-516">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="7c912-517">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="7c912-517">AzureRM.Relay</span></span>
* <span data-ttu-id="7c912-518">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-518">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-519">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-519">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-520">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="7c912-520">Support template deployment at subscription scope.</span></span> <span data-ttu-id="7c912-521">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7c912-521">Add new Cmdlets:</span></span>
    - <span data-ttu-id="7c912-522">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-522">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="7c912-523">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-523">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="7c912-524">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-524">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="7c912-525">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-525">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="7c912-526">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-526">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="7c912-527">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="7c912-527">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="7c912-528">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="7c912-528">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="7c912-529">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="7c912-529">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="7c912-530">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-530">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="7c912-531">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-531">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="7c912-532">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="7c912-532">AzureRM.Scheduler</span></span>
* <span data-ttu-id="7c912-533">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-533">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-534">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-534">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-535">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-535">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7c912-536">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7c912-536">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7c912-537">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-537">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7c912-538">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-538">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-539">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-539">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="7c912-540">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-540">AzureRM.Storage</span></span>
* <span data-ttu-id="7c912-541">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-541">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="7c912-542">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="7c912-542">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="7c912-543">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-543">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="7c912-544">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="7c912-544">AzureRM.Tags</span></span>
* <span data-ttu-id="7c912-545">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-545">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7c912-546">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7c912-546">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7c912-547">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-547">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="7c912-548">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="7c912-548">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="7c912-549">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-549">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-550">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-550">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-551">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-551">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="7c912-552">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-552">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7c912-553">Geral</span><span class="sxs-lookup"><span data-stu-id="7c912-553">General</span></span>
* <span data-ttu-id="7c912-554">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="7c912-554">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7c912-555">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-555">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-556">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="7c912-556">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="7c912-557">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-557">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="7c912-558">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-558">Azure.Storage</span></span>
* <span data-ttu-id="7c912-559">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="7c912-559">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="7c912-560">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7c912-560">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7c912-561">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7c912-561">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7c912-562">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-562">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="7c912-563">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="7c912-563">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="7c912-564">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-564">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="7c912-565">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="7c912-565">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="7c912-566">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="7c912-566">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="7c912-567">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="7c912-567">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-568">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-568">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-569">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="7c912-569">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="7c912-570">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="7c912-570">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="7c912-571">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="7c912-571">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="7c912-572">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="7c912-572">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="7c912-573">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="7c912-573">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="7c912-574">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="7c912-574">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="7c912-575">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="7c912-575">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="7c912-576">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="7c912-576">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="7c912-577">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="7c912-577">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="7c912-578">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="7c912-578">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7c912-579">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7c912-579">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7c912-580">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="7c912-580">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="7c912-581">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="7c912-581">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="7c912-582">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-582">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="7c912-583">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="7c912-583">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7c912-584">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c912-584">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c912-585">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="7c912-585">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7c912-586">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7c912-586">AzureRM.EventHub</span></span>
* <span data-ttu-id="7c912-587">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="7c912-587">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="7c912-588">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7c912-588">AzureRM.Insights</span></span>
* <span data-ttu-id="7c912-589">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="7c912-589">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="7c912-590">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="7c912-590">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7c912-591">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c912-591">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c912-592">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-592">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-593">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-594">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="7c912-594">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-595">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-595">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-596">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="7c912-596">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="7c912-597">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="7c912-597">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-598">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-598">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-599">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="7c912-599">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="7c912-600">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="7c912-600">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="7c912-601">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-601">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-602">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7c912-602">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="7c912-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="7c912-604">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7c912-604">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="7c912-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="7c912-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="7c912-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="7c912-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="7c912-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="7c912-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="7c912-608">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="7c912-608">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="7c912-609">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="7c912-609">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="7c912-610">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-610">AzureRM.Storage</span></span>
* <span data-ttu-id="7c912-611">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="7c912-611">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="7c912-612">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="7c912-612">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="7c912-613">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7c912-613">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="7c912-614">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7c912-614">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="7c912-615">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7c912-615">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="7c912-616">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="7c912-616">AzureRM.Tags</span></span>
* <span data-ttu-id="7c912-617">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="7c912-617">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="7c912-618">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-618">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-619">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-619">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-620">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="7c912-620">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="7c912-621">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-621">Azure.Storage</span></span>
* <span data-ttu-id="7c912-622">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="7c912-622">Support Upload Blob or File with write only Sas token</span></span>
* <span data-ttu-id="7c912-623">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7c912-623">Set-AzureStorageBlobContent</span></span>
* <span data-ttu-id="7c912-624">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="7c912-624">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="7c912-625">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7c912-625">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="7c912-626">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="7c912-626">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="7c912-627">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="7c912-627">AzureRM.Automation</span></span>
* <span data-ttu-id="7c912-628">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="7c912-628">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-629">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-629">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-630">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="7c912-630">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="7c912-631">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="7c912-631">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="7c912-632">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="7c912-632">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="7c912-633">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="7c912-633">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="7c912-634">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="7c912-634">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7c912-635">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7c912-635">AzureRM.EventHub</span></span>
* <span data-ttu-id="7c912-636">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="7c912-636">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7c912-637">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c912-637">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c912-638">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7c912-638">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="7c912-639">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7c912-639">AzureRM.LogicApp</span></span>
* <span data-ttu-id="7c912-640">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="7c912-640">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-641">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-641">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-642">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="7c912-642">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="7c912-643">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="7c912-643">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="7c912-644">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="7c912-644">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="7c912-645">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="7c912-645">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="7c912-646">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="7c912-646">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="7c912-647">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="7c912-647">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="7c912-648">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="7c912-648">AzureRM.Relay</span></span>
* <span data-ttu-id="7c912-649">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="7c912-649">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-650">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-650">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-651">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="7c912-651">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="7c912-652">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="7c912-652">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="7c912-653">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7c912-653">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="7c912-654">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="7c912-654">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="7c912-655">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7c912-655">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-656">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-656">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-657">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="7c912-657">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="7c912-658">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="7c912-658">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="7c912-659">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7c912-659">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7c912-660">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7c912-660">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7c912-661">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7c912-661">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7c912-662">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7c912-662">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7c912-663">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7c912-663">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="7c912-664">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="7c912-664">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7c912-665">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7c912-665">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7c912-666">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="7c912-666">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7c912-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-667">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-668">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="7c912-668">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="7c912-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="7c912-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-671">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-671">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-672">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="7c912-672">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="7c912-673">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="7c912-673">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="7c912-674">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="7c912-674">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="7c912-675">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-675">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7c912-676">Geral</span><span class="sxs-lookup"><span data-stu-id="7c912-676">General</span></span>
* <span data-ttu-id="7c912-677">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="7c912-677">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7c912-678">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-678">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-679">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="7c912-679">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-680">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-680">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-681">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="7c912-681">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="7c912-682">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="7c912-682">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="7c912-683">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-683">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="7c912-684">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="7c912-684">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="7c912-685">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-685">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="7c912-686">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="7c912-686">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="7c912-687">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-687">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="7c912-688">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7c912-688">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="7c912-689">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7c912-689">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="7c912-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7c912-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="7c912-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7c912-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="7c912-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7c912-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7c912-693">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c912-693">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c912-694">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="7c912-694">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="7c912-695">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="7c912-695">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="7c912-696">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="7c912-696">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="7c912-697">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="7c912-697">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7c912-698">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7c912-698">AzureRM.EventHub</span></span>
* <span data-ttu-id="7c912-699">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="7c912-699">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="7c912-700">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="7c912-700">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="7c912-701">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="7c912-701">Provided Default Parameter set.</span></span>
* <span data-ttu-id="7c912-702">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="7c912-702">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7c912-703">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c912-703">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c912-704">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="7c912-704">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-705">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-705">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-706">Apresentação de novos SKUs para VirtualNetworkGateways com redundância entre zonas</span><span class="sxs-lookup"><span data-stu-id="7c912-706">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="7c912-707">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="7c912-707">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="7c912-708">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="7c912-708">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="7c912-709">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="7c912-709">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="7c912-710">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="7c912-710">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="7c912-711">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="7c912-711">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="7c912-712">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="7c912-712">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="7c912-713">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="7c912-713">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="7c912-714">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="7c912-714">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="7c912-715">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7c912-715">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7c912-716">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7c912-716">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7c912-717">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="7c912-717">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="7c912-718">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="7c912-718">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="7c912-719">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="7c912-719">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-720">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-720">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-721">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="7c912-721">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="7c912-722">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7c912-722">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="7c912-723">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7c912-723">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="7c912-724">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="7c912-724">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="7c912-725">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="7c912-725">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="7c912-726">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7c912-726">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="7c912-727">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="7c912-727">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="7c912-728">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="7c912-728">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="7c912-729">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7c912-729">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="7c912-730">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="7c912-730">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="7c912-731">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="7c912-731">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="7c912-732">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="7c912-732">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="7c912-733">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="7c912-733">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="7c912-734">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7c912-734">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7c912-735">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="7c912-735">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7c912-736">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-736">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-737">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="7c912-737">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="7c912-738">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="7c912-738">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="7c912-739">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-739">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-740">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-740">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-741">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="7c912-741">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="7c912-742">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="7c912-742">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="7c912-743">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c912-743">Azure.Storage</span></span>
* <span data-ttu-id="7c912-744">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="7c912-744">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-745">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-745">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-746">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="7c912-746">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="7c912-747">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="7c912-747">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="7c912-748">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="7c912-748">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="7c912-749">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="7c912-749">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="7c912-750">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="7c912-750">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="7c912-751">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="7c912-751">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="7c912-752">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7c912-752">Start-AzureRmVM</span></span>
    - <span data-ttu-id="7c912-753">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7c912-753">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="7c912-754">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7c912-754">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="7c912-755">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7c912-755">Set-AzureRmVM</span></span>
    - <span data-ttu-id="7c912-756">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="7c912-756">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="7c912-757">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-757">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="7c912-758">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="7c912-758">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="7c912-759">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="7c912-759">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="7c912-760">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-760">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="7c912-761">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-761">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="7c912-762">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-762">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="7c912-763">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7c912-763">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="7c912-764">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="7c912-764">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="7c912-765">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="7c912-765">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="7c912-766">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="7c912-766">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="7c912-767">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="7c912-767">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="7c912-768">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="7c912-768">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="7c912-769">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="7c912-769">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="7c912-770">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="7c912-770">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="7c912-771">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7c912-771">AzureRM.EventGrid</span></span>
* <span data-ttu-id="7c912-772">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="7c912-772">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7c912-773">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c912-773">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c912-774">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="7c912-774">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="7c912-775">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7c912-775">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="7c912-776">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="7c912-776">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="7c912-777">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="7c912-777">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="7c912-778">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="7c912-778">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7c912-779">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7c912-779">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7c912-780">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="7c912-780">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="7c912-781">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="7c912-781">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7c912-782">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-782">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-783">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="7c912-783">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7c912-784">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7c912-784">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7c912-785">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-785">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-786">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-786">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-787">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="7c912-787">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="7c912-788">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="7c912-788">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="7c912-789">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-789">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="7c912-790">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7c912-790">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="7c912-791">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="7c912-791">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="7c912-792">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-792">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-793">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-793">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-794">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="7c912-794">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7c912-795">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c912-795">AzureRM.Compute</span></span>
* <span data-ttu-id="7c912-796">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="7c912-796">VMSS VM Update feature</span></span>
    - <span data-ttu-id="7c912-797">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="7c912-797">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="7c912-798">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="7c912-798">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7c912-799">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7c912-799">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7c912-800">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="7c912-800">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="7c912-801">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="7c912-801">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="7c912-802">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="7c912-802">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="7c912-803">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="7c912-803">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="7c912-804">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="7c912-804">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="7c912-805">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c912-805">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c912-806">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="7c912-806">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="7c912-807">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-807">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-808">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="7c912-808">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7c912-809">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c912-809">AzureRM.Resources</span></span>
* <span data-ttu-id="7c912-810">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="7c912-810">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="7c912-811">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="7c912-811">AzureRM.Scheduler</span></span>
* <span data-ttu-id="7c912-812">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="7c912-812">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="7c912-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-813">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-814">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="7c912-814">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="7c912-815">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7c912-815">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="7c912-816">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="7c912-816">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="7c912-817">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="7c912-817">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="7c912-818">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="7c912-818">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="7c912-819">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7c912-819">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7c912-820">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c912-820">AzureRM.Websites</span></span>
* <span data-ttu-id="7c912-821">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="7c912-821">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="7c912-822">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="7c912-822">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7c912-823">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c912-823">AzureRM.Profile</span></span>
* <span data-ttu-id="7c912-824">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="7c912-824">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="7c912-825">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7c912-825">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="7c912-826">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="7c912-826">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7c912-827">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7c912-827">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7c912-828">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="7c912-828">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="7c912-829">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7c912-829">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="7c912-830">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="7c912-830">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="7c912-831">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="7c912-831">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="7c912-832">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="7c912-832">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="7c912-833">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="7c912-833">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="7c912-834">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="7c912-834">Added support for MSI identity</span></span>
* <span data-ttu-id="7c912-835">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="7c912-835">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="7c912-836">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="7c912-836">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="7c912-837">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-837">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="7c912-838">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="7c912-838">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="7c912-839">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="7c912-839">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="7c912-840">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="7c912-840">AzureRM.Batch</span></span>
* <span data-ttu-id="7c912-841">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="7c912-841">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="7c912-842">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="7c912-842">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="7c912-843">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="7c912-843">AzureRM.Consumption</span></span>
* <span data-ttu-id="7c912-844">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="7c912-844">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7c912-845">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c912-845">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c912-846">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="7c912-846">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="7c912-847">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7c912-847">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="7c912-848">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7c912-848">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="7c912-849">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c912-849">AzureRM.Network</span></span>
* <span data-ttu-id="7c912-850">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="7c912-850">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="7c912-851">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="7c912-851">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="7c912-852">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c912-852">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="7c912-853">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7c912-853">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="7c912-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="7c912-855">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7c912-855">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="7c912-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="7c912-857">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="7c912-857">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="7c912-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="7c912-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7c912-859">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7c912-859">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7c912-860">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="7c912-860">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7c912-861">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7c912-861">AzureRM.Sql</span></span>
* <span data-ttu-id="7c912-862">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="7c912-862">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="7c912-863">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="7c912-863">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="7c912-864">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="7c912-864">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="7c912-865">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="7c912-865">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="7c912-866">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="7c912-866">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="7c912-867">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7c912-867">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="7c912-868">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="7c912-868">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="7c912-869">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="7c912-869">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="7c912-870">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="7c912-870">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="7c912-871">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7c912-871">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7c912-872">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7c912-872">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7c912-873">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="7c912-873">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
