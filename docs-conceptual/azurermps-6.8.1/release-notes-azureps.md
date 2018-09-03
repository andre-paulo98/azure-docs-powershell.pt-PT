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
ms.openlocfilehash: 6043d17df1b5e91521bad31e65372c10ee6a5c6a
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250562"
---
# <a name="release-notes"></a><span data-ttu-id="eaf83-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="eaf83-103">Release notes</span></span>

<span data-ttu-id="eaf83-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="eaf83-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="680---august-2018"></a><span data-ttu-id="eaf83-105">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-105">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="eaf83-106">Geral</span><span class="sxs-lookup"><span data-stu-id="eaf83-106">General</span></span>
* <span data-ttu-id="eaf83-107">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="eaf83-107">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-108">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-109">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="eaf83-109">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-110">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-111">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="eaf83-111">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="eaf83-112">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="eaf83-112">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="eaf83-113">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="eaf83-113">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="eaf83-114">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="eaf83-114">AzureRM.IotHub</span></span>
* <span data-ttu-id="eaf83-115">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="eaf83-115">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-116">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-116">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-117">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="eaf83-117">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="eaf83-118">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="eaf83-118">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="eaf83-119">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="eaf83-119">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="eaf83-120">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="eaf83-120">AzureRM.Resources</span></span>
* <span data-ttu-id="eaf83-121">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="eaf83-121">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="eaf83-122">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="eaf83-122">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="eaf83-123">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="eaf83-123">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="eaf83-124">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="eaf83-124">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="eaf83-125">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="eaf83-125">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="eaf83-126">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="eaf83-126">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="eaf83-127">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="eaf83-127">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="eaf83-128">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="eaf83-128">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="eaf83-129">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="eaf83-129">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="eaf83-130">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="eaf83-130">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="eaf83-131">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="eaf83-131">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="eaf83-132">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="eaf83-132">AzureRM.Websites</span></span>
* <span data-ttu-id="eaf83-133">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="eaf83-133">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="eaf83-134">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-134">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-135">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-135">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-136">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-136">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="eaf83-137">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="eaf83-137">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="eaf83-138">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="eaf83-138">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="eaf83-139">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="eaf83-139">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="eaf83-140">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-140">Azure.Storage</span></span>
* <span data-ttu-id="eaf83-141">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="eaf83-141">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="eaf83-142">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="eaf83-142">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="eaf83-143">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="eaf83-143">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="eaf83-144">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-144">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="eaf83-145">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="eaf83-145">Azure.AnalysisServices</span></span>
* <span data-ttu-id="eaf83-146">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-146">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="eaf83-147">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="eaf83-147">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="eaf83-148">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-148">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="eaf83-149">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="eaf83-149">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="eaf83-150">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-150">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="eaf83-151">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="eaf83-151">AzureRM.Automation</span></span>
* <span data-ttu-id="eaf83-152">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-152">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="eaf83-153">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="eaf83-153">AzureRM.Backup</span></span>
* <span data-ttu-id="eaf83-154">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-154">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="eaf83-155">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="eaf83-155">AzureRM.Batch</span></span>
* <span data-ttu-id="eaf83-156">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-156">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="eaf83-157">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="eaf83-157">AzureRM.Billing</span></span>
* <span data-ttu-id="eaf83-158">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="eaf83-159">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="eaf83-159">AzureRM.Cdn</span></span>
* <span data-ttu-id="eaf83-160">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="eaf83-161">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="eaf83-161">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="eaf83-162">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-163">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-163">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-164">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-164">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="eaf83-165">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="eaf83-165">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="eaf83-166">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="eaf83-166">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="eaf83-167">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="eaf83-167">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="eaf83-168">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="eaf83-168">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="eaf83-169">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="eaf83-169">AzureRM.Consumption</span></span>
* <span data-ttu-id="eaf83-170">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="eaf83-171">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="eaf83-171">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="eaf83-172">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="eaf83-173">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="eaf83-173">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="eaf83-174">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="eaf83-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="eaf83-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="eaf83-176">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="eaf83-177">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="eaf83-177">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="eaf83-178">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="eaf83-179">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="eaf83-179">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="eaf83-180">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="eaf83-181">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="eaf83-181">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="eaf83-182">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="eaf83-182">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="eaf83-183">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="eaf83-183">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="eaf83-184">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-184">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="eaf83-185">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="eaf83-185">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="eaf83-186">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="eaf83-186">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="eaf83-187">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="eaf83-188">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="eaf83-188">AzureRM.Dns</span></span>
* <span data-ttu-id="eaf83-189">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="eaf83-190">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="eaf83-190">AzureRM.EventGrid</span></span>
* <span data-ttu-id="eaf83-191">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="eaf83-192">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="eaf83-192">AzureRM.EventHub</span></span>
* <span data-ttu-id="eaf83-193">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="eaf83-194">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="eaf83-194">AzureRM.HDInsight</span></span>
* <span data-ttu-id="eaf83-195">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="eaf83-196">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="eaf83-196">AzureRM.Insights</span></span>
* <span data-ttu-id="eaf83-197">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="eaf83-198">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="eaf83-198">AzureRM.IotHub</span></span>
* <span data-ttu-id="eaf83-199">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="eaf83-200">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="eaf83-200">AzureRM.KeyVault</span></span>
* <span data-ttu-id="eaf83-201">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="eaf83-202">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="eaf83-202">AzureRM.LogicApp</span></span>
* <span data-ttu-id="eaf83-203">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-203">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="eaf83-204">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="eaf83-204">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="eaf83-205">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-205">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="eaf83-206">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="eaf83-206">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="eaf83-207">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="eaf83-208">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="eaf83-208">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="eaf83-209">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="eaf83-210">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="eaf83-210">AzureRM.Media</span></span>
* <span data-ttu-id="eaf83-211">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-212">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-212">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-213">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="eaf83-213">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="eaf83-214">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="eaf83-214">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="eaf83-215">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="eaf83-215">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="eaf83-216">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="eaf83-216">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="eaf83-217">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="eaf83-217">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="eaf83-218">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="eaf83-218">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="eaf83-219">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="eaf83-219">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="eaf83-220">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="eaf83-220">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="eaf83-221">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="eaf83-221">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="eaf83-222">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-222">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="eaf83-223">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="eaf83-223">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="eaf83-224">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="eaf83-225">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="eaf83-225">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="eaf83-226">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="eaf83-227">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="eaf83-227">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="eaf83-228">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="eaf83-229">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="eaf83-229">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="eaf83-230">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="eaf83-231">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="eaf83-231">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="eaf83-232">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="eaf83-232">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="eaf83-233">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="eaf83-233">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="eaf83-234">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="eaf83-234">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="eaf83-235">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-235">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="eaf83-236">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="eaf83-236">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="eaf83-237">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="eaf83-237">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="eaf83-238">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="eaf83-238">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="eaf83-239">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="eaf83-239">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="eaf83-240">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="eaf83-241">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="eaf83-241">AzureRM.RedisCache</span></span>
* <span data-ttu-id="eaf83-242">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="eaf83-243">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="eaf83-243">AzureRM.Relay</span></span>
* <span data-ttu-id="eaf83-244">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="eaf83-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="eaf83-245">AzureRM.Resources</span></span>
* <span data-ttu-id="eaf83-246">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="eaf83-246">Support template deployment at subscription scope.</span></span> <span data-ttu-id="eaf83-247">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="eaf83-247">Add new Cmdlets:</span></span>
    - <span data-ttu-id="eaf83-248">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-248">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="eaf83-249">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-249">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="eaf83-250">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-250">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="eaf83-251">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-251">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="eaf83-252">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-252">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="eaf83-253">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="eaf83-253">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="eaf83-254">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="eaf83-254">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="eaf83-255">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="eaf83-255">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="eaf83-256">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-256">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="eaf83-257">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-257">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="eaf83-258">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="eaf83-258">AzureRM.Scheduler</span></span>
