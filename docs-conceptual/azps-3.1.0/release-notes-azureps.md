---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: 2280b594ee9f525b2fa3175c917f6365cea354ba
ms.sourcegitcommit: 45e1823aa1a792840aa4829831b5f67a9d5d24a0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/26/2019
ms.locfileid: "74537127"
---
## <a name="310---november-2019"></a><span data-ttu-id="1c1bc-103">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-103">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c1bc-104">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c1bc-104">Highlights since the last major release</span></span>
* <span data-ttu-id="1c1bc-105">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="1c1bc-105">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="1c1bc-106">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="1c1bc-106">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-107">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-108">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-108">VM Reapply feature</span></span>
    - <span data-ttu-id="1c1bc-109">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-109">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="1c1bc-110">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-110">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="1c1bc-111">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-111">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="1c1bc-112">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-112">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="1c1bc-113">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-113">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="1c1bc-114">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="1c1bc-114">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="1c1bc-115">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="1c1bc-115">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="1c1bc-116">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="1c1bc-116">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="1c1bc-117">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="1c1bc-117">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="1c1bc-118">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-118">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="1c1bc-119">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="1c1bc-119">Az.DataBoxEdge</span></span>
* <span data-ttu-id="1c1bc-120">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-120">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="1c1bc-121">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-121">Get the Order</span></span>
* <span data-ttu-id="1c1bc-122">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-122">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="1c1bc-123">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-123">Create new Order</span></span>
* <span data-ttu-id="1c1bc-124">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-124">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="1c1bc-125">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-125">Remove the Order</span></span>
* <span data-ttu-id="1c1bc-126">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-126">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="1c1bc-127">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="1c1bc-127">Now creates Local Share</span></span>
* <span data-ttu-id="1c1bc-128">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-128">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="1c1bc-129">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="1c1bc-129">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="1c1bc-130">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-130">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="1c1bc-131">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-131">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="1c1bc-132">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-132">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="1c1bc-133">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="1c1bc-133">Gets the information about Triggers</span></span>
* <span data-ttu-id="1c1bc-134">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-134">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="1c1bc-135">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="1c1bc-135">Create new Triggers</span></span>
* <span data-ttu-id="1c1bc-136">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-136">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="1c1bc-137">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="1c1bc-137">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-138">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-139">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-139">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="1c1bc-140">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-140">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-141">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-141">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-142">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="1c1bc-142">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c1bc-143">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-143">Az.EventHub</span></span>
* <span data-ttu-id="1c1bc-144">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="1c1bc-144">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c1bc-145">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-145">Az.FrontDoor</span></span>
* <span data-ttu-id="1c1bc-146">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-146">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="1c1bc-147">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-147">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="1c1bc-148">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="1c1bc-148">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="1c1bc-149">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-149">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-150">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-150">Az.Network</span></span>
* <span data-ttu-id="1c1bc-151">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-151">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="1c1bc-152">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="1c1bc-152">Az.PrivateDns</span></span>
* <span data-ttu-id="1c1bc-153">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-153">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-154">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-154">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-155">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-155">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="1c1bc-156">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-156">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="1c1bc-157">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-157">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c1bc-158">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c1bc-158">Az.RedisCache</span></span>
* <span data-ttu-id="1c1bc-159">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-159">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="1c1bc-160">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-160">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="1c1bc-161">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-161">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-162">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-162">Az.Resources</span></span>
- <span data-ttu-id="1c1bc-163">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-163">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="1c1bc-164">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-164">Updated create policy definition help example</span></span>
- <span data-ttu-id="1c1bc-165">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-165">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="1c1bc-166">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-166">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="1c1bc-167">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-167">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-168">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-168">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-169">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-169">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="1c1bc-170">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="1c1bc-170">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="1c1bc-171">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-171">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="1c1bc-172">Geral</span><span class="sxs-lookup"><span data-stu-id="1c1bc-172">General</span></span>
* <span data-ttu-id="1c1bc-173">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-173">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-174">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-174">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-175">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-175">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="1c1bc-176">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-176">Az.Advisor</span></span>
* <span data-ttu-id="1c1bc-177">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-177">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1c1bc-178">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c1bc-178">Az.Batch</span></span>
* <span data-ttu-id="1c1bc-179">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-179">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="1c1bc-180">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-180">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="1c1bc-181">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-181">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="1c1bc-182">O parâmetro `-ResourceFile` de **New-AzBatchTask** agora assume uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-182">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="1c1bc-183">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-183">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="1c1bc-184">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-184">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="1c1bc-185">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-185">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="1c1bc-186">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-186">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="1c1bc-187">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-187">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="1c1bc-188">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-188">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="1c1bc-189">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-189">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="1c1bc-190">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-190">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="1c1bc-191">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-191">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="1c1bc-192">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-192">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="1c1bc-193">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-193">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="1c1bc-194">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-194">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="1c1bc-195">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-195">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="1c1bc-196">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-196">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="1c1bc-197">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-197">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="1c1bc-198">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-198">This operation is no longer supported.</span></span>
* <span data-ttu-id="1c1bc-199">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-199">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="1c1bc-200">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-200">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="1c1bc-201">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-201">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="1c1bc-202">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-202">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="1c1bc-203">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-203">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="1c1bc-204">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-204">New non-verified images are also now returned.</span></span> <span data-ttu-id="1c1bc-205">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-205">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="1c1bc-206">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-206">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="1c1bc-207">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-207">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="1c1bc-208">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-208">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="1c1bc-209">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-209">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="1c1bc-210">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-210">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="1c1bc-211">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-211">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="1c1bc-212">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-212">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="1c1bc-213">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-213">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="1c1bc-214">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-214">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c1bc-215">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c1bc-215">Az.Cdn</span></span>
* <span data-ttu-id="1c1bc-216">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-216">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="1c1bc-217">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-217">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-218">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-218">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-219">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-219">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="1c1bc-220">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-220">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="1c1bc-221">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-221">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="1c1bc-222">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="1c1bc-222">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="1c1bc-223">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-223">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1c1bc-224">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-224">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="1c1bc-225">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="1c1bc-225">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="1c1bc-226">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-226">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="1c1bc-227">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-227">Breaking changes</span></span>
    - <span data-ttu-id="1c1bc-228">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="1c1bc-228">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="1c1bc-229">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="1c1bc-229">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-230">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-230">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-231">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-231">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-232">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-232">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-233">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="1c1bc-233">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="1c1bc-234">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-234">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="1c1bc-235">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="1c1bc-235">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="1c1bc-236">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="1c1bc-236">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="1c1bc-237">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="1c1bc-237">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="1c1bc-238">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-238">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c1bc-239">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-239">Az.FrontDoor</span></span>
* <span data-ttu-id="1c1bc-240">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-240">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="1c1bc-241">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c1bc-241">Az.HDInsight</span></span>
* <span data-ttu-id="1c1bc-242">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-242">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="1c1bc-243">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-243">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="1c1bc-244">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-244">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="1c1bc-245">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-245">Removed five cmdlets:</span></span>
    - <span data-ttu-id="1c1bc-246">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="1c1bc-246">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="1c1bc-247">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="1c1bc-247">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="1c1bc-248">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="1c1bc-248">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="1c1bc-249">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c1bc-249">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="1c1bc-250">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c1bc-250">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="1c1bc-251">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-251">Added three cmdlets:</span></span>
    - <span data-ttu-id="1c1bc-252">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-252">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="1c1bc-253">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-253">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="1c1bc-254">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-254">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="1c1bc-255">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-255">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="1c1bc-256">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-256">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="1c1bc-257">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-257">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="1c1bc-258">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-258">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="1c1bc-259">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-259">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="1c1bc-260">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-260">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="1c1bc-261">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-261">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="1c1bc-262">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-262">Added some scenario test cases.</span></span>
* <span data-ttu-id="1c1bc-263">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-263">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-264">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-264">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-265">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-265">Breaking changes:</span></span>
    - <span data-ttu-id="1c1bc-266">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-266">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c1bc-267">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-267">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="1c1bc-268">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-268">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c1bc-269">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-269">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="1c1bc-270">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-270">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="1c1bc-271">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-271">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="1c1bc-272">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-272">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="1c1bc-273">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-273">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="1c1bc-274">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-274">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c1bc-275">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-275">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="1c1bc-276">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-276">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c1bc-277">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-277">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-278">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-278">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-279">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-279">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-280">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-280">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="1c1bc-281">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-281">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="1c1bc-282">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-282">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-283">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-283">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-284">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-284">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-285">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-285">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-286">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-286">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-287">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="1c1bc-287">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-288">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-289">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-289">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-290">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-290">Az.Network</span></span>
