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
ms.openlocfilehash: f4f3141998be14f0b5b223aed1af283534bf061d
ms.sourcegitcommit: 971f19181b2cd68b7845bbebdb22858c06541c8c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/06/2018
ms.locfileid: "43383843"
---
# <a name="release-notes"></a><span data-ttu-id="7dff6-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="7dff6-103">Release notes</span></span>

<span data-ttu-id="7dff6-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="7dff6-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="681---august-2018"></a><span data-ttu-id="7dff6-105">6.8.1 - Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-105">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7dff6-106">Geral</span><span class="sxs-lookup"><span data-stu-id="7dff6-106">General</span></span>
* <span data-ttu-id="7dff6-107">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7dff6-107">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="7dff6-108">Assemblagens de runtime comum atualizadas</span><span class="sxs-lookup"><span data-stu-id="7dff6-108">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7dff6-109">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7dff6-109">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7dff6-110">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7dff6-110">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="7dff6-111">Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-111">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="7dff6-112">Agora, os cmdlets Import-AzureRmApiManagementApi e \*-AzureRmApiManagementCertificate identificam caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="7dff6-112">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="7dff6-113">Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-113">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="7dff6-114">O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="7dff6-114">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="7dff6-115">Corrigido com a atualização para 4.0.4-nuget de pré-visualização</span><span class="sxs-lookup"><span data-stu-id="7dff6-115">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="7dff6-116">Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="7dff6-117">Foi corrigido o filtro de Odata para procurar por nome de produto</span><span class="sxs-lookup"><span data-stu-id="7dff6-117">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="7dff6-118">Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="7dff6-119">Foi corrigido o filtro de Odata para procurar por nome na API</span><span class="sxs-lookup"><span data-stu-id="7dff6-119">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="7dff6-120">Foi adicionado suporte para o logger de AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="7dff6-120">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-121">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-121">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-122">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="7dff6-122">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="7dff6-123">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="7dff6-123">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="7dff6-124">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7dff6-124">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="7dff6-125">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="7dff6-125">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-126">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-126">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-127">Representação de saída de cmdlet predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="7dff6-127">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="7dff6-128">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7dff6-128">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="7dff6-129">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="7dff6-129">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="7dff6-130">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-130">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-131">Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7dff6-131">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7dff6-132">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7dff6-132">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7dff6-133">Problemas corrigidos</span><span class="sxs-lookup"><span data-stu-id="7dff6-133">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7dff6-134">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7dff6-134">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7dff6-135">Suporte adicionado para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="7dff6-135">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="7dff6-136">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="7dff6-136">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="7dff6-137">Suporte adicionado para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="7dff6-137">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="7dff6-138">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="7dff6-138">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="7dff6-139">Suporte adicionado para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7dff6-139">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="7dff6-140">Suporte adicionado para intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7dff6-140">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="7dff6-141">Suporte adicionado para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="7dff6-141">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="7dff6-142">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-142">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7dff6-143">Geral</span><span class="sxs-lookup"><span data-stu-id="7dff6-143">General</span></span>
* <span data-ttu-id="7dff6-144">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="7dff6-144">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-145">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-145">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-146">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="7dff6-146">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-147">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-147">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-148">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="7dff6-148">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="7dff6-149">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="7dff6-149">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="7dff6-150">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="7dff6-150">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="7dff6-151">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="7dff6-151">AzureRM.IotHub</span></span>
* <span data-ttu-id="7dff6-152">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="7dff6-152">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-153">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-153">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-154">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="7dff6-154">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="7dff6-155">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7dff6-155">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="7dff6-156">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="7dff6-156">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7dff6-157">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-157">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-158">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7dff6-158">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7dff6-159">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7dff6-159">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7dff6-160">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="7dff6-160">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7dff6-161">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7dff6-161">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7dff6-162">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="7dff6-162">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="7dff6-163">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="7dff6-163">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="7dff6-164">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="7dff6-164">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="7dff6-165">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="7dff6-165">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="7dff6-166">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7dff6-166">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="7dff6-167">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="7dff6-167">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="7dff6-168">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="7dff6-168">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7dff6-169">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7dff6-169">AzureRM.Websites</span></span>
* <span data-ttu-id="7dff6-170">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="7dff6-170">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="7dff6-171">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-171">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-172">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-172">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-173">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-173">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7dff6-174">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="7dff6-174">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="7dff6-175">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="7dff6-175">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="7dff6-176">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="7dff6-176">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="7dff6-177">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-177">Azure.Storage</span></span>
* <span data-ttu-id="7dff6-178">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="7dff6-178">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="7dff6-179">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="7dff6-179">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="7dff6-180">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7dff6-180">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="7dff6-181">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-181">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="7dff6-182">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7dff6-182">Azure.AnalysisServices</span></span>
* <span data-ttu-id="7dff6-183">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-183">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7dff6-184">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7dff6-184">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7dff6-185">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-185">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="7dff6-186">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="7dff6-186">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="7dff6-187">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="7dff6-188">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="7dff6-188">AzureRM.Automation</span></span>
* <span data-ttu-id="7dff6-189">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="7dff6-190">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="7dff6-190">AzureRM.Backup</span></span>
* <span data-ttu-id="7dff6-191">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="7dff6-192">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="7dff6-192">AzureRM.Batch</span></span>
* <span data-ttu-id="7dff6-193">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="7dff6-194">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="7dff6-194">AzureRM.Billing</span></span>
* <span data-ttu-id="7dff6-195">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="7dff6-196">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="7dff6-196">AzureRM.Cdn</span></span>
* <span data-ttu-id="7dff6-197">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="7dff6-198">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7dff6-198">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="7dff6-199">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-200">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-200">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-201">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-201">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7dff6-202">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="7dff6-202">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="7dff6-203">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="7dff6-203">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="7dff6-204">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="7dff6-204">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="7dff6-205">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="7dff6-205">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="7dff6-206">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="7dff6-206">AzureRM.Consumption</span></span>
* <span data-ttu-id="7dff6-207">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="7dff6-208">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7dff6-208">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="7dff6-209">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="7dff6-210">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="7dff6-210">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="7dff6-211">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="7dff6-212">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="7dff6-212">AzureRM.DataFactories</span></span>
* <span data-ttu-id="7dff6-213">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7dff6-214">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7dff6-214">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7dff6-215">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="7dff6-216">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7dff6-216">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="7dff6-217">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-217">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7dff6-218">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7dff6-218">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7dff6-219">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="7dff6-219">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="7dff6-220">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="7dff6-220">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="7dff6-221">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-221">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7dff6-222">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7dff6-222">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="7dff6-223">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="7dff6-223">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="7dff6-224">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="7dff6-225">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="7dff6-225">AzureRM.Dns</span></span>
* <span data-ttu-id="7dff6-226">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="7dff6-227">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7dff6-227">AzureRM.EventGrid</span></span>
* <span data-ttu-id="7dff6-228">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7dff6-229">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7dff6-229">AzureRM.EventHub</span></span>
* <span data-ttu-id="7dff6-230">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="7dff6-231">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7dff6-231">AzureRM.HDInsight</span></span>
* <span data-ttu-id="7dff6-232">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="7dff6-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7dff6-233">AzureRM.Insights</span></span>
* <span data-ttu-id="7dff6-234">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="7dff6-235">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="7dff6-235">AzureRM.IotHub</span></span>
* <span data-ttu-id="7dff6-236">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7dff6-237">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7dff6-237">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7dff6-238">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="7dff6-239">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7dff6-239">AzureRM.LogicApp</span></span>
* <span data-ttu-id="7dff6-240">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="7dff6-241">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7dff6-241">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="7dff6-242">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="7dff6-243">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="7dff6-243">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="7dff6-244">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="7dff6-245">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="7dff6-245">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="7dff6-246">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="7dff6-247">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="7dff6-247">AzureRM.Media</span></span>
* <span data-ttu-id="7dff6-248">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-249">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-249">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-250">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="7dff6-250">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="7dff6-251">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="7dff6-251">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="7dff6-252">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="7dff6-252">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="7dff6-253">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="7dff6-253">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="7dff6-254">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="7dff6-254">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="7dff6-255">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="7dff6-255">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="7dff6-256">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="7dff6-256">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="7dff6-257">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="7dff6-257">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="7dff6-258">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="7dff6-258">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="7dff6-259">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="7dff6-260">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7dff6-260">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="7dff6-261">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="7dff6-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7dff6-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="7dff6-263">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="7dff6-264">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7dff6-264">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="7dff6-265">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="7dff6-266">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7dff6-266">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="7dff6-267">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7dff6-268">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7dff6-268">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7dff6-269">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="7dff6-269">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="7dff6-270">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="7dff6-270">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="7dff6-271">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="7dff6-271">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="7dff6-272">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-272">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="7dff6-273">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="7dff6-273">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="7dff6-274">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="7dff6-274">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="7dff6-275">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="7dff6-275">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="7dff6-276">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="7dff6-276">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="7dff6-277">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="7dff6-278">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7dff6-278">AzureRM.RedisCache</span></span>
* <span data-ttu-id="7dff6-279">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-279">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="7dff6-280">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="7dff6-280">AzureRM.Relay</span></span>
* <span data-ttu-id="7dff6-281">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-281">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7dff6-282">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-282">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-283">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="7dff6-283">Support template deployment at subscription scope.</span></span> <span data-ttu-id="7dff6-284">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7dff6-284">Add new Cmdlets:</span></span>
    - <span data-ttu-id="7dff6-285">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-285">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="7dff6-286">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-286">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="7dff6-287">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-287">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="7dff6-288">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-288">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="7dff6-289">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-289">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="7dff6-290">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="7dff6-290">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="7dff6-291">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="7dff6-291">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="7dff6-292">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="7dff6-292">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="7dff6-293">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-293">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="7dff6-294">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-294">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="7dff6-295">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="7dff6-295">AzureRM.Scheduler</span></span>