* <span data-ttu-id="eaf83-259">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="eaf83-260">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="eaf83-260">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="eaf83-261">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="eaf83-262">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="eaf83-262">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="eaf83-263">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="eaf83-264">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-264">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-265">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="eaf83-266">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-266">AzureRM.Storage</span></span>
* <span data-ttu-id="eaf83-267">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="eaf83-268">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="eaf83-268">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="eaf83-269">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-269">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="eaf83-270">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="eaf83-270">AzureRM.Tags</span></span>
* <span data-ttu-id="eaf83-271">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-271">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="eaf83-272">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="eaf83-272">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="eaf83-273">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-273">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="eaf83-274">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="eaf83-274">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="eaf83-275">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-275">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="eaf83-276">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="eaf83-276">AzureRM.Websites</span></span>
* <span data-ttu-id="eaf83-277">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="eaf83-278">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-278">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="eaf83-279">Geral</span><span class="sxs-lookup"><span data-stu-id="eaf83-279">General</span></span>
* <span data-ttu-id="eaf83-280">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="eaf83-280">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-281">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-281">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-282">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="eaf83-282">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="eaf83-283">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-283">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="eaf83-284">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-284">Azure.Storage</span></span>
* <span data-ttu-id="eaf83-285">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="eaf83-285">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="eaf83-286">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="eaf83-286">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="eaf83-287">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="eaf83-287">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="eaf83-288">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="eaf83-288">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="eaf83-289">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="eaf83-289">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="eaf83-290">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="eaf83-290">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="eaf83-291">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="eaf83-291">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="eaf83-292">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="eaf83-292">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="eaf83-293">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="eaf83-293">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-294">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-294">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-295">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="eaf83-295">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="eaf83-296">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="eaf83-296">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="eaf83-297">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="eaf83-297">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="eaf83-298">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="eaf83-298">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="eaf83-299">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="eaf83-299">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="eaf83-300">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="eaf83-300">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="eaf83-301">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="eaf83-301">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="eaf83-302">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="eaf83-302">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="eaf83-303">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="eaf83-303">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="eaf83-304">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="eaf83-304">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="eaf83-305">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="eaf83-305">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="eaf83-306">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="eaf83-306">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="eaf83-307">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="eaf83-307">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="eaf83-308">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-308">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="eaf83-309">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="eaf83-309">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="eaf83-310">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="eaf83-310">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="eaf83-311">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="eaf83-311">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="eaf83-312">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="eaf83-312">AzureRM.EventHub</span></span>
* <span data-ttu-id="eaf83-313">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="eaf83-313">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="eaf83-314">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="eaf83-314">AzureRM.Insights</span></span>
* <span data-ttu-id="eaf83-315">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="eaf83-315">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="eaf83-316">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="eaf83-316">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="eaf83-317">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="eaf83-317">AzureRM.KeyVault</span></span>
* <span data-ttu-id="eaf83-318">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="eaf83-318">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-319">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-319">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-320">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="eaf83-320">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="eaf83-321">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="eaf83-321">AzureRM.Resources</span></span>
* <span data-ttu-id="eaf83-322">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="eaf83-322">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="eaf83-323">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="eaf83-323">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="eaf83-324">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="eaf83-324">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="eaf83-325">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="eaf83-325">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="eaf83-326">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="eaf83-326">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="eaf83-327">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-327">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-328">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="eaf83-328">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="eaf83-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="eaf83-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="eaf83-330">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="eaf83-330">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="eaf83-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="eaf83-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="eaf83-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="eaf83-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="eaf83-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="eaf83-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="eaf83-334">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="eaf83-334">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="eaf83-335">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="eaf83-335">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="eaf83-336">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-336">AzureRM.Storage</span></span>
* <span data-ttu-id="eaf83-337">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="eaf83-337">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="eaf83-338">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="eaf83-338">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="eaf83-339">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="eaf83-339">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="eaf83-340">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="eaf83-340">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="eaf83-341">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="eaf83-341">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="eaf83-342">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="eaf83-342">AzureRM.Tags</span></span>
* <span data-ttu-id="eaf83-343">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="eaf83-343">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="eaf83-344">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-344">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-345">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-345">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-346">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="eaf83-346">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="eaf83-347">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-347">Azure.Storage</span></span>
* <span data-ttu-id="eaf83-348">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="eaf83-348">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="eaf83-349">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="eaf83-349">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="eaf83-350">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="eaf83-350">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="eaf83-351">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="eaf83-351">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="eaf83-352">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="eaf83-352">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="eaf83-353">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="eaf83-353">AzureRM.Automation</span></span>
* <span data-ttu-id="eaf83-354">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="eaf83-354">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-355">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-355">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-356">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="eaf83-356">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="eaf83-357">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="eaf83-357">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="eaf83-358">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="eaf83-358">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="eaf83-359">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="eaf83-359">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="eaf83-360">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="eaf83-360">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="eaf83-361">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="eaf83-361">AzureRM.EventHub</span></span>
* <span data-ttu-id="eaf83-362">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="eaf83-362">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="eaf83-363">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="eaf83-363">AzureRM.KeyVault</span></span>
* <span data-ttu-id="eaf83-364">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="eaf83-364">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="eaf83-365">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="eaf83-365">AzureRM.LogicApp</span></span>
* <span data-ttu-id="eaf83-366">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="eaf83-366">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-367">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-367">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-368">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="eaf83-368">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="eaf83-369">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="eaf83-369">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="eaf83-370">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="eaf83-370">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="eaf83-371">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="eaf83-371">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="eaf83-372">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="eaf83-372">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="eaf83-373">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="eaf83-373">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="eaf83-374">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="eaf83-374">AzureRM.Relay</span></span>
* <span data-ttu-id="eaf83-375">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="eaf83-375">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="eaf83-376">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="eaf83-376">AzureRM.Resources</span></span>
* <span data-ttu-id="eaf83-377">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="eaf83-377">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="eaf83-378">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="eaf83-378">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="eaf83-379">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="eaf83-379">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="eaf83-380">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="eaf83-380">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="eaf83-381">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="eaf83-381">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="eaf83-382">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="eaf83-382">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="eaf83-383">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="eaf83-383">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="eaf83-384">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="eaf83-384">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="eaf83-385">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="eaf83-385">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="eaf83-386">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="eaf83-386">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="eaf83-387">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="eaf83-387">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="eaf83-388">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="eaf83-388">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="eaf83-389">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="eaf83-389">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="eaf83-390">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="eaf83-390">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="eaf83-391">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="eaf83-391">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="eaf83-392">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="eaf83-392">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="eaf83-393">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-393">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-394">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="eaf83-394">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="eaf83-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="eaf83-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="eaf83-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="eaf83-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="eaf83-397">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="eaf83-397">AzureRM.Websites</span></span>
* <span data-ttu-id="eaf83-398">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="eaf83-398">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="eaf83-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="eaf83-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="eaf83-400">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="eaf83-400">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="eaf83-401">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-401">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="eaf83-402">Geral</span><span class="sxs-lookup"><span data-stu-id="eaf83-402">General</span></span>
* <span data-ttu-id="eaf83-403">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="eaf83-403">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-404">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-404">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-405">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="eaf83-405">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-406">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-406">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-407">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="eaf83-407">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="eaf83-408">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="eaf83-408">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="eaf83-409">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="eaf83-409">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="eaf83-410">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="eaf83-410">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="eaf83-411">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-411">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="eaf83-412">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-412">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="eaf83-413">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-413">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="eaf83-414">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="eaf83-414">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="eaf83-415">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="eaf83-415">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="eaf83-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="eaf83-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="eaf83-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="eaf83-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="eaf83-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="eaf83-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="eaf83-419">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="eaf83-419">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="eaf83-420">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="eaf83-420">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="eaf83-421">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="eaf83-421">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="eaf83-422">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="eaf83-422">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="eaf83-423">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="eaf83-423">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="eaf83-424">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="eaf83-424">AzureRM.EventHub</span></span>
* <span data-ttu-id="eaf83-425">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="eaf83-425">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="eaf83-426">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="eaf83-426">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="eaf83-427">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="eaf83-427">Provided Default Parameter set.</span></span>
* <span data-ttu-id="eaf83-428">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="eaf83-428">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="eaf83-429">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="eaf83-429">AzureRM.KeyVault</span></span>
* <span data-ttu-id="eaf83-430">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="eaf83-430">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-431">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-431">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-432">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="eaf83-432">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="eaf83-433">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="eaf83-433">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="eaf83-434">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="eaf83-434">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="eaf83-435">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="eaf83-435">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="eaf83-436">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="eaf83-436">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="eaf83-437">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="eaf83-437">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="eaf83-438">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="eaf83-438">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="eaf83-439">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="eaf83-439">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="eaf83-440">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="eaf83-440">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="eaf83-441">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="eaf83-441">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="eaf83-442">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="eaf83-442">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="eaf83-443">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="eaf83-443">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="eaf83-444">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="eaf83-444">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="eaf83-445">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="eaf83-445">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="eaf83-446">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="eaf83-446">AzureRM.Resources</span></span>
* <span data-ttu-id="eaf83-447">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="eaf83-447">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="eaf83-448">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="eaf83-448">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="eaf83-449">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="eaf83-449">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="eaf83-450">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="eaf83-450">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="eaf83-451">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="eaf83-451">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="eaf83-452">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="eaf83-452">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="eaf83-453">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="eaf83-453">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="eaf83-454">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="eaf83-454">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="eaf83-455">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="eaf83-455">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="eaf83-456">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="eaf83-456">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="eaf83-457">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="eaf83-457">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="eaf83-458">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="eaf83-458">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="eaf83-459">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="eaf83-459">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="eaf83-460">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="eaf83-460">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="eaf83-461">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="eaf83-461">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="eaf83-462">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-462">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-463">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="eaf83-463">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="eaf83-464">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="eaf83-464">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="eaf83-465">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-465">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-466">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-466">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-467">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="eaf83-467">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="eaf83-468">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="eaf83-468">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="eaf83-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="eaf83-469">Azure.Storage</span></span>
* <span data-ttu-id="eaf83-470">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="eaf83-470">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-471">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-471">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-472">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="eaf83-472">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="eaf83-473">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="eaf83-473">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="eaf83-474">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="eaf83-474">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="eaf83-475">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="eaf83-475">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="eaf83-476">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="eaf83-476">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="eaf83-477">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="eaf83-477">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="eaf83-478">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="eaf83-478">Start-AzureRmVM</span></span>
    - <span data-ttu-id="eaf83-479">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="eaf83-479">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="eaf83-480">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="eaf83-480">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="eaf83-481">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="eaf83-481">Set-AzureRmVM</span></span>
    - <span data-ttu-id="eaf83-482">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="eaf83-482">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="eaf83-483">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-483">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="eaf83-484">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="eaf83-484">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="eaf83-485">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="eaf83-485">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="eaf83-486">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-486">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="eaf83-487">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-487">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="eaf83-488">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-488">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="eaf83-489">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="eaf83-489">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="eaf83-490">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="eaf83-490">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="eaf83-491">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="eaf83-491">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="eaf83-492">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="eaf83-492">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="eaf83-493">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="eaf83-493">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="eaf83-494">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="eaf83-494">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="eaf83-495">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="eaf83-495">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="eaf83-496">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="eaf83-496">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="eaf83-497">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="eaf83-497">AzureRM.EventGrid</span></span>