* <span data-ttu-id="1c1bc-291">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-291">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="1c1bc-292">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-292">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c1bc-293">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-293">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-294">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-294">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-295">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-295">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-296">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-296">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-297">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-297">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="1c1bc-298">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-298">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="1c1bc-299">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-299">New cmdlet:</span></span>
        - <span data-ttu-id="1c1bc-300">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="1c1bc-300">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="1c1bc-301">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-301">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="1c1bc-302">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-302">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="1c1bc-303">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-303">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="1c1bc-304">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-304">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="1c1bc-305">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-305">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="1c1bc-306">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-306">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="1c1bc-307">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-307">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="1c1bc-308">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-308">New cmdlets added:</span></span>
        - <span data-ttu-id="1c1bc-309">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-309">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="1c1bc-310">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-310">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="1c1bc-311">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-311">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="1c1bc-312">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-312">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="1c1bc-313">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-313">Set-AzVirtualHub</span></span>
* <span data-ttu-id="1c1bc-314">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="1c1bc-314">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="1c1bc-315">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-315">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c1bc-316">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="1c1bc-316">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="1c1bc-317">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="1c1bc-317">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="1c1bc-318">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-318">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="1c1bc-319">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-319">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="1c1bc-320">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-320">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="1c1bc-321">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-321">New cmdlets added:</span></span>
        - <span data-ttu-id="1c1bc-322">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-322">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="1c1bc-323">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-323">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c1bc-324">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-324">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c1bc-325">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-325">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c1bc-326">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-326">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c1bc-327">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-327">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c1bc-328">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-328">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="1c1bc-329">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="1c1bc-329">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="1c1bc-330">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-330">New cmdlets added:</span></span>
        - <span data-ttu-id="1c1bc-331">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="1c1bc-331">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="1c1bc-332">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="1c1bc-332">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="1c1bc-333">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="1c1bc-333">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="1c1bc-334">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="1c1bc-334">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="1c1bc-335">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-335">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="1c1bc-336">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-336">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="1c1bc-337">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-337">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c1bc-338">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-338">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="1c1bc-339">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-339">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="1c1bc-340">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="1c1bc-340">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="1c1bc-341">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="1c1bc-341">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="1c1bc-342">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-342">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c1bc-343">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-343">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="1c1bc-344">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-344">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="1c1bc-345">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-345">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="1c1bc-346">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c1bc-346">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="1c1bc-347">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-347">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="1c1bc-348">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-348">New cmdlets added:</span></span>
        - <span data-ttu-id="1c1bc-349">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-349">New-AzIpGroup</span></span>
        - <span data-ttu-id="1c1bc-350">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-350">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="1c1bc-351">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-351">Get-AzIpGroup</span></span>
        - <span data-ttu-id="1c1bc-352">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-352">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-353">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-353">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-354">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-354">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-355">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-355">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-356">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-356">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="1c1bc-357">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-357">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="1c1bc-358">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-358">Removed deprecated aliases:</span></span>
* <span data-ttu-id="1c1bc-359">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-359">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="1c1bc-360">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-360">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="1c1bc-361">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-361">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="1c1bc-362">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="1c1bc-362">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="1c1bc-363">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="1c1bc-363">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="1c1bc-364">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-364">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-365">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-365">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-366">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1c1bc-366">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="1c1bc-367">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-367">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="1c1bc-368">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-368">Set-AzStorageAccount</span></span>
* <span data-ttu-id="1c1bc-369">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="1c1bc-369">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="1c1bc-370">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c1bc-370">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="1c1bc-371">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c1bc-371">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="1c1bc-372">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-372">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="1c1bc-373">Geral</span><span class="sxs-lookup"><span data-stu-id="1c1bc-373">General</span></span>
* <span data-ttu-id="1c1bc-374">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-374">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-375">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-375">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-376">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-376">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-377">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-377">Az.ApiManagement</span></span>
* <span data-ttu-id="1c1bc-378">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-378">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="1c1bc-379">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="1c1bc-379">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-380">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-380">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-381">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-381">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="1c1bc-382">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c1bc-382">Az.Batch</span></span>
* <span data-ttu-id="1c1bc-383">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-383">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-384">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-384">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-385">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-385">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="1c1bc-386">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="1c1bc-386">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="1c1bc-387">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-387">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="1c1bc-388">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-388">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-389">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-389">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-390">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-390">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="1c1bc-391">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-391">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="1c1bc-392">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-392">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-393">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-393">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-394">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="1c1bc-394">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="1c1bc-395">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="1c1bc-395">Az.HealthcareApis</span></span>
* <span data-ttu-id="1c1bc-396">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-396">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="1c1bc-397">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-397">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="1c1bc-398">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="1c1bc-398">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="1c1bc-399">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-399">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-400">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-400">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-401">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="1c1bc-401">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="1c1bc-402">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-402">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-403">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-403">Az.Monitor</span></span>
* <span data-ttu-id="1c1bc-404">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="1c1bc-404">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="1c1bc-405">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-405">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="1c1bc-406">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="1c1bc-406">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="1c1bc-407">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-407">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-408">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-408">Az.Network</span></span>
* <span data-ttu-id="1c1bc-409">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-409">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="1c1bc-410">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c1bc-410">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="1c1bc-411">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-411">New cmdlets added:</span></span>
        - <span data-ttu-id="1c1bc-412">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-412">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="1c1bc-413">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-413">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="1c1bc-414">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="1c1bc-414">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="1c1bc-415">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-415">Updated cmdlets:</span></span>
        - <span data-ttu-id="1c1bc-416">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-416">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c1bc-417">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-417">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c1bc-418">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-418">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="1c1bc-419">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="1c1bc-419">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="1c1bc-420">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="1c1bc-420">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="1c1bc-421">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-421">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="1c1bc-422">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-422">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c1bc-423">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c1bc-423">Az.RedisCache</span></span>
* <span data-ttu-id="1c1bc-424">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-424">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-425">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-425">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-426">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="1c1bc-426">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-427">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-427">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-428">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-428">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="1c1bc-429">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="1c1bc-429">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="1c1bc-430">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="1c1bc-430">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="1c1bc-431">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="1c1bc-431">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="1c1bc-432">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-432">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="1c1bc-433">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="1c1bc-433">Az.StorageSync</span></span>
* <span data-ttu-id="1c1bc-434">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-434">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-435">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-435">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-436">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="1c1bc-436">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="1c1bc-437">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-437">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-438">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-438">Az.ApiManagement</span></span>
* <span data-ttu-id="1c1bc-439">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-439">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="1c1bc-440">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-440">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="1c1bc-441">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-441">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-442">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-442">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-443">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-443">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="1c1bc-444">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="1c1bc-444">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="1c1bc-445">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-445">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-446">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-446">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-447">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-447">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="1c1bc-448">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-448">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1c1bc-449">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-449">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="1c1bc-450">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-450">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="1c1bc-451">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-451">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="1c1bc-452">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-452">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="1c1bc-453">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-453">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="1c1bc-454">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-454">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="1c1bc-455">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-455">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-456">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-456">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-457">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-457">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="1c1bc-458">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="1c1bc-458">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="1c1bc-459">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c1bc-459">Az.HDInsight</span></span>
* <span data-ttu-id="1c1bc-460">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-460">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-461">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-461">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-462">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-462">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="1c1bc-463">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-463">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="1c1bc-464">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-464">New cmdlets are:</span></span>
    - <span data-ttu-id="1c1bc-465">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c1bc-465">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="1c1bc-466">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c1bc-466">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="1c1bc-467">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c1bc-467">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="1c1bc-468">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c1bc-468">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-469">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-469">Az.Monitor</span></span>
* <span data-ttu-id="1c1bc-470">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="1c1bc-470">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="1c1bc-471">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-471">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="1c1bc-472">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-472">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="1c1bc-473">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-473">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="1c1bc-474">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-474">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="1c1bc-475">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-475">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="1c1bc-476">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-476">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="1c1bc-477">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-477">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="1c1bc-478">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-478">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="1c1bc-479">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-479">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="1c1bc-480">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-480">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="1c1bc-481">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-481">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="1c1bc-482">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-482">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="1c1bc-483">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="1c1bc-483">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="1c1bc-484">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="1c1bc-484">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="1c1bc-485">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-485">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="1c1bc-486">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-486">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="1c1bc-487">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-487">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="1c1bc-488">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-488">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="1c1bc-489">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-489">Overall improved help files</span></span>
* <span data-ttu-id="1c1bc-490">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-490">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-491">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-491">Az.Network</span></span>
* <span data-ttu-id="1c1bc-492">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-492">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="1c1bc-493">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="1c1bc-493">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="1c1bc-494">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="1c1bc-494">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="1c1bc-495">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-495">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="1c1bc-496">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="1c1bc-496">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="1c1bc-497">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="1c1bc-497">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="1c1bc-498">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-498">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="1c1bc-499">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="1c1bc-499">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="1c1bc-500">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-500">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="1c1bc-501">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-501">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="1c1bc-502">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c1bc-502">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="1c1bc-503">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="1c1bc-503">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="1c1bc-504">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-504">New cmdlets</span></span>
        - <span data-ttu-id="1c1bc-505">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="1c1bc-505">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="1c1bc-506">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-506">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="1c1bc-507">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-507">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c1bc-508">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="1c1bc-508">New-VpnSite</span></span>
        - <span data-ttu-id="1c1bc-509">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="1c1bc-509">Update-VpnSite</span></span>
        - <span data-ttu-id="1c1bc-510">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-510">New-VpnConnection</span></span>
        - <span data-ttu-id="1c1bc-511">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-511">Update-VpnConnection</span></span>
