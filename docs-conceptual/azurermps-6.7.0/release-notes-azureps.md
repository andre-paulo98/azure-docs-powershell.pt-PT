---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 2a6e20137f12ae9317c7eeed330a2433774e1ea9
ms.sourcegitcommit: f648ac92fafb16cc0e9ca6bc85d00fa327baf396
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/28/2018
ms.locfileid: "43018534"
---
# <a name="release-notes"></a><span data-ttu-id="d06fc-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="d06fc-103">Release notes</span></span>

<span data-ttu-id="d06fc-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="d06fc-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="670---august-2018"></a><span data-ttu-id="d06fc-105">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-105">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-106">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-107">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-107">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d06fc-108">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="d06fc-108">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="d06fc-109">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="d06fc-109">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="d06fc-110">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="d06fc-110">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="d06fc-111">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-111">Azure.Storage</span></span>
* <span data-ttu-id="d06fc-112">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="d06fc-112">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="d06fc-113">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="d06fc-113">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="d06fc-114">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d06fc-114">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="d06fc-115">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-115">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="d06fc-116">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d06fc-116">Azure.AnalysisServices</span></span>
* <span data-ttu-id="d06fc-117">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-117">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d06fc-118">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d06fc-118">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d06fc-119">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-119">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="d06fc-120">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="d06fc-120">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="d06fc-121">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-121">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="d06fc-122">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="d06fc-122">AzureRM.Automation</span></span>
* <span data-ttu-id="d06fc-123">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-123">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="d06fc-124">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="d06fc-124">AzureRM.Backup</span></span>
* <span data-ttu-id="d06fc-125">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-125">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="d06fc-126">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="d06fc-126">AzureRM.Batch</span></span>
* <span data-ttu-id="d06fc-127">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-127">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="d06fc-128">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="d06fc-128">AzureRM.Billing</span></span>
* <span data-ttu-id="d06fc-129">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-129">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="d06fc-130">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="d06fc-130">AzureRM.Cdn</span></span>
* <span data-ttu-id="d06fc-131">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-131">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="d06fc-132">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d06fc-132">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="d06fc-133">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-133">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d06fc-134">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d06fc-134">AzureRM.Compute</span></span>
* <span data-ttu-id="d06fc-135">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-135">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d06fc-136">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="d06fc-136">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="d06fc-137">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="d06fc-137">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="d06fc-138">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="d06fc-138">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="d06fc-139">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="d06fc-139">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="d06fc-140">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="d06fc-140">AzureRM.Consumption</span></span>
* <span data-ttu-id="d06fc-141">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-141">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="d06fc-142">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d06fc-142">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="d06fc-143">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-143">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="d06fc-144">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d06fc-144">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="d06fc-145">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-145">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="d06fc-146">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="d06fc-146">AzureRM.DataFactories</span></span>
* <span data-ttu-id="d06fc-147">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-147">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d06fc-148">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d06fc-148">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d06fc-149">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-149">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="d06fc-150">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d06fc-150">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="d06fc-151">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-151">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d06fc-152">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d06fc-152">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d06fc-153">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="d06fc-153">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="d06fc-154">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="d06fc-154">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="d06fc-155">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-155">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d06fc-156">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d06fc-156">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="d06fc-157">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="d06fc-157">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="d06fc-158">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="d06fc-159">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="d06fc-159">AzureRM.Dns</span></span>
* <span data-ttu-id="d06fc-160">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="d06fc-161">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d06fc-161">AzureRM.EventGrid</span></span>
* <span data-ttu-id="d06fc-162">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d06fc-163">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d06fc-163">AzureRM.EventHub</span></span>
* <span data-ttu-id="d06fc-164">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-164">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="d06fc-165">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d06fc-165">AzureRM.HDInsight</span></span>
* <span data-ttu-id="d06fc-166">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-166">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="d06fc-167">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d06fc-167">AzureRM.Insights</span></span>
* <span data-ttu-id="d06fc-168">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-168">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="d06fc-169">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="d06fc-169">AzureRM.IotHub</span></span>
* <span data-ttu-id="d06fc-170">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d06fc-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d06fc-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d06fc-172">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="d06fc-173">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d06fc-173">AzureRM.LogicApp</span></span>
* <span data-ttu-id="d06fc-174">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="d06fc-175">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d06fc-175">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="d06fc-176">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="d06fc-177">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="d06fc-177">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="d06fc-178">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="d06fc-179">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="d06fc-179">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="d06fc-180">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="d06fc-181">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="d06fc-181">AzureRM.Media</span></span>
* <span data-ttu-id="d06fc-182">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-182">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d06fc-183">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d06fc-183">AzureRM.Network</span></span>
* <span data-ttu-id="d06fc-184">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="d06fc-184">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="d06fc-185">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="d06fc-185">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="d06fc-186">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="d06fc-186">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="d06fc-187">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="d06fc-187">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="d06fc-188">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="d06fc-188">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="d06fc-189">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="d06fc-189">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="d06fc-190">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="d06fc-190">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="d06fc-191">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="d06fc-191">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="d06fc-192">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="d06fc-192">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="d06fc-193">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="d06fc-194">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d06fc-194">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="d06fc-195">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="d06fc-196">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d06fc-196">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="d06fc-197">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="d06fc-198">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="d06fc-198">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="d06fc-199">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="d06fc-200">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d06fc-200">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="d06fc-201">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="d06fc-202">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d06fc-202">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d06fc-203">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="d06fc-203">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="d06fc-204">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="d06fc-204">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="d06fc-205">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="d06fc-205">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="d06fc-206">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-206">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d06fc-207">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="d06fc-207">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="d06fc-208">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="d06fc-208">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="d06fc-209">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="d06fc-209">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="d06fc-210">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="d06fc-210">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="d06fc-211">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="d06fc-212">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d06fc-212">AzureRM.RedisCache</span></span>
* <span data-ttu-id="d06fc-213">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="d06fc-214">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="d06fc-214">AzureRM.Relay</span></span>
* <span data-ttu-id="d06fc-215">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d06fc-216">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d06fc-216">AzureRM.Resources</span></span>
* <span data-ttu-id="d06fc-217">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="d06fc-217">Support template deployment at subscription scope.</span></span> <span data-ttu-id="d06fc-218">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d06fc-218">Add new Cmdlets:</span></span>
    - <span data-ttu-id="d06fc-219">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-219">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="d06fc-220">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-220">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="d06fc-221">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-221">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="d06fc-222">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-222">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="d06fc-223">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-223">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="d06fc-224">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="d06fc-224">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="d06fc-225">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="d06fc-225">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="d06fc-226">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="d06fc-226">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="d06fc-227">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-227">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="d06fc-228">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="d06fc-229">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="d06fc-229">AzureRM.Scheduler</span></span>