* <span data-ttu-id="eaf83-498">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="eaf83-498">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="eaf83-499">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="eaf83-499">AzureRM.KeyVault</span></span>
* <span data-ttu-id="eaf83-500">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="eaf83-500">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="eaf83-501">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="eaf83-501">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="eaf83-502">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="eaf83-502">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="eaf83-503">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="eaf83-503">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="eaf83-504">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="eaf83-504">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="eaf83-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="eaf83-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="eaf83-506">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="eaf83-506">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="eaf83-507">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="eaf83-507">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="eaf83-508">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-508">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-509">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="eaf83-509">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="eaf83-510">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="eaf83-510">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="eaf83-511">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="eaf83-511">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="eaf83-512">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="eaf83-512">AzureRM.Websites</span></span>
* <span data-ttu-id="eaf83-513">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="eaf83-513">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="eaf83-514">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="eaf83-514">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="eaf83-515">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-515">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="eaf83-516">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="eaf83-516">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="eaf83-517">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="eaf83-517">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="eaf83-518">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-518">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-519">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-519">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-520">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="eaf83-520">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="eaf83-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="eaf83-521">AzureRM.Compute</span></span>
* <span data-ttu-id="eaf83-522">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="eaf83-522">VMSS VM Update feature</span></span>
    - <span data-ttu-id="eaf83-523">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="eaf83-523">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="eaf83-524">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="eaf83-524">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="eaf83-525">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="eaf83-525">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="eaf83-526">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="eaf83-526">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="eaf83-527">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="eaf83-527">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="eaf83-528">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="eaf83-528">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="eaf83-529">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="eaf83-529">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="eaf83-530">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="eaf83-530">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="eaf83-531">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="eaf83-531">AzureRM.KeyVault</span></span>