* <span data-ttu-id="1c1bc-512">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-512">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-513">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-513">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-514">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-514">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="1c1bc-515">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="1c1bc-515">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-516">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-516">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-517">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-517">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-518">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-518">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-519">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-519">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="1c1bc-520">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-520">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="1c1bc-521">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c1bc-521">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c1bc-522">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-522">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="1c1bc-523">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1c1bc-523">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="1c1bc-524">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-524">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="1c1bc-525">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c1bc-525">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c1bc-526">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c1bc-526">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c1bc-527">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-527">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="1c1bc-528">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1c1bc-528">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="1c1bc-529">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-529">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="1c1bc-530">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c1bc-530">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c1bc-531">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-531">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="1c1bc-532">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1c1bc-532">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="1c1bc-533">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="1c1bc-533">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="1c1bc-534">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-534">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1c1bc-535">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1c1bc-535">Az.SignalR</span></span>
* <span data-ttu-id="1c1bc-536">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-536">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-537">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-537">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-538">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-538">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="1c1bc-539">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-539">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="1c1bc-540">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-540">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="1c1bc-541">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-541">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="1c1bc-542">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-542">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-543">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-543">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-544">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-544">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="1c1bc-545">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="1c1bc-545">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="1c1bc-546">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-546">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="1c1bc-547">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-547">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="1c1bc-548">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-548">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="1c1bc-549">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-549">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="1c1bc-550">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="1c1bc-550">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="1c1bc-551">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c1bc-551">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="1c1bc-552">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c1bc-552">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="1c1bc-553">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c1bc-553">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="1c1bc-554">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c1bc-554">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-555">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-555">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-556">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="1c1bc-556">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="1c1bc-557">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="1c1bc-557">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="1c1bc-558">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-558">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="1c1bc-559">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-559">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="1c1bc-560">Geral</span><span class="sxs-lookup"><span data-stu-id="1c1bc-560">General</span></span>
* <span data-ttu-id="1c1bc-561">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-561">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-562">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-562">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-563">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-563">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="1c1bc-564">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="1c1bc-564">Az.Aks</span></span>
* <span data-ttu-id="1c1bc-565">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-565">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="1c1bc-566">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="1c1bc-566">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-567">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-567">Az.ApiManagement</span></span>
* <span data-ttu-id="1c1bc-568">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="1c1bc-568">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="1c1bc-569">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-569">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="1c1bc-570">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-570">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="1c1bc-571">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="1c1bc-571">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="1c1bc-572">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-572">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1c1bc-573">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c1bc-573">Az.Batch</span></span>
* <span data-ttu-id="1c1bc-574">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="1c1bc-574">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c1bc-575">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c1bc-575">Az.Cdn</span></span>
* <span data-ttu-id="1c1bc-576">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="1c1bc-576">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-577">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-577">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-578">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-578">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="1c1bc-579">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-579">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="1c1bc-580">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-580">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="1c1bc-581">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-581">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="1c1bc-582">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="1c1bc-582">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="1c1bc-583">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-583">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="1c1bc-584">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="1c1bc-584">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="1c1bc-585">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-585">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-586">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-586">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-587">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-587">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="1c1bc-588">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-588">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="1c1bc-589">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="1c1bc-589">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="1c1bc-590">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="1c1bc-590">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-591">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-591">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-592">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-592">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c1bc-593">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-593">Az.EventHub</span></span>
* <span data-ttu-id="1c1bc-594">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-594">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="1c1bc-595">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="1c1bc-595">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="1c1bc-596">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="1c1bc-596">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="1c1bc-597">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="1c1bc-597">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="1c1bc-598">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1c1bc-598">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="1c1bc-599">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-599">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-600">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-600">Az.Monitor</span></span>
* <span data-ttu-id="1c1bc-601">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-601">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-602">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-602">Az.Network</span></span>
* <span data-ttu-id="1c1bc-603">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-603">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="1c1bc-604">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-604">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="1c1bc-605">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-605">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="1c1bc-606">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-606">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="1c1bc-607">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-607">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="1c1bc-608">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-608">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="1c1bc-609">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="1c1bc-609">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-610">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-610">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c1bc-611">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-611">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="1c1bc-612">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-612">Added example</span></span>
    - <span data-ttu-id="1c1bc-613">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-613">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="1c1bc-614">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="1c1bc-614">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="1c1bc-615">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="1c1bc-615">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-616">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-616">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-617">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-617">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-618">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-618">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-619">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="1c1bc-619">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="1c1bc-620">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="1c1bc-620">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="1c1bc-621">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-621">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="1c1bc-622">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-622">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c1bc-623">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-623">Az.ServiceBus</span></span>
* <span data-ttu-id="1c1bc-624">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-624">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="1c1bc-625">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="1c1bc-625">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="1c1bc-626">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="1c1bc-626">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-627">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-627">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-628">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-628">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="1c1bc-629">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-629">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="1c1bc-630">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="1c1bc-630">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="1c1bc-631">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-631">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="1c1bc-632">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="1c1bc-632">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="1c1bc-633">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1bc-633">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-634">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-634">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-635">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-635">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-636">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-636">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-637">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-637">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="1c1bc-638">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="1c1bc-638">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="1c1bc-639">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-639">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="1c1bc-640">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-640">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="1c1bc-641">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="1c1bc-641">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="1c1bc-642">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-642">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-643">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-643">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-644">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="1c1bc-644">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="1c1bc-645">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-645">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-646">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-646">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-647">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c1bc-647">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="1c1bc-648">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-648">Az.ApplicationInsights</span></span>
* <span data-ttu-id="1c1bc-649">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-649">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-650">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-650">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-651">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-651">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c1bc-652">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-652">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c1bc-653">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-653">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-654">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-654">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-655">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-655">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="1c1bc-656">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1c1bc-656">Az.ContainerRegistry</span></span>
* <span data-ttu-id="1c1bc-657">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-657">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="1c1bc-658">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="1c1bc-658">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-659">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-659">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-660">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-660">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="1c1bc-661">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-661">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c1bc-662">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-662">Az.EventHub</span></span>
* <span data-ttu-id="1c1bc-663">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="1c1bc-663">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="1c1bc-664">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="1c1bc-664">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c1bc-665">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-665">Az.KeyVault</span></span>
* <span data-ttu-id="1c1bc-666">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-666">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c1bc-667">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-667">Az.LogicApp</span></span>
* <span data-ttu-id="1c1bc-668">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="1c1bc-668">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="1c1bc-669">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="1c1bc-669">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="1c1bc-670">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-670">Az.ManagedServices</span></span>
* <span data-ttu-id="1c1bc-671">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-671">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-672">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-672">Az.Network</span></span>
* <span data-ttu-id="1c1bc-673">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-673">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="1c1bc-674">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-674">New cmdlets</span></span>
        - <span data-ttu-id="1c1bc-675">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c1bc-675">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c1bc-676">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-676">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="1c1bc-677">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-677">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-678">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-678">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-679">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-679">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-680">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-680">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c1bc-681">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="1c1bc-681">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="1c1bc-682">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-682">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="1c1bc-683">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="1c1bc-683">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="1c1bc-684">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-684">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="1c1bc-685">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-685">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="1c1bc-686">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-686">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="1c1bc-687">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="1c1bc-687">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="1c1bc-688">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="1c1bc-688">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="1c1bc-689">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-689">Updated cmdlets</span></span>
        - <span data-ttu-id="1c1bc-690">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-690">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c1bc-691">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-691">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c1bc-692">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-692">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="1c1bc-693">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-693">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="1c1bc-694">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-694">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="1c1bc-695">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-695">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c1bc-696">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-696">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="1c1bc-697">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-697">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="1c1bc-698">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-698">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="1c1bc-699">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-699">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="1c1bc-700">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-700">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="1c1bc-701">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-701">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-702">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-702">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c1bc-703">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-703">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="1c1bc-704">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-704">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-705">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-705">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-706">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-706">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="1c1bc-707">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-707">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="1c1bc-708">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-708">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="1c1bc-709">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-709">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="1c1bc-710">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-710">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="1c1bc-711">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-711">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="1c1bc-712">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-712">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="1c1bc-713">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-713">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="1c1bc-714">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-714">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="1c1bc-715">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-715">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-716">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-716">Az.Resources</span></span>