* <span data-ttu-id="7dff6-296">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-296">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7dff6-297">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7dff6-297">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7dff6-298">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-298">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7dff6-299">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7dff6-299">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7dff6-300">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-300">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7dff6-301">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-301">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-302">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-302">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="7dff6-303">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-303">AzureRM.Storage</span></span>
* <span data-ttu-id="7dff6-304">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-304">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="7dff6-305">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="7dff6-305">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="7dff6-306">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-306">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="7dff6-307">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="7dff6-307">AzureRM.Tags</span></span>
* <span data-ttu-id="7dff6-308">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-308">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7dff6-309">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7dff6-309">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7dff6-310">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="7dff6-311">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="7dff6-311">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="7dff6-312">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7dff6-313">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7dff6-313">AzureRM.Websites</span></span>
* <span data-ttu-id="7dff6-314">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="7dff6-315">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-315">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7dff6-316">Geral</span><span class="sxs-lookup"><span data-stu-id="7dff6-316">General</span></span>
* <span data-ttu-id="7dff6-317">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="7dff6-317">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-318">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-318">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-319">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="7dff6-319">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="7dff6-320">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-320">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="7dff6-321">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-321">Azure.Storage</span></span>
* <span data-ttu-id="7dff6-322">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="7dff6-322">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="7dff6-323">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7dff6-323">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7dff6-324">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7dff6-324">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7dff6-325">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-325">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="7dff6-326">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="7dff6-326">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="7dff6-327">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-327">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="7dff6-328">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="7dff6-328">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="7dff6-329">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="7dff6-329">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="7dff6-330">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="7dff6-330">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-331">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-331">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-332">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="7dff6-332">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="7dff6-333">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="7dff6-333">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="7dff6-334">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="7dff6-334">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="7dff6-335">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="7dff6-335">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="7dff6-336">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="7dff6-336">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="7dff6-337">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="7dff6-337">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="7dff6-338">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="7dff6-338">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="7dff6-339">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="7dff6-339">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="7dff6-340">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="7dff6-340">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="7dff6-341">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="7dff6-341">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7dff6-342">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7dff6-342">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7dff6-343">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="7dff6-343">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="7dff6-344">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="7dff6-344">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="7dff6-345">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-345">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="7dff6-346">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="7dff6-346">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7dff6-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7dff6-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7dff6-348">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="7dff6-348">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7dff6-349">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7dff6-349">AzureRM.EventHub</span></span>
* <span data-ttu-id="7dff6-350">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="7dff6-350">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="7dff6-351">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7dff6-351">AzureRM.Insights</span></span>
* <span data-ttu-id="7dff6-352">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="7dff6-352">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="7dff6-353">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="7dff6-353">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7dff6-354">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7dff6-354">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7dff6-355">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7dff6-355">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-356">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-356">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-357">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="7dff6-357">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7dff6-358">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-358">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-359">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="7dff6-359">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="7dff6-360">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="7dff6-360">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7dff6-361">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7dff6-361">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7dff6-362">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="7dff6-362">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="7dff6-363">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="7dff6-363">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="7dff6-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-364">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-365">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7dff6-365">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="7dff6-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7dff6-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="7dff6-367">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7dff6-367">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="7dff6-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="7dff6-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="7dff6-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="7dff6-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="7dff6-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="7dff6-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="7dff6-371">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="7dff6-371">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="7dff6-372">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="7dff6-372">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="7dff6-373">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-373">AzureRM.Storage</span></span>
* <span data-ttu-id="7dff6-374">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="7dff6-374">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="7dff6-375">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="7dff6-375">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="7dff6-376">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7dff6-376">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="7dff6-377">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7dff6-377">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="7dff6-378">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7dff6-378">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="7dff6-379">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="7dff6-379">AzureRM.Tags</span></span>
* <span data-ttu-id="7dff6-380">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="7dff6-380">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="7dff6-381">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-381">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-382">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-383">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="7dff6-383">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="7dff6-384">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-384">Azure.Storage</span></span>
* <span data-ttu-id="7dff6-385">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="7dff6-385">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="7dff6-386">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7dff6-386">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="7dff6-387">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="7dff6-387">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="7dff6-388">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7dff6-388">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="7dff6-389">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="7dff6-389">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="7dff6-390">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="7dff6-390">AzureRM.Automation</span></span>
* <span data-ttu-id="7dff6-391">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="7dff6-391">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-392">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-392">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-393">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="7dff6-393">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="7dff6-394">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="7dff6-394">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="7dff6-395">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="7dff6-395">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="7dff6-396">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="7dff6-396">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="7dff6-397">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="7dff6-397">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7dff6-398">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7dff6-398">AzureRM.EventHub</span></span>
* <span data-ttu-id="7dff6-399">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="7dff6-399">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7dff6-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7dff6-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7dff6-401">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7dff6-401">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="7dff6-402">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7dff6-402">AzureRM.LogicApp</span></span>
* <span data-ttu-id="7dff6-403">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="7dff6-403">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-404">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-404">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-405">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="7dff6-405">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="7dff6-406">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="7dff6-406">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="7dff6-407">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="7dff6-407">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="7dff6-408">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="7dff6-408">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="7dff6-409">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="7dff6-409">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="7dff6-410">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="7dff6-410">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="7dff6-411">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="7dff6-411">AzureRM.Relay</span></span>
* <span data-ttu-id="7dff6-412">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="7dff6-412">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7dff6-413">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-413">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-414">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="7dff6-414">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="7dff6-415">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="7dff6-415">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="7dff6-416">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7dff6-416">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="7dff6-417">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="7dff6-417">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="7dff6-418">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7dff6-418">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="7dff6-419">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7dff6-419">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7dff6-420">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="7dff6-420">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="7dff6-421">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="7dff6-421">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="7dff6-422">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7dff6-422">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7dff6-423">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7dff6-423">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7dff6-424">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7dff6-424">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7dff6-425">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7dff6-425">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="7dff6-426">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="7dff6-426">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="7dff6-427">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="7dff6-427">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7dff6-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7dff6-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7dff6-429">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="7dff6-429">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7dff6-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-430">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-431">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="7dff6-431">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="7dff6-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="7dff6-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="7dff6-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="7dff6-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7dff6-434">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7dff6-434">AzureRM.Websites</span></span>
* <span data-ttu-id="7dff6-435">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="7dff6-435">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="7dff6-436">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="7dff6-436">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="7dff6-437">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="7dff6-437">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="7dff6-438">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-438">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7dff6-439">Geral</span><span class="sxs-lookup"><span data-stu-id="7dff6-439">General</span></span>
* <span data-ttu-id="7dff6-440">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="7dff6-440">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-441">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-441">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-442">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="7dff6-442">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-443">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-443">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-444">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="7dff6-444">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="7dff6-445">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="7dff6-445">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="7dff6-446">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="7dff6-446">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="7dff6-447">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="7dff6-447">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="7dff6-448">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-448">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="7dff6-449">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-449">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="7dff6-450">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-450">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="7dff6-451">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7dff6-451">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="7dff6-452">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7dff6-452">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="7dff6-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7dff6-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="7dff6-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7dff6-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="7dff6-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7dff6-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7dff6-456">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7dff6-456">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7dff6-457">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="7dff6-457">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="7dff6-458">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="7dff6-458">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="7dff6-459">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="7dff6-459">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="7dff6-460">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="7dff6-460">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="7dff6-461">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7dff6-461">AzureRM.EventHub</span></span>
* <span data-ttu-id="7dff6-462">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="7dff6-462">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="7dff6-463">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="7dff6-463">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="7dff6-464">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="7dff6-464">Provided Default Parameter set.</span></span>
* <span data-ttu-id="7dff6-465">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="7dff6-465">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7dff6-466">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7dff6-466">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7dff6-467">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="7dff6-467">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-468">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-468">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-469">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="7dff6-469">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="7dff6-470">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="7dff6-470">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="7dff6-471">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="7dff6-471">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="7dff6-472">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="7dff6-472">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="7dff6-473">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="7dff6-473">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="7dff6-474">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="7dff6-474">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="7dff6-475">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="7dff6-475">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="7dff6-476">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="7dff6-476">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="7dff6-477">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="7dff6-477">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="7dff6-478">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7dff6-478">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7dff6-479">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7dff6-479">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7dff6-480">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="7dff6-480">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="7dff6-481">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="7dff6-481">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="7dff6-482">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="7dff6-482">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7dff6-483">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-483">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-484">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="7dff6-484">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="7dff6-485">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7dff6-485">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="7dff6-486">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7dff6-486">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="7dff6-487">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="7dff6-487">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="7dff6-488">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="7dff6-488">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="7dff6-489">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7dff6-489">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="7dff6-490">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="7dff6-490">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="7dff6-491">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="7dff6-491">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="7dff6-492">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="7dff6-492">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="7dff6-493">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="7dff6-493">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="7dff6-494">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="7dff6-494">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="7dff6-495">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="7dff6-495">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="7dff6-496">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="7dff6-496">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="7dff6-497">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7dff6-497">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="7dff6-498">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="7dff6-498">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7dff6-499">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-499">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-500">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="7dff6-500">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="7dff6-501">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="7dff6-501">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="7dff6-502">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-502">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-503">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-503">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-504">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="7dff6-504">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="7dff6-505">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="7dff6-505">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="7dff6-506">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7dff6-506">Azure.Storage</span></span>
* <span data-ttu-id="7dff6-507">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="7dff6-507">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-508">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-508">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-509">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="7dff6-509">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="7dff6-510">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="7dff6-510">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="7dff6-511">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="7dff6-511">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="7dff6-512">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="7dff6-512">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="7dff6-513">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="7dff6-513">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="7dff6-514">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="7dff6-514">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="7dff6-515">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7dff6-515">Start-AzureRmVM</span></span>
    - <span data-ttu-id="7dff6-516">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7dff6-516">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="7dff6-517">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7dff6-517">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="7dff6-518">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="7dff6-518">Set-AzureRmVM</span></span>
    - <span data-ttu-id="7dff6-519">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="7dff6-519">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="7dff6-520">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-520">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="7dff6-521">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="7dff6-521">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="7dff6-522">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="7dff6-522">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="7dff6-523">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-523">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="7dff6-524">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-524">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="7dff6-525">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-525">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="7dff6-526">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="7dff6-526">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="7dff6-527">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="7dff6-527">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="7dff6-528">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="7dff6-528">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="7dff6-529">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="7dff6-529">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="7dff6-530">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="7dff6-530">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="7dff6-531">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="7dff6-531">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="7dff6-532">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="7dff6-532">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="7dff6-533">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="7dff6-533">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="7dff6-534">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7dff6-534">AzureRM.EventGrid</span></span>