* <span data-ttu-id="d06fc-230">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d06fc-231">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d06fc-231">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d06fc-232">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="d06fc-233">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d06fc-233">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="d06fc-234">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d06fc-235">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-235">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-236">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="d06fc-237">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-237">AzureRM.Storage</span></span>
* <span data-ttu-id="d06fc-238">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="d06fc-239">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="d06fc-239">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="d06fc-240">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="d06fc-241">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="d06fc-241">AzureRM.Tags</span></span>
* <span data-ttu-id="d06fc-242">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d06fc-243">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d06fc-243">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d06fc-244">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="d06fc-245">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="d06fc-245">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="d06fc-246">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d06fc-247">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d06fc-247">AzureRM.Websites</span></span>
* <span data-ttu-id="d06fc-248">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="d06fc-249">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-249">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d06fc-250">Geral</span><span class="sxs-lookup"><span data-stu-id="d06fc-250">General</span></span>
* <span data-ttu-id="d06fc-251">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="d06fc-251">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-252">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-252">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-253">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="d06fc-253">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="d06fc-254">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-254">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="d06fc-255">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-255">Azure.Storage</span></span>
* <span data-ttu-id="d06fc-256">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="d06fc-256">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="d06fc-257">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d06fc-257">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d06fc-258">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d06fc-258">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d06fc-259">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="d06fc-259">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="d06fc-260">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="d06fc-260">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="d06fc-261">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="d06fc-261">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="d06fc-262">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="d06fc-262">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="d06fc-263">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="d06fc-263">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="d06fc-264">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="d06fc-264">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d06fc-265">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d06fc-265">AzureRM.Compute</span></span>
* <span data-ttu-id="d06fc-266">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="d06fc-266">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="d06fc-267">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="d06fc-267">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="d06fc-268">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="d06fc-268">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="d06fc-269">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="d06fc-269">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="d06fc-270">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="d06fc-270">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="d06fc-271">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="d06fc-271">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="d06fc-272">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="d06fc-272">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="d06fc-273">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="d06fc-273">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="d06fc-274">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="d06fc-274">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="d06fc-275">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="d06fc-275">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d06fc-276">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d06fc-276">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d06fc-277">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="d06fc-277">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="d06fc-278">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="d06fc-278">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="d06fc-279">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-279">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="d06fc-280">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="d06fc-280">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d06fc-281">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d06fc-281">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d06fc-282">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="d06fc-282">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d06fc-283">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d06fc-283">AzureRM.EventHub</span></span>
* <span data-ttu-id="d06fc-284">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="d06fc-284">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="d06fc-285">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d06fc-285">AzureRM.Insights</span></span>
* <span data-ttu-id="d06fc-286">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="d06fc-286">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="d06fc-287">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="d06fc-287">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d06fc-288">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d06fc-288">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d06fc-289">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d06fc-289">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d06fc-290">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d06fc-290">AzureRM.Network</span></span>
* <span data-ttu-id="d06fc-291">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="d06fc-291">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d06fc-292">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d06fc-292">AzureRM.Resources</span></span>
* <span data-ttu-id="d06fc-293">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="d06fc-293">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="d06fc-294">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="d06fc-294">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d06fc-295">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d06fc-295">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d06fc-296">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="d06fc-296">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="d06fc-297">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="d06fc-297">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="d06fc-298">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-298">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-299">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d06fc-299">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="d06fc-300">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d06fc-300">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="d06fc-301">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d06fc-301">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="d06fc-302">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="d06fc-302">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="d06fc-303">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="d06fc-303">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="d06fc-304">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="d06fc-304">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="d06fc-305">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="d06fc-305">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="d06fc-306">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="d06fc-306">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="d06fc-307">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-307">AzureRM.Storage</span></span>
* <span data-ttu-id="d06fc-308">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="d06fc-308">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="d06fc-309">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="d06fc-309">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="d06fc-310">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d06fc-310">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="d06fc-311">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d06fc-311">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="d06fc-312">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d06fc-312">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="d06fc-313">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="d06fc-313">AzureRM.Tags</span></span>
* <span data-ttu-id="d06fc-314">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="d06fc-314">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="d06fc-315">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-315">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-316">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-316">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-317">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="d06fc-317">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="d06fc-318">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-318">Azure.Storage</span></span>
* <span data-ttu-id="d06fc-319">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="d06fc-319">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="d06fc-320">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="d06fc-320">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="d06fc-321">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="d06fc-321">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="d06fc-322">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d06fc-322">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="d06fc-323">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="d06fc-323">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="d06fc-324">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="d06fc-324">AzureRM.Automation</span></span>
* <span data-ttu-id="d06fc-325">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="d06fc-325">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d06fc-326">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d06fc-326">AzureRM.Compute</span></span>
* <span data-ttu-id="d06fc-327">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="d06fc-327">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="d06fc-328">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="d06fc-328">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="d06fc-329">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="d06fc-329">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="d06fc-330">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="d06fc-330">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="d06fc-331">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="d06fc-331">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d06fc-332">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d06fc-332">AzureRM.EventHub</span></span>
* <span data-ttu-id="d06fc-333">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="d06fc-333">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d06fc-334">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d06fc-334">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d06fc-335">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d06fc-335">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="d06fc-336">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d06fc-336">AzureRM.LogicApp</span></span>
* <span data-ttu-id="d06fc-337">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="d06fc-337">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d06fc-338">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d06fc-338">AzureRM.Network</span></span>
* <span data-ttu-id="d06fc-339">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="d06fc-339">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="d06fc-340">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="d06fc-340">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="d06fc-341">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="d06fc-341">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="d06fc-342">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="d06fc-342">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="d06fc-343">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="d06fc-343">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="d06fc-344">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="d06fc-344">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="d06fc-345">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="d06fc-345">AzureRM.Relay</span></span>
* <span data-ttu-id="d06fc-346">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="d06fc-346">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d06fc-347">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d06fc-347">AzureRM.Resources</span></span>
* <span data-ttu-id="d06fc-348">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="d06fc-348">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="d06fc-349">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="d06fc-349">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="d06fc-350">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d06fc-350">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="d06fc-351">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="d06fc-351">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="d06fc-352">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d06fc-352">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d06fc-353">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d06fc-353">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d06fc-354">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="d06fc-354">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="d06fc-355">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="d06fc-355">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="d06fc-356">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d06fc-356">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d06fc-357">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d06fc-357">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d06fc-358">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d06fc-358">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d06fc-359">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d06fc-359">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d06fc-360">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d06fc-360">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="d06fc-361">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="d06fc-361">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="d06fc-362">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d06fc-362">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="d06fc-363">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="d06fc-363">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d06fc-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-364">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-365">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="d06fc-365">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="d06fc-366">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="d06fc-366">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="d06fc-367">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="d06fc-367">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d06fc-368">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d06fc-368">AzureRM.Websites</span></span>
* <span data-ttu-id="d06fc-369">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="d06fc-369">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="d06fc-370">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="d06fc-370">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="d06fc-371">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="d06fc-371">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="d06fc-372">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-372">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d06fc-373">Geral</span><span class="sxs-lookup"><span data-stu-id="d06fc-373">General</span></span>
* <span data-ttu-id="d06fc-374">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="d06fc-374">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-375">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-375">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-376">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="d06fc-376">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d06fc-377">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d06fc-377">AzureRM.Compute</span></span>
* <span data-ttu-id="d06fc-378">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="d06fc-378">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="d06fc-379">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="d06fc-379">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="d06fc-380">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="d06fc-380">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="d06fc-381">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="d06fc-381">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="d06fc-382">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-382">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="d06fc-383">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-383">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="d06fc-384">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-384">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="d06fc-385">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d06fc-385">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="d06fc-386">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d06fc-386">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="d06fc-387">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d06fc-387">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="d06fc-388">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d06fc-388">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="d06fc-389">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d06fc-389">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d06fc-390">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d06fc-390">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d06fc-391">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="d06fc-391">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="d06fc-392">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="d06fc-392">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="d06fc-393">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="d06fc-393">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="d06fc-394">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="d06fc-394">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d06fc-395">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d06fc-395">AzureRM.EventHub</span></span>
* <span data-ttu-id="d06fc-396">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="d06fc-396">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="d06fc-397">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="d06fc-397">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="d06fc-398">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="d06fc-398">Provided Default Parameter set.</span></span>
* <span data-ttu-id="d06fc-399">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="d06fc-399">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d06fc-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d06fc-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d06fc-401">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="d06fc-401">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d06fc-402">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d06fc-402">AzureRM.Network</span></span>
* <span data-ttu-id="d06fc-403">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="d06fc-403">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="d06fc-404">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="d06fc-404">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="d06fc-405">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="d06fc-405">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="d06fc-406">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="d06fc-406">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="d06fc-407">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="d06fc-407">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="d06fc-408">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="d06fc-408">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="d06fc-409">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="d06fc-409">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="d06fc-410">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="d06fc-410">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="d06fc-411">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="d06fc-411">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="d06fc-412">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="d06fc-412">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="d06fc-413">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d06fc-413">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d06fc-414">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="d06fc-414">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="d06fc-415">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="d06fc-415">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="d06fc-416">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="d06fc-416">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d06fc-417">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d06fc-417">AzureRM.Resources</span></span>
* <span data-ttu-id="d06fc-418">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="d06fc-418">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="d06fc-419">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="d06fc-419">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="d06fc-420">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="d06fc-420">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="d06fc-421">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="d06fc-421">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="d06fc-422">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="d06fc-422">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="d06fc-423">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="d06fc-423">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="d06fc-424">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="d06fc-424">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="d06fc-425">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="d06fc-425">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="d06fc-426">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="d06fc-426">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="d06fc-427">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="d06fc-427">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="d06fc-428">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="d06fc-428">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="d06fc-429">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="d06fc-429">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="d06fc-430">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="d06fc-430">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="d06fc-431">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d06fc-431">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d06fc-432">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="d06fc-432">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d06fc-433">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-433">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-434">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="d06fc-434">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="d06fc-435">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="d06fc-435">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="d06fc-436">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-436">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-437">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-437">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-438">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="d06fc-438">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="d06fc-439">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="d06fc-439">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="d06fc-440">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d06fc-440">Azure.Storage</span></span>
* <span data-ttu-id="d06fc-441">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="d06fc-441">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d06fc-442">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d06fc-442">AzureRM.Compute</span></span>
* <span data-ttu-id="d06fc-443">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="d06fc-443">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="d06fc-444">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="d06fc-444">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="d06fc-445">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="d06fc-445">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="d06fc-446">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="d06fc-446">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="d06fc-447">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="d06fc-447">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="d06fc-448">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="d06fc-448">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="d06fc-449">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d06fc-449">Start-AzureRmVM</span></span>
    - <span data-ttu-id="d06fc-450">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d06fc-450">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="d06fc-451">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d06fc-451">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="d06fc-452">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d06fc-452">Set-AzureRmVM</span></span>
    - <span data-ttu-id="d06fc-453">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="d06fc-453">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="d06fc-454">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-454">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="d06fc-455">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="d06fc-455">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="d06fc-456">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="d06fc-456">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="d06fc-457">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-457">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="d06fc-458">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-458">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="d06fc-459">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-459">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="d06fc-460">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d06fc-460">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="d06fc-461">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="d06fc-461">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="d06fc-462">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="d06fc-462">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="d06fc-463">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="d06fc-463">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="d06fc-464">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="d06fc-464">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="d06fc-465">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="d06fc-465">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="d06fc-466">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="d06fc-466">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="d06fc-467">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="d06fc-467">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="d06fc-468">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d06fc-468">AzureRM.EventGrid</span></span>