- <span data-ttu-id="1c1bc-717">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-717">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="1c1bc-718">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="1c1bc-718">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c1bc-719">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-719">Az.ServiceBus</span></span>
* <span data-ttu-id="1c1bc-720">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="1c1bc-720">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="1c1bc-721">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="1c1bc-721">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-722">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-722">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-723">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="1c1bc-723">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="1c1bc-724">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="1c1bc-724">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="1c1bc-725">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-725">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-726">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-726">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-727">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="1c1bc-727">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="1c1bc-728">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="1c1bc-728">Az.StorageSync</span></span>
* <span data-ttu-id="1c1bc-729">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-729">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="1c1bc-730">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="1c1bc-730">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-731">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-731">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-732">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-732">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="1c1bc-733">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-733">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="1c1bc-734">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-734">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="1c1bc-735">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-735">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-736">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-736">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-737">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="1c1bc-737">Add support for profile cmdlets</span></span>
* <span data-ttu-id="1c1bc-738">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-738">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="1c1bc-739">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="1c1bc-739">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="1c1bc-740">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-740">Az.Advisor</span></span>
* <span data-ttu-id="1c1bc-741">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-741">GA release of Az.Advisor</span></span>
* <span data-ttu-id="1c1bc-742">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-742">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-743">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-743">Az.ApiManagement</span></span>
* <span data-ttu-id="1c1bc-744">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="1c1bc-744">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="1c1bc-745">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-745">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="1c1bc-746">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="1c1bc-746">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="1c1bc-747">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-747">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="1c1bc-748">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="1c1bc-748">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="1c1bc-749">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-749">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="1c1bc-750">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="1c1bc-750">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-751">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-751">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-752">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-752">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-753">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-753">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-754">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-754">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-755">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-755">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-756">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-756">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c1bc-757">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c1bc-757">Az.EventGrid</span></span>
* <span data-ttu-id="1c1bc-758">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-758">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-759">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-759">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-760">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-760">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-761">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-761">Az.Network</span></span>
* <span data-ttu-id="1c1bc-762">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="1c1bc-762">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="1c1bc-763">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-763">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c1bc-764">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-764">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c1bc-765">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="1c1bc-765">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="1c1bc-766">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="1c1bc-766">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-767">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-767">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c1bc-768">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="1c1bc-768">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-769">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-769">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-770">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="1c1bc-770">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-771">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-771">Az.Resources</span></span>
    - <span data-ttu-id="1c1bc-772">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="1c1bc-772">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="1c1bc-773">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="1c1bc-773">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="1c1bc-774">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-774">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="1c1bc-775">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="1c1bc-775">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c1bc-776">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-776">Az.ServiceBus</span></span>
* <span data-ttu-id="1c1bc-777">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-777">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-778">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-778">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-779">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="1c1bc-779">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="1c1bc-780">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-780">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="1c1bc-781">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-781">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="1c1bc-782">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-782">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="1c1bc-783">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-783">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="1c1bc-784">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-784">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="1c1bc-785">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-785">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="1c1bc-786">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-786">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="1c1bc-787">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="1c1bc-787">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-788">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-788">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-789">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-789">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="1c1bc-790">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1c1bc-790">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="1c1bc-791">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-791">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="1c1bc-792">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="1c1bc-792">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="1c1bc-793">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-793">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="1c1bc-794">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-794">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="1c1bc-795">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-795">Set-AzStorageAccount</span></span>
* <span data-ttu-id="1c1bc-796">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="1c1bc-796">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="1c1bc-797">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c1bc-797">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="1c1bc-798">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c1bc-798">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="1c1bc-799">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="1c1bc-799">Az.StorageSync</span></span>
* <span data-ttu-id="1c1bc-800">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-800">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="1c1bc-801">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-801">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-802">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-802">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-803">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="1c1bc-803">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="1c1bc-804">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="1c1bc-804">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="1c1bc-805">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="1c1bc-805">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="1c1bc-806">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="1c1bc-806">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="1c1bc-807">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="1c1bc-807">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-808">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-808">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-809">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-809">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="1c1bc-810">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-810">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="1c1bc-811">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="1c1bc-811">Az.Dns</span></span>
* <span data-ttu-id="1c1bc-812">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-812">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c1bc-813">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c1bc-813">Az.EventGrid</span></span>
* <span data-ttu-id="1c1bc-814">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-814">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="1c1bc-815">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-815">New cmdlets:</span></span>
    - <span data-ttu-id="1c1bc-816">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="1c1bc-816">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="1c1bc-817">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-817">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="1c1bc-818">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="1c1bc-818">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="1c1bc-819">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-819">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="1c1bc-820">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="1c1bc-820">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="1c1bc-821">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-821">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="1c1bc-822">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="1c1bc-822">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="1c1bc-823">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-823">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="1c1bc-824">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="1c1bc-824">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="1c1bc-825">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-825">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="1c1bc-826">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-826">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="1c1bc-827">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-827">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="1c1bc-828">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="1c1bc-828">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="1c1bc-829">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="1c1bc-829">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="1c1bc-830">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-830">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="1c1bc-831">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-831">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="1c1bc-832">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-832">Updated cmdlets:</span></span>
    - <span data-ttu-id="1c1bc-833">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-833">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="1c1bc-834">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-834">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="1c1bc-835">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-835">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="1c1bc-836">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-836">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="1c1bc-837">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-837">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="1c1bc-838">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="1c1bc-838">Event subscription expiration date,</span></span>
            - <span data-ttu-id="1c1bc-839">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-839">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="1c1bc-840">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-840">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="1c1bc-841">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="1c1bc-841">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="1c1bc-842">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-842">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="1c1bc-843">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-843">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="1c1bc-844">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="1c1bc-844">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="1c1bc-845">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-845">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="1c1bc-846">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-846">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c1bc-847">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-847">Az.FrontDoor</span></span>
* <span data-ttu-id="1c1bc-848">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-848">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="1c1bc-849">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-849">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="1c1bc-850">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-850">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="1c1bc-851">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="1c1bc-851">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-852">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-852">Az.Network</span></span>
* <span data-ttu-id="1c1bc-853">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c1bc-853">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="1c1bc-854">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-854">New cmdlets</span></span>
        - <span data-ttu-id="1c1bc-855">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="1c1bc-855">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="1c1bc-856">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-856">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="1c1bc-857">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-857">New cmdlets</span></span> 
        - <span data-ttu-id="1c1bc-858">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="1c1bc-858">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="1c1bc-859">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-859">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="1c1bc-860">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-860">New cmdlets</span></span> 
        - <span data-ttu-id="1c1bc-861">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-861">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="1c1bc-862">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-862">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="1c1bc-863">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-863">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="1c1bc-864">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-864">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="1c1bc-865">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-865">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="1c1bc-866">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c1bc-866">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="1c1bc-867">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-867">New cmdlets</span></span>
        - <span data-ttu-id="1c1bc-868">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c1bc-868">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c1bc-869">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c1bc-869">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c1bc-870">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c1bc-870">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c1bc-871">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-871">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="1c1bc-872">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-872">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="1c1bc-873">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-873">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="1c1bc-874">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-874">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="1c1bc-875">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-875">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="1c1bc-876">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-876">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="1c1bc-877">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="1c1bc-877">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="1c1bc-878">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-878">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="1c1bc-879">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-879">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="1c1bc-880">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-880">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="1c1bc-881">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="1c1bc-881">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="1c1bc-882">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-882">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="1c1bc-883">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-883">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="1c1bc-884">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="1c1bc-884">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="1c1bc-885">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c1bc-885">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="1c1bc-886">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-886">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="1c1bc-887">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="1c1bc-887">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="1c1bc-888">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c1bc-888">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="1c1bc-889">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-889">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="1c1bc-890">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="1c1bc-890">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="1c1bc-891">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-891">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="1c1bc-892">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-892">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="1c1bc-893">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-893">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="1c1bc-894">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-894">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-895">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-895">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c1bc-896">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-896">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-897">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-897">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-898">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-898">Support for additional Template Export options</span></span>
    - <span data-ttu-id="1c1bc-899">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-899">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="1c1bc-900">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-900">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="1c1bc-901">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-901">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-902">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-902">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-903">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-903">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-904">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-904">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-905">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-905">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="1c1bc-906">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-906">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="1c1bc-907">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-907">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="1c1bc-908">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="1c1bc-908">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="1c1bc-909">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="1c1bc-909">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="1c1bc-910">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="1c1bc-910">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="1c1bc-911">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="1c1bc-911">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="1c1bc-912">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="1c1bc-912">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-913">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-913">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-914">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1c1bc-914">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="1c1bc-915">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-915">New-AzStorageAccount</span></span>