* <span data-ttu-id="7dff6-535">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="7dff6-535">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="7dff6-536">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7dff6-536">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7dff6-537">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="7dff6-537">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="7dff6-538">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7dff6-538">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="7dff6-539">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="7dff6-539">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="7dff6-540">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="7dff6-540">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="7dff6-541">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dff6-541">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="7dff6-542">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7dff6-542">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7dff6-543">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="7dff6-543">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="7dff6-544">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="7dff6-544">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7dff6-545">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-545">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-546">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="7dff6-546">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7dff6-547">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7dff6-547">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7dff6-548">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="7dff6-548">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7dff6-549">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7dff6-549">AzureRM.Websites</span></span>
* <span data-ttu-id="7dff6-550">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="7dff6-550">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="7dff6-551">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="7dff6-551">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="7dff6-552">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-552">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="7dff6-553">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7dff6-553">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="7dff6-554">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="7dff6-554">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="7dff6-555">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-555">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-556">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-556">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-557">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="7dff6-557">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="7dff6-558">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7dff6-558">AzureRM.Compute</span></span>
* <span data-ttu-id="7dff6-559">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="7dff6-559">VMSS VM Update feature</span></span>
    - <span data-ttu-id="7dff6-560">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="7dff6-560">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="7dff6-561">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="7dff6-561">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7dff6-562">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7dff6-562">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7dff6-563">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="7dff6-563">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="7dff6-564">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="7dff6-564">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="7dff6-565">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="7dff6-565">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="7dff6-566">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="7dff6-566">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="7dff6-567">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="7dff6-567">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="7dff6-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7dff6-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7dff6-569">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="7dff6-569">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-570">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-570">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-571">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="7dff6-571">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="7dff6-572">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7dff6-572">AzureRM.Resources</span></span>