* <span data-ttu-id="d06fc-469">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="d06fc-469">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d06fc-470">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d06fc-470">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d06fc-471">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="d06fc-471">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="d06fc-472">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d06fc-472">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="d06fc-473">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="d06fc-473">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="d06fc-474">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="d06fc-474">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="d06fc-475">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="d06fc-475">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="d06fc-476">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d06fc-476">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d06fc-477">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="d06fc-477">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="d06fc-478">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="d06fc-478">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d06fc-479">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-479">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-480">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="d06fc-480">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d06fc-481">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d06fc-481">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d06fc-482">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="d06fc-482">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d06fc-483">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d06fc-483">AzureRM.Websites</span></span>
* <span data-ttu-id="d06fc-484">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="d06fc-484">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="d06fc-485">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="d06fc-485">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="d06fc-486">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-486">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="d06fc-487">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d06fc-487">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="d06fc-488">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="d06fc-488">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="d06fc-489">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-489">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-490">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-490">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-491">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="d06fc-491">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d06fc-492">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d06fc-492">AzureRM.Compute</span></span>
* <span data-ttu-id="d06fc-493">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="d06fc-493">VMSS VM Update feature</span></span>
    - <span data-ttu-id="d06fc-494">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="d06fc-494">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="d06fc-495">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="d06fc-495">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d06fc-496">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d06fc-496">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d06fc-497">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="d06fc-497">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="d06fc-498">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="d06fc-498">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="d06fc-499">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="d06fc-499">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="d06fc-500">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="d06fc-500">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="d06fc-501">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="d06fc-501">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="d06fc-502">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d06fc-502">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d06fc-503">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="d06fc-503">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="d06fc-504">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d06fc-504">AzureRM.Network</span></span>