* <span data-ttu-id="1c1bc-916">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="1c1bc-916">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="1c1bc-917">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-917">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-918">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-918">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-919">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="1c1bc-919">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="1c1bc-920">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="1c1bc-920">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="1c1bc-921">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-921">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="1c1bc-922">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c1bc-922">Az.Cdn</span></span>
* <span data-ttu-id="1c1bc-923">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-923">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-924">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-924">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-925">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-925">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="1c1bc-926">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-926">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c1bc-927">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-927">Az.EventHub</span></span>
* <span data-ttu-id="1c1bc-928">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-928">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="1c1bc-929">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="1c1bc-929">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-930">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-930">Az.Network</span></span>
* <span data-ttu-id="1c1bc-931">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-931">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="1c1bc-932">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="1c1bc-932">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c1bc-933">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-933">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c1bc-934">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-934">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-935">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-935">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-936">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="1c1bc-936">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c1bc-937">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-937">Az.ServiceBus</span></span>
* <span data-ttu-id="1c1bc-938">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="1c1bc-938">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-939">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-939">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-940">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-940">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="1c1bc-941">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-941">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-942">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-942">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-943">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-943">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="1c1bc-944">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-944">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="1c1bc-945">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-945">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="1c1bc-946">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-946">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-947">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-947">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-948">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-948">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="1c1bc-949">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-949">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-950">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-950">Az.ApiManagement</span></span>
* <span data-ttu-id="1c1bc-951">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-951">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="1c1bc-952">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-952">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="1c1bc-953">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-953">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="1c1bc-954">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-954">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="1c1bc-955">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-955">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="1c1bc-956">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="1c1bc-956">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="1c1bc-957">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-957">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="1c1bc-958">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-958">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="1c1bc-959">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-959">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="1c1bc-960">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="1c1bc-960">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="1c1bc-961">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="1c1bc-961">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="1c1bc-962">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="1c1bc-962">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="1c1bc-963">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="1c1bc-963">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="1c1bc-964">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-964">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="1c1bc-965">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-965">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="1c1bc-966">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-966">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="1c1bc-967">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-967">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="1c1bc-968">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="1c1bc-968">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="1c1bc-969">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-969">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="1c1bc-970">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="1c1bc-970">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="1c1bc-971">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="1c1bc-971">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="1c1bc-972">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-972">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="1c1bc-973">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-973">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="1c1bc-974">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-974">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="1c1bc-975">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-975">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="1c1bc-976">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-976">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="1c1bc-977">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-977">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="1c1bc-978">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-978">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="1c1bc-979">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-979">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="1c1bc-980">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-980">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="1c1bc-981">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="1c1bc-981">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="1c1bc-982">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="1c1bc-982">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="1c1bc-983">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-983">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="1c1bc-984">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-984">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="1c1bc-985">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-985">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="1c1bc-986">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="1c1bc-986">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="1c1bc-987">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-987">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="1c1bc-988">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-988">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="1c1bc-989">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-989">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="1c1bc-990">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-990">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="1c1bc-991">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-991">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="1c1bc-992">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-992">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="1c1bc-993">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-993">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="1c1bc-994">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-994">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="1c1bc-995">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-995">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="1c1bc-996">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-996">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="1c1bc-997">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-997">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="1c1bc-998">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-998">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="1c1bc-999">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-999">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="1c1bc-1000">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1000">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="1c1bc-1001">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1001">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="1c1bc-1002">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1002">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="1c1bc-1003">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1003">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="1c1bc-1004">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1004">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="1c1bc-1005">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1005">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="1c1bc-1006">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1006">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="1c1bc-1007">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1007">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="1c1bc-1008">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1008">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="1c1bc-1009">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1009">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="1c1bc-1010">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1010">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="1c1bc-1011">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1011">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="1c1bc-1012">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1012">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="1c1bc-1013">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1013">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="1c1bc-1014">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1014">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="1c1bc-1015">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1015">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="1c1bc-1016">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1016">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="1c1bc-1017">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1017">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="1c1bc-1018">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1018">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="1c1bc-1019">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1019">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="1c1bc-1020">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1020">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="1c1bc-1021">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1021">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="1c1bc-1022">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1022">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="1c1bc-1023">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1023">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="1c1bc-1024">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1024">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="1c1bc-1025">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1025">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="1c1bc-1026">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1026">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="1c1bc-1027">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1027">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-1028">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1028">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1029">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1029">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="1c1bc-1030">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1030">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="1c1bc-1031">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1031">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="1c1bc-1032">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1032">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="1c1bc-1033">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1033">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="1c1bc-1034">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1034">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="1c1bc-1035">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1035">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1036">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1036">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1037">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1037">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="1c1bc-1038">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1038">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1039">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1039">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1040">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1040">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-1041">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1041">Az.Monitor</span></span>
* <span data-ttu-id="1c1bc-1042">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1042">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1043">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1043">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1044">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1044">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="1c1bc-1045">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1045">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c1bc-1046">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1046">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="1c1bc-1047">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1047">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1048">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1048">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1049">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1049">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1050">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1050">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1051">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1051">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="1c1bc-1052">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1052">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1053">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1053">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1054">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1054">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c1bc-1055">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1055">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c1bc-1056">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1056">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="1c1bc-1057">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1057">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1058">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1058">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1059">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1059">Proximity placement group feature.</span></span>
    - <span data-ttu-id="1c1bc-1060">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1060">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="1c1bc-1061">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1061">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="1c1bc-1062">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1062">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="1c1bc-1063">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1063">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="1c1bc-1064">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1064">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="1c1bc-1065">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1065">Breaking changes</span></span>
    - <span data-ttu-id="1c1bc-1066">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1066">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="1c1bc-1067">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1067">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="1c1bc-1068">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1068">Az.DeploymentManager</span></span>
* <span data-ttu-id="1c1bc-1069">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1069">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="1c1bc-1070">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1070">Az.Dns</span></span>
* <span data-ttu-id="1c1bc-1071">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1071">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="1c1bc-1072">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1072">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="1c1bc-1073">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1073">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c1bc-1074">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1074">Az.FrontDoor</span></span>
* <span data-ttu-id="1c1bc-1075">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1075">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="1c1bc-1076">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1076">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="1c1bc-1077">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1077">Az.HDInsight</span></span>
* <span data-ttu-id="1c1bc-1078">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1078">Removed two cmdlets:</span></span>
    - <span data-ttu-id="1c1bc-1079">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1079">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="1c1bc-1080">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1080">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="1c1bc-1081">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1081">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="1c1bc-1082">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1082">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="1c1bc-1083">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1083">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="1c1bc-1084">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1084">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-1085">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1085">Az.Monitor</span></span>
* <span data-ttu-id="1c1bc-1086">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1086">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="1c1bc-1087">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1087">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="1c1bc-1088">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1088">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="1c1bc-1089">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1089">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="1c1bc-1090">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1090">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="1c1bc-1091">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1091">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="1c1bc-1092">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1092">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="1c1bc-1093">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1093">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c1bc-1094">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1094">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c1bc-1095">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1095">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c1bc-1096">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1096">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c1bc-1097">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1097">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c1bc-1098">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1098">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="1c1bc-1099">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1099">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1100">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1100">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1101">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1101">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="1c1bc-1102">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1102">New cmdlets</span></span>
        - <span data-ttu-id="1c1bc-1103">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1103">New-AzNatGateway</span></span>
        - <span data-ttu-id="1c1bc-1104">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1104">Get-AzNatGateway</span></span>
        - <span data-ttu-id="1c1bc-1105">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1105">Set-AzNatGateway</span></span>
        - <span data-ttu-id="1c1bc-1106">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1106">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="1c1bc-1107">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1107">Updated cmdlets</span></span>
        - <span data-ttu-id="1c1bc-1108">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1108">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="1c1bc-1109">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1109">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="1c1bc-1110">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1110">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="1c1bc-1111">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1111">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="1c1bc-1112">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1112">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c1bc-1113">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1113">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c1bc-1114">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1114">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="1c1bc-1115">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1115">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="1c1bc-1116">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1116">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1117">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1117">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-1118">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1118">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="1c1bc-1119">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1119">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="1c1bc-1120">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1120">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="1c1bc-1121">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1121">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="1c1bc-1122">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1122">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="1c1bc-1123">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1123">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="1c1bc-1124">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1124">Az.Relay</span></span>
* <span data-ttu-id="1c1bc-1125">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1125">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c1bc-1126">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1126">Az.ServiceBus</span></span>
* <span data-ttu-id="1c1bc-1127">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1127">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-1128">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1128">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-1129">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1129">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="1c1bc-1130">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1130">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="1c1bc-1131">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1131">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="1c1bc-1132">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1132">New-AzStorageAccount</span></span>
* <span data-ttu-id="1c1bc-1133">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1133">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="1c1bc-1134">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1134">New-AzStorageAccount</span></span>
    - <span data-ttu-id="1c1bc-1135">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1135">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="1c1bc-1136">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1136">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1137">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1137">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1138">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1138">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="1c1bc-1139">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1139">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="1c1bc-1140">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1140">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c1bc-1141">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1141">Highlights since the last major release</span></span>