* <span data-ttu-id="eaf83-532">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="eaf83-532">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-533">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-534">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="eaf83-534">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="eaf83-535">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="eaf83-535">AzureRM.Resources</span></span>
* <span data-ttu-id="eaf83-536">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="eaf83-536">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="eaf83-537">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="eaf83-537">AzureRM.Scheduler</span></span>
* <span data-ttu-id="eaf83-538">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="eaf83-538">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="eaf83-539">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-539">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-540">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="eaf83-540">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="eaf83-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="eaf83-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="eaf83-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="eaf83-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="eaf83-543">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="eaf83-543">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="eaf83-544">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="eaf83-544">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="eaf83-545">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="eaf83-545">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="eaf83-546">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="eaf83-546">AzureRM.Websites</span></span>
* <span data-ttu-id="eaf83-547">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="eaf83-547">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="eaf83-548">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="eaf83-548">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="eaf83-549">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="eaf83-549">AzureRM.Profile</span></span>
* <span data-ttu-id="eaf83-550">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="eaf83-550">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="eaf83-551">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="eaf83-551">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="eaf83-552">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="eaf83-552">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="eaf83-553">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="eaf83-553">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="eaf83-554">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="eaf83-554">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="eaf83-555">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="eaf83-555">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="eaf83-556">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="eaf83-556">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="eaf83-557">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="eaf83-557">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="eaf83-558">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="eaf83-558">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="eaf83-559">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="eaf83-559">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="eaf83-560">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="eaf83-560">Added support for MSI identity</span></span>
* <span data-ttu-id="eaf83-561">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="eaf83-561">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="eaf83-562">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="eaf83-562">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="eaf83-563">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="eaf83-563">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="eaf83-564">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="eaf83-564">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="eaf83-565">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="eaf83-565">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="eaf83-566">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="eaf83-566">AzureRM.Batch</span></span>
* <span data-ttu-id="eaf83-567">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="eaf83-567">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="eaf83-568">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="eaf83-568">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="eaf83-569">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="eaf83-569">AzureRM.Consumption</span></span>
* <span data-ttu-id="eaf83-570">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="eaf83-570">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="eaf83-571">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="eaf83-571">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="eaf83-572">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="eaf83-572">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="eaf83-573">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="eaf83-573">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="eaf83-574">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="eaf83-574">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="eaf83-575">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="eaf83-575">AzureRM.Network</span></span>
* <span data-ttu-id="eaf83-576">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="eaf83-576">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="eaf83-577">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="eaf83-577">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="eaf83-578">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="eaf83-578">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="eaf83-579">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="eaf83-579">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="eaf83-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="eaf83-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="eaf83-581">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="eaf83-581">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="eaf83-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="eaf83-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="eaf83-583">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="eaf83-583">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="eaf83-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="eaf83-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="eaf83-585">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="eaf83-585">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="eaf83-586">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="eaf83-586">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="eaf83-587">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="eaf83-587">AzureRM.Sql</span></span>
* <span data-ttu-id="eaf83-588">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="eaf83-588">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="eaf83-589">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="eaf83-589">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="eaf83-590">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="eaf83-590">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="eaf83-591">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="eaf83-591">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="eaf83-592">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="eaf83-592">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="eaf83-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="eaf83-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="eaf83-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="eaf83-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="eaf83-595">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="eaf83-595">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="eaf83-596">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="eaf83-596">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="eaf83-597">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="eaf83-597">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="eaf83-598">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="eaf83-598">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="eaf83-599">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="eaf83-599">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