* <span data-ttu-id="d06fc-505">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="d06fc-505">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d06fc-506">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d06fc-506">AzureRM.Resources</span></span>
* <span data-ttu-id="d06fc-507">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="d06fc-507">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="d06fc-508">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="d06fc-508">AzureRM.Scheduler</span></span>
* <span data-ttu-id="d06fc-509">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="d06fc-509">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="d06fc-510">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-510">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-511">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="d06fc-511">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="d06fc-512">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d06fc-512">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="d06fc-513">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="d06fc-513">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="d06fc-514">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="d06fc-514">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="d06fc-515">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="d06fc-515">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="d06fc-516">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d06fc-516">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d06fc-517">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d06fc-517">AzureRM.Websites</span></span>
* <span data-ttu-id="d06fc-518">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="d06fc-518">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="d06fc-519">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="d06fc-519">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d06fc-520">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d06fc-520">AzureRM.Profile</span></span>
* <span data-ttu-id="d06fc-521">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="d06fc-521">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="d06fc-522">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d06fc-522">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="d06fc-523">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="d06fc-523">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d06fc-524">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d06fc-524">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d06fc-525">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="d06fc-525">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="d06fc-526">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d06fc-526">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="d06fc-527">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="d06fc-527">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="d06fc-528">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="d06fc-528">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="d06fc-529">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="d06fc-529">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="d06fc-530">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="d06fc-530">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="d06fc-531">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="d06fc-531">Added support for MSI identity</span></span>
* <span data-ttu-id="d06fc-532">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="d06fc-532">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="d06fc-533">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="d06fc-533">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="d06fc-534">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="d06fc-534">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="d06fc-535">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="d06fc-535">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="d06fc-536">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="d06fc-536">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="d06fc-537">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="d06fc-537">AzureRM.Batch</span></span>
* <span data-ttu-id="d06fc-538">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="d06fc-538">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="d06fc-539">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="d06fc-539">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="d06fc-540">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="d06fc-540">AzureRM.Consumption</span></span>
* <span data-ttu-id="d06fc-541">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="d06fc-541">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d06fc-542">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d06fc-542">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d06fc-543">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="d06fc-543">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="d06fc-544">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d06fc-544">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="d06fc-545">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d06fc-545">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="d06fc-546">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d06fc-546">AzureRM.Network</span></span>
* <span data-ttu-id="d06fc-547">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="d06fc-547">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="d06fc-548">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="d06fc-548">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="d06fc-549">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="d06fc-549">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="d06fc-550">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="d06fc-550">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="d06fc-551">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="d06fc-551">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="d06fc-552">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="d06fc-552">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="d06fc-553">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="d06fc-553">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="d06fc-554">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="d06fc-554">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="d06fc-555">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="d06fc-555">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="d06fc-556">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d06fc-556">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="d06fc-557">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="d06fc-557">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d06fc-558">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d06fc-558">AzureRM.Sql</span></span>
* <span data-ttu-id="d06fc-559">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="d06fc-559">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="d06fc-560">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="d06fc-560">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="d06fc-561">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="d06fc-561">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="d06fc-562">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="d06fc-562">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="d06fc-563">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="d06fc-563">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="d06fc-564">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d06fc-564">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="d06fc-565">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="d06fc-565">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="d06fc-566">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="d06fc-566">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="d06fc-567">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="d06fc-567">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="d06fc-568">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d06fc-568">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d06fc-569">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d06fc-569">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d06fc-570">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="d06fc-570">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