* <span data-ttu-id="1c1bc-1142">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1142">General availability of `Az` module</span></span>
* <span data-ttu-id="1c1bc-1143">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1143">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1c1bc-1144">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1144">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1c1bc-1145">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1145">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1c1bc-1146">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1146">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c1bc-1147">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1147">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1148">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1148">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1149">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1150">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1150">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1c1bc-1151">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1151">Az.Batch</span></span>
* <span data-ttu-id="1c1bc-1152">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1152">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c1bc-1153">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1153">Az.Cdn</span></span>
* <span data-ttu-id="1c1bc-1154">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1154">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c1bc-1155">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1155">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c1bc-1156">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1156">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1157">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1157">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1158">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1158">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="1c1bc-1159">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1159">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c1bc-1160">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1160">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-1161">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1161">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-1162">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1162">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1163">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1163">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1164">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1164">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c1bc-1165">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1165">Az.EventGrid</span></span>
* <span data-ttu-id="1c1bc-1166">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1166">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c1bc-1167">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1167">Az.EventHub</span></span>
* <span data-ttu-id="1c1bc-1168">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1168">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="1c1bc-1169">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1169">Az.HDInsight</span></span>
* <span data-ttu-id="1c1bc-1170">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1170">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-1171">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1171">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-1172">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1172">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c1bc-1173">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1173">Az.KeyVault</span></span>
* <span data-ttu-id="1c1bc-1174">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1174">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c1bc-1175">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1175">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="1c1bc-1176">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1176">Az.MachineLearning</span></span>
* <span data-ttu-id="1c1bc-1177">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1177">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="1c1bc-1178">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1178">Az.Media</span></span>
* <span data-ttu-id="1c1bc-1179">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1179">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-1180">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1180">Az.Monitor</span></span>
  * <span data-ttu-id="1c1bc-1181">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1181">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="1c1bc-1182">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1182">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="1c1bc-1183">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1183">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="1c1bc-1184">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1184">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1c1bc-1185">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1185">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1c1bc-1186">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1186">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="1c1bc-1187">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1187">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1188">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1188">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1189">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1189">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c1bc-1190">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1190">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="1c1bc-1191">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1191">Az.NotificationHubs</span></span>
* <span data-ttu-id="1c1bc-1192">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1192">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-1193">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1193">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c1bc-1194">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1194">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="1c1bc-1195">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1195">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="1c1bc-1196">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1196">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1197">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1197">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-1198">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1198">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c1bc-1199">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1199">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="1c1bc-1200">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1200">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="1c1bc-1201">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1201">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c1bc-1202">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1202">Az.RedisCache</span></span>
* <span data-ttu-id="1c1bc-1203">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1204">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1204">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1205">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1205">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1206">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1206">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1207">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1207">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="1c1bc-1208">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c1bc-1209">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1209">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="1c1bc-1210">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1210">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="1c1bc-1211">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1211">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="1c1bc-1212">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1212">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="1c1bc-1213">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1213">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1214">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1214">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1215">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1215">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="1c1bc-1216">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1216">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c1bc-1217">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1217">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="1c1bc-1218">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1218">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="1c1bc-1219">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1219">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c1bc-1220">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1220">Highlights since the last major release</span></span>
* <span data-ttu-id="1c1bc-1221">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1221">General availability of `Az` module</span></span>
* <span data-ttu-id="1c1bc-1222">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1222">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1c1bc-1223">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1223">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1c1bc-1224">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1224">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1c1bc-1225">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1225">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c1bc-1226">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1226">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1227">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1227">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1228">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1228">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1229">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1229">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1c1bc-1230">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1230">Az.AnalysisServices</span></span>
* <span data-ttu-id="1c1bc-1231">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1231">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="1c1bc-1232">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1232">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-1233">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1233">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1234">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1234">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="1c1bc-1235">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1235">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="1c1bc-1236">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1236">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1237">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1237">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1238">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1238">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1c1bc-1239">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1239">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="1c1bc-1240">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1240">Az.ContainerInstance</span></span>
* <span data-ttu-id="1c1bc-1241">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1241">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-1242">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1242">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-1243">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1243">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="1c1bc-1244">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1244">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1245">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1245">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1246">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1246">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="1c1bc-1247">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1247">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="1c1bc-1248">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1248">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="1c1bc-1249">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1249">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="1c1bc-1250">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1250">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="1c1bc-1251">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1251">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1252">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1252">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1253">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1253">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-1254">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1254">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-1255">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1255">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="1c1bc-1256">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1256">New-AzStorageContext</span></span>
* <span data-ttu-id="1c1bc-1257">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1257">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="1c1bc-1258">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1258">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1c1bc-1259">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1259">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1c1bc-1260">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1260">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="1c1bc-1261">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1261">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="1c1bc-1262">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1262">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="1c1bc-1263">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1263">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1c1bc-1264">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1264">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1c1bc-1265">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1265">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="1c1bc-1266">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1266">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="1c1bc-1267">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1267">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c1bc-1268">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1268">Highlights since the last major release</span></span>
* <span data-ttu-id="1c1bc-1269">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1269">General availability of `Az` module</span></span>
* <span data-ttu-id="1c1bc-1270">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1270">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1c1bc-1271">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1271">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1c1bc-1272">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1272">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1c1bc-1273">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1273">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c1bc-1274">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1274">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1275">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1275">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-1276">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1276">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1277">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1277">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="1c1bc-1278">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1278">Dynamic grouping</span></span>
    * <span data-ttu-id="1c1bc-1279">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1279">Pre-Post script</span></span>
    * <span data-ttu-id="1c1bc-1280">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1280">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1281">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1282">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1282">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="1c1bc-1283">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1283">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c1bc-1284">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1284">Az.KeyVault</span></span>