* <span data-ttu-id="7dff6-573">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="7dff6-573">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="7dff6-574">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="7dff6-574">AzureRM.Scheduler</span></span>
* <span data-ttu-id="7dff6-575">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="7dff6-575">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="7dff6-576">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-576">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-577">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="7dff6-577">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="7dff6-578">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7dff6-578">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="7dff6-579">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="7dff6-579">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="7dff6-580">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="7dff6-580">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="7dff6-581">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="7dff6-581">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="7dff6-582">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7dff6-582">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="7dff6-583">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7dff6-583">AzureRM.Websites</span></span>
* <span data-ttu-id="7dff6-584">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="7dff6-584">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="7dff6-585">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="7dff6-585">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="7dff6-586">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7dff6-586">AzureRM.Profile</span></span>
* <span data-ttu-id="7dff6-587">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="7dff6-587">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="7dff6-588">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7dff6-588">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="7dff6-589">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="7dff6-589">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="7dff6-590">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7dff6-590">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7dff6-591">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="7dff6-591">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="7dff6-592">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7dff6-592">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="7dff6-593">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="7dff6-593">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="7dff6-594">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="7dff6-594">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="7dff6-595">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="7dff6-595">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="7dff6-596">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="7dff6-596">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="7dff6-597">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="7dff6-597">Added support for MSI identity</span></span>
* <span data-ttu-id="7dff6-598">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="7dff6-598">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="7dff6-599">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="7dff6-599">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="7dff6-600">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dff6-600">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="7dff6-601">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="7dff6-601">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="7dff6-602">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="7dff6-602">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="7dff6-603">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="7dff6-603">AzureRM.Batch</span></span>
* <span data-ttu-id="7dff6-604">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="7dff6-604">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="7dff6-605">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="7dff6-605">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="7dff6-606">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="7dff6-606">AzureRM.Consumption</span></span>
* <span data-ttu-id="7dff6-607">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="7dff6-607">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="7dff6-608">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7dff6-608">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7dff6-609">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="7dff6-609">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="7dff6-610">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7dff6-610">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="7dff6-611">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="7dff6-611">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="7dff6-612">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7dff6-612">AzureRM.Network</span></span>
* <span data-ttu-id="7dff6-613">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="7dff6-613">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="7dff6-614">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="7dff6-614">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="7dff6-615">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dff6-615">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="7dff6-616">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7dff6-616">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="7dff6-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="7dff6-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="7dff6-618">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7dff6-618">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="7dff6-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="7dff6-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="7dff6-620">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="7dff6-620">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="7dff6-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="7dff6-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="7dff6-622">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7dff6-622">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7dff6-623">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="7dff6-623">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="7dff6-624">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="7dff6-624">AzureRM.Sql</span></span>
* <span data-ttu-id="7dff6-625">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="7dff6-625">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="7dff6-626">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="7dff6-626">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="7dff6-627">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="7dff6-627">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="7dff6-628">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="7dff6-628">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="7dff6-629">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="7dff6-629">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="7dff6-630">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7dff6-630">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="7dff6-631">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="7dff6-631">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="7dff6-632">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="7dff6-632">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="7dff6-633">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="7dff6-633">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="7dff6-634">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="7dff6-634">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="7dff6-635">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7dff6-635">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="7dff6-636">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="7dff6-636">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