* <span data-ttu-id="1c1bc-1285">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1285">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1286">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1286">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1287">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1287">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="1c1bc-1288">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1288">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1289">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1289">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-1290">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1290">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="1c1bc-1291">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1291">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1292">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1292">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1293">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1293">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="1c1bc-1294">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1294">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1295">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1295">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1296">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1296">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-1297">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1297">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-1298">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1298">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="1c1bc-1299">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1299">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1c1bc-1300">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1300">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1c1bc-1301">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1301">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1c1bc-1302">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1302">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="1c1bc-1303">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1303">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="1c1bc-1304">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1304">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1305">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1305">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1306">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1306">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="1c1bc-1307">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1307">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1308">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1308">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1309">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1309">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="1c1bc-1310">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1310">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-1311">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1311">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1312">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1312">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="1c1bc-1313">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1313">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="1c1bc-1314">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1314">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c1bc-1315">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1315">Az.Cdn</span></span>
* <span data-ttu-id="1c1bc-1316">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1316">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1317">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1317">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1318">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1318">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-1319">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1319">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-1320">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1320">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c1bc-1321">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1321">Az.LogicApp</span></span>
* <span data-ttu-id="1c1bc-1322">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1322">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1323">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1323">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1324">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1324">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1325">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1325">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-1326">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1326">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="1c1bc-1327">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1327">SDK Update</span></span>
* <span data-ttu-id="1c1bc-1328">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1328">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="1c1bc-1329">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1329">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1330">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1330">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1331">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1331">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="1c1bc-1332">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1332">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="1c1bc-1333">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1333">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="1c1bc-1334">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1334">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="1c1bc-1335">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1335">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="1c1bc-1336">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1336">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1337">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1337">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1338">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1338">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="1c1bc-1339">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1339">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-1340">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1340">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-1341">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1341">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="1c1bc-1342">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1342">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="1c1bc-1343">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1343">Az.AnalysisServices</span></span>
* <span data-ttu-id="1c1bc-1344">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1344">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-1345">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1345">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1346">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1346">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="1c1bc-1347">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1347">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="1c1bc-1348">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1348">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c1bc-1349">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1349">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c1bc-1350">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1350">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1351">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1351">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1352">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1352">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="1c1bc-1353">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1353">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="1c1bc-1354">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1354">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="1c1bc-1355">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1355">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1356">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1356">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1357">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1357">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c1bc-1358">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1358">Az.EventHub</span></span>
* <span data-ttu-id="1c1bc-1359">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1359">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="1c1bc-1360">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1360">Az.KeyVault</span></span>
* <span data-ttu-id="1c1bc-1361">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1361">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c1bc-1362">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1362">Az.LogicApp</span></span>
* <span data-ttu-id="1c1bc-1363">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1363">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="1c1bc-1364">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1364">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="1c1bc-1365">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1365">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="1c1bc-1366">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1366">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1c1bc-1367">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1367">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1c1bc-1368">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1368">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1c1bc-1369">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1369">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="1c1bc-1370">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1370">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="1c1bc-1371">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1371">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1c1bc-1372">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1372">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1c1bc-1373">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1373">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1c1bc-1374">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1374">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="1c1bc-1375">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1375">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c1bc-1376">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1376">Az.Monitor</span></span>
* <span data-ttu-id="1c1bc-1377">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1377">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1378">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1378">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1379">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1379">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-1380">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1380">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c1bc-1381">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1381">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="1c1bc-1382">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1382">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="1c1bc-1383">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1383">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1384">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1384">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1385">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1385">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1c1bc-1386">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1386">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="1c1bc-1387">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1387">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="1c1bc-1388">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1388">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1389">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1389">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1390">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1390">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="1c1bc-1391">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1391">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1392">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1392">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1393">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1393">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="1c1bc-1394">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1394">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1395">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1395">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1396">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1396">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1c1bc-1397">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1397">Az.AnalysisServices</span></span>
<span data-ttu-id="1c1bc-1398">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1398">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1399">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1399">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1400">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1400">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="1c1bc-1401">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1401">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="1c1bc-1402">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1402">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1403">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1403">Az.RecoveryServices</span></span>
<span data-ttu-id="1c1bc-1404">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1404">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1405">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1405">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1406">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1406">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="1c1bc-1407">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1407">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1c1bc-1408">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1408">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="1c1bc-1409">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1409">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1410">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1410">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1411">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1411">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="1c1bc-1412">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1412">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="1c1bc-1413">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1413">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="1c1bc-1414">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1414">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1415">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1415">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1416">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1416">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1c1bc-1417">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1417">Az.AnalysisServices</span></span>
* <span data-ttu-id="1c1bc-1418">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1418">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1419">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1419">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c1bc-1420">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1420">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="1c1bc-1421">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1421">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1422">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1422">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1423">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1423">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c1bc-1424">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1424">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c1bc-1425">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1425">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="1c1bc-1426">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1426">Az.Aks</span></span>
* <span data-ttu-id="1c1bc-1427">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1427">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c1bc-1428">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1428">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1429">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1429">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="1c1bc-1430">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1430">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c1bc-1431">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1431">Az.Cdn</span></span>
* <span data-ttu-id="1c1bc-1432">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1432">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1433">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1433">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1434">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1434">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="1c1bc-1435">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1435">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="1c1bc-1436">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1436">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="1c1bc-1437">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1437">Az.ContainerRegistry</span></span>
* <span data-ttu-id="1c1bc-1438">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1438">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c1bc-1439">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1439">Az.DataFactory</span></span>
* <span data-ttu-id="1c1bc-1440">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1440">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1441">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1441">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1442">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1442">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="1c1bc-1443">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1443">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="1c1bc-1444">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1444">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-1445">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1445">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-1446">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1446">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c1bc-1447">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1447">Az.KeyVault</span></span>
* <span data-ttu-id="1c1bc-1448">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1448">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1449">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1449">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1450">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1450">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1451">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1451">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1452">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1452">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="1c1bc-1453">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1453">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="1c1bc-1454">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1454">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="1c1bc-1455">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1455">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="1c1bc-1456">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1456">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="1c1bc-1457">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1457">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="1c1bc-1458">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1458">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-1459">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1459">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-1460">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1460">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="1c1bc-1461">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1461">Fix some error messages.</span></span>
* <span data-ttu-id="1c1bc-1462">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1462">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="1c1bc-1463">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1463">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1c1bc-1464">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1464">Az.SignalR</span></span>
* <span data-ttu-id="1c1bc-1465">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1465">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1466">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1466">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1467">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1467">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c1bc-1468">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1468">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="1c1bc-1469">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1469">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="1c1bc-1470">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1470">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-1471">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1471">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-1472">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1472">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c1bc-1473">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1473">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="1c1bc-1474">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1474">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="1c1bc-1475">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1475">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="1c1bc-1476">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1476">Az.TrafficManager</span></span>
* <span data-ttu-id="1c1bc-1477">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1477">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1478">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1478">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1479">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1479">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c1bc-1480">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1480">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="1c1bc-1481">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1481">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="1c1bc-1482">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1482">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1483">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1483">Az.Accounts</span></span>
* <span data-ttu-id="1c1bc-1484">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1484">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1485">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1485">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1486">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1486">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="1c1bc-1487">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1487">Updated the description of ID in help files</span></span>
* <span data-ttu-id="1c1bc-1488">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1488">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1489">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1489">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1490">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1490">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="1c1bc-1491">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1491">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c1bc-1492">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1492">Az.EventGrid</span></span>
* <span data-ttu-id="1c1bc-1493">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1493">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="1c1bc-1494">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1494">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="1c1bc-1495">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1495">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1c1bc-1496">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1496">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1c1bc-1497">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1497">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1c1bc-1498">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1498">Dead letter endpoint.</span></span>
    - <span data-ttu-id="1c1bc-1499">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1499">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1c1bc-1500">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1500">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1c1bc-1501">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1501">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1c1bc-1502">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1502">Dead letter endpoint.</span></span>
* <span data-ttu-id="1c1bc-1503">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1503">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="1c1bc-1504">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1504">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c1bc-1505">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1505">Az.IotHub</span></span>
* <span data-ttu-id="1c1bc-1506">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1506">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c1bc-1507">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1507">Az.LogicApp</span></span>
* <span data-ttu-id="1c1bc-1508">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1508">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1509">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1509">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1510">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1510">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="1c1bc-1511">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1511">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="1c1bc-1512">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1512">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1c1bc-1513">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1513">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="1c1bc-1514">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1514">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="1c1bc-1515">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1515">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1c1bc-1516">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1516">Az.SignalR</span></span>
* <span data-ttu-id="1c1bc-1517">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1517">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1518">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1518">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1519">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1519">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c1bc-1520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1520">Az.Storage</span></span>
* <span data-ttu-id="1c1bc-1521">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1521">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="1c1bc-1522">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1522">New-AzStorageContext</span></span>
* <span data-ttu-id="1c1bc-1523">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1523">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="1c1bc-1524">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1524">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1525">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1525">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1526">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1526">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="1c1bc-1527">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1527">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="1c1bc-1528">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1528">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="1c1bc-1529">Geral</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1529">General</span></span>

- <span data-ttu-id="1c1bc-1530">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1530">General Availability of Az Module</span></span>
- <span data-ttu-id="1c1bc-1531">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1531">Online help for each module</span></span>
- <span data-ttu-id="1c1bc-1532">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1532">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="1c1bc-1533">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1533">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="1c1bc-1534">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1534">Az.Accounts</span></span>
- <span data-ttu-id="1c1bc-1535">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1535">Changed from Az.Profile</span></span>
- <span data-ttu-id="1c1bc-1536">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1536">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-1537">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1537">Az.ApiManagement</span></span>
- <span data-ttu-id="1c1bc-1538">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1538">Fixes for #7002</span></span>
- <span data-ttu-id="1c1bc-1539">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1539">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="1c1bc-1540">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1540">Az.Batch</span></span>
- <span data-ttu-id="1c1bc-1541">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1541">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="1c1bc-1542">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1542">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="1c1bc-1543">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1543">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="1c1bc-1544">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1544">Az.Billing</span></span>
- <span data-ttu-id="1c1bc-1545">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1545">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="1c1bc-1546">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1546">Az.CognitivServices</span></span>
- <span data-ttu-id="1c1bc-1547">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1547">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="1c1bc-1548">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1548">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1c1bc-1549">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1549">Az.ContainerInstance</span></span>
- <span data-ttu-id="1c1bc-1550">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1550">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="1c1bc-1551">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1551">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="1c1bc-1552">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1552">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1553">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1553">Az.DataLakeStore</span></span>
- <span data-ttu-id="1c1bc-1554">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1554">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="1c1bc-1555">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1555">Az.Monitor</span></span>
- <span data-ttu-id="1c1bc-1556">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1556">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="1c1bc-1557">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1557">Az.KeyVault</span></span>
- <span data-ttu-id="1c1bc-1558">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1558">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="1c1bc-1559">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1559">Az.MachineLearning</span></span>
- <span data-ttu-id="1c1bc-1560">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1560">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="1c1bc-1561">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1561">Az.Media</span></span>
- <span data-ttu-id="1c1bc-1562">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1562">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1563">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1563">Az.Network</span></span>
<span data-ttu-id="1c1bc-1564">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1564">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="1c1bc-1565">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1565">New cmdlets added:</span></span>
        - <span data-ttu-id="1c1bc-1566">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1566">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c1bc-1567">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1567">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c1bc-1568">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1568">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c1bc-1569">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1569">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c1bc-1570">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1570">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c1bc-1571">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1571">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="1c1bc-1572">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1572">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="1c1bc-1573">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1573">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="1c1bc-1574">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1574">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="1c1bc-1575">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1575">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="1c1bc-1576">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1576">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1c1bc-1577">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1577">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1c1bc-1578">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1578">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="1c1bc-1579">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1579">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="1c1bc-1580">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1580">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="1c1bc-1581">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1581">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="1c1bc-1582">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1582">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1c1bc-1583">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1583">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1c1bc-1584">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1584">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="1c1bc-1585">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1585">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="1c1bc-1586">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1586">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="1c1bc-1587">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1587">Az.OperationalInsights</span></span>
- <span data-ttu-id="1c1bc-1588">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1588">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="1c1bc-1589">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1589">Az.Profile</span></span>
- <span data-ttu-id="1c1bc-1590">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1590">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1591">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1591">Az.RecoveryServices</span></span>
- <span data-ttu-id="1c1bc-1592">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1592">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="1c1bc-1593">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1593">Az.Resources</span></span>
- <span data-ttu-id="1c1bc-1594">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1594">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-1595">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1595">Az.ServiceFabric</span></span>
- <span data-ttu-id="1c1bc-1596">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1596">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="1c1bc-1597">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1597">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="1c1bc-1598">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1598">Az.SIgnalR</span></span>
- <span data-ttu-id="1c1bc-1599">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1599">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="1c1bc-1600">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1600">Az.Sql</span></span>
- <span data-ttu-id="1c1bc-1601">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1601">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="1c1bc-1602">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1602">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="1c1bc-1603">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="1c1bc-1604">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1604">Az.Storage</span></span>
- <span data-ttu-id="1c1bc-1605">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1605">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1606">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1606">Az.Websites</span></span>
- <span data-ttu-id="1c1bc-1607">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1607">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="1c1bc-1608">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1608">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="1c1bc-1609">Geral</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1609">General</span></span>

* <span data-ttu-id="1c1bc-1610">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1610">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="1c1bc-1611">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1611">Az.Compute</span></span>

* <span data-ttu-id="1c1bc-1612">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1612">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1613">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1613">Az.DataLakeStore</span></span>

* <span data-ttu-id="1c1bc-1614">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1614">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="1c1bc-1615">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1615">Az.FrontDoor</span></span>

* <span data-ttu-id="1c1bc-1616">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1616">Fixed some broken links</span></span>
    - <span data-ttu-id="1c1bc-1617">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1617">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="1c1bc-1618">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1618">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1c1bc-1619">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1619">Az.RecoveryServices</span></span>

* <span data-ttu-id="1c1bc-1620">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1620">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="1c1bc-1621">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1621">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="1c1bc-1622">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1622">Az.Resources</span></span>

* <span data-ttu-id="1c1bc-1623">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1623">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="1c1bc-1624">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1624">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="1c1bc-1625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1625">Az.Sql</span></span>

* <span data-ttu-id="1c1bc-1626">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1626">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="1c1bc-1627">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1627">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="1c1bc-1628">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1628">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="1c1bc-1629">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1629">Az.Storage</span></span>

* <span data-ttu-id="1c1bc-1630">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1630">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="1c1bc-1631">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1631">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="1c1bc-1632">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1632">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1c1bc-1633">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1633">Support Static Website configuration</span></span>
    - <span data-ttu-id="1c1bc-1634">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1634">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="1c1bc-1635">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1635">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1636">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1636">Az.Websites</span></span>

* <span data-ttu-id="1c1bc-1637">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1637">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="1c1bc-1638">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1638">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="1c1bc-1639">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1639">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="1c1bc-1640">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1640">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1c1bc-1641">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1641">Az.ApiManagement</span></span>
* <span data-ttu-id="1c1bc-1642">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1642">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="1c1bc-1643">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1643">Az.Automation</span></span>
* <span data-ttu-id="1c1bc-1644">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1644">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="1c1bc-1645">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1645">Added Update Management cmdlets</span></span>
* <span data-ttu-id="1c1bc-1646">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1646">Added Source Control cmdlets</span></span>
* <span data-ttu-id="1c1bc-1647">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1647">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="1c1bc-1648">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1648">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="1c1bc-1649">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1649">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1650">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1650">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="1c1bc-1651">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1651">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1c1bc-1652">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1652">Az.ContainerInstance</span></span>
* <span data-ttu-id="1c1bc-1653">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1653">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="1c1bc-1654">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1654">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="1c1bc-1655">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1655">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1656">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1656">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1657">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1657">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="1c1bc-1658">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1658">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="1c1bc-1659">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1659">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="1c1bc-1660">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1660">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="1c1bc-1661">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1661">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1c1bc-1662">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1662">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="1c1bc-1663">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1663">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="1c1bc-1664">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1664">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="1c1bc-1665">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1665">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="1c1bc-1666">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1666">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="1c1bc-1667">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1667">Az.Relay</span></span>
* <span data-ttu-id="1c1bc-1668">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1668">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="1c1bc-1669">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1669">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1670">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1670">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="1c1bc-1671">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1671">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="1c1bc-1672">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1672">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-1673">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1673">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-1674">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1674">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="1c1bc-1675">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1675">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1676">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1676">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="1c1bc-1677">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1677">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c1bc-1678">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1678">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c1bc-1679">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1679">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c1bc-1680">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1680">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c1bc-1681">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1681">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1c1bc-1682">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1682">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1c1bc-1683">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1683">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1c1bc-1684">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1684">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="1c1bc-1685">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1685">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="1c1bc-1686">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1686">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="1c1bc-1687">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1687">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="1c1bc-1688">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1688">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1c1bc-1689">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1689">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1c1bc-1690">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1690">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="1c1bc-1691">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1691">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="1c1bc-1692">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1692">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="1c1bc-1693">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1693">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1c1bc-1694">Geral</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1694">General</span></span>
* <span data-ttu-id="1c1bc-1695">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1695">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="1c1bc-1696">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1696">Az.Profile</span></span>
* <span data-ttu-id="1c1bc-1697">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1697">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="1c1bc-1698">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1698">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="1c1bc-1699">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1699">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="1c1bc-1700">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1700">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="1c1bc-1701">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1701">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="1c1bc-1702">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1702">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="1c1bc-1703">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1703">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c1bc-1704">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1704">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c1bc-1705">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1705">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1706">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1706">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1707">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1707">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="1c1bc-1708">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1708">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="1c1bc-1709">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1709">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1710">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1710">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1711">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1711">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="1c1bc-1712">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1712">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="1c1bc-1713">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1713">Az.Insights</span></span>
* <span data-ttu-id="1c1bc-1714">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1714">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="1c1bc-1715">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1715">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="1c1bc-1716">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1716">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="1c1bc-1717">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1717">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1718">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1718">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1719">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1719">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="1c1bc-1720">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1720">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="1c1bc-1721">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1721">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="1c1bc-1722">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1722">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="1c1bc-1723">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1723">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="1c1bc-1724">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1724">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="1c1bc-1725">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1725">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c1bc-1726">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1726">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c1bc-1727">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1727">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1728">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1728">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1729">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1729">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="1c1bc-1730">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1730">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c1bc-1731">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1731">Az.ServiceBus</span></span>
* <span data-ttu-id="1c1bc-1732">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1732">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c1bc-1733">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1733">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c1bc-1734">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1734">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="1c1bc-1735">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1735">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="1c1bc-1736">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1736">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="1c1bc-1737">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1737">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="1c1bc-1738">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1738">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="1c1bc-1739">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1739">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="1c1bc-1740">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1740">Az.Profile</span></span>
* <span data-ttu-id="1c1bc-1741">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1741">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="1c1bc-1742">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1742">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1743">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1743">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1744">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1744">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="1c1bc-1745">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1745">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c1bc-1746">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1746">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c1bc-1747">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1747">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="1c1bc-1748">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1748">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="1c1bc-1749">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1749">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1c1bc-1750">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1750">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1c1bc-1751">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1751">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1752">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1752">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1753">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1753">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="1c1bc-1754">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1754">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1755">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1755">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1756">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1756">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="1c1bc-1757">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1757">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="1c1bc-1758">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1758">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="1c1bc-1759">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1759">Azure.Storage</span></span>
* <span data-ttu-id="1c1bc-1760">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1760">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="1c1bc-1761">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1761">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="1c1bc-1762">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1762">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1c1bc-1763">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1763">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="1c1bc-1764">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1764">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="1c1bc-1765">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1765">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c1bc-1766">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1766">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c1bc-1767">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1767">Az.Compute</span></span>
* <span data-ttu-id="1c1bc-1768">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1768">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="1c1bc-1769">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1769">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="1c1bc-1770">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1770">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="1c1bc-1771">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1771">Az.DataFactoryV2</span></span>
* <span data-ttu-id="1c1bc-1772">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1772">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c1bc-1773">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1773">Az.Network</span></span>
* <span data-ttu-id="1c1bc-1774">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1774">Added NetworkProfile functionality.</span></span> <span data-ttu-id="1c1bc-1775">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1775">new cmdlets added</span></span>
    - <span data-ttu-id="1c1bc-1776">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1776">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c1bc-1777">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1777">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c1bc-1778">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1778">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c1bc-1779">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1779">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c1bc-1780">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1780">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="1c1bc-1781">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1781">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="1c1bc-1782">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1782">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="1c1bc-1783">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1783">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="1c1bc-1784">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1784">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c1bc-1785">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1785">Az.RedisCache</span></span>
* <span data-ttu-id="1c1bc-1786">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1786">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="1c1bc-1787">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1787">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c1bc-1788">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1788">Az.Resources</span></span>
* <span data-ttu-id="1c1bc-1789">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1789">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1c1bc-1790">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1790">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c1bc-1791">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1791">Az.Sql</span></span>
* <span data-ttu-id="1c1bc-1792">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1792">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c1bc-1793">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1793">Az.Websites</span></span>
* <span data-ttu-id="1c1bc-1794">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1794">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="1c1bc-1795">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1795">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="1c1bc-1796">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1796">0.2.0 - September 2018</span></span>
 <span data-ttu-id="1c1bc-1797">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="1c1bc-1797">Initial Release</span></span>
