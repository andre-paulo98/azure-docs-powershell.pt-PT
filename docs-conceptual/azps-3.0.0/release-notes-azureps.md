---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: ee3f54e6bc15dbbaeb97cad7463cb1d2e5795e3e
ms.sourcegitcommit: 05431341858d10eb9c345213275c3ccc24c83c9b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/13/2019
ms.locfileid: "74062144"
---
## <a name="300---november-2019"></a><span data-ttu-id="1c80f-103">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-103">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="1c80f-104">Geral</span><span class="sxs-lookup"><span data-stu-id="1c80f-104">General</span></span>
* <span data-ttu-id="1c80f-105">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-105">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c80f-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-106">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-107">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="1c80f-107">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="1c80f-108">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="1c80f-108">Az.Advisor</span></span>
* <span data-ttu-id="1c80f-109">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="1c80f-109">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1c80f-110">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c80f-110">Az.Batch</span></span>
* <span data-ttu-id="1c80f-111">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-111">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="1c80f-112">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-112">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="1c80f-113">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-113">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="1c80f-114">O parâmetro `-ResourceFile` de **New-AzBatchTask** agora assume uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-114">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="1c80f-115">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-115">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="1c80f-116">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-116">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="1c80f-117">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="1c80f-117">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="1c80f-118">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="1c80f-118">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="1c80f-119">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="1c80f-119">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="1c80f-120">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-120">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="1c80f-121">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-121">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="1c80f-122">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-122">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="1c80f-123">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-123">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="1c80f-124">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-124">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="1c80f-125">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-125">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="1c80f-126">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-126">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="1c80f-127">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-127">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="1c80f-128">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-128">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="1c80f-129">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-129">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="1c80f-130">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-130">This operation is no longer supported.</span></span>
* <span data-ttu-id="1c80f-131">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-131">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="1c80f-132">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-132">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="1c80f-133">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-133">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="1c80f-134">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-134">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="1c80f-135">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="1c80f-135">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="1c80f-136">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-136">New non-verified images are also now returned.</span></span> <span data-ttu-id="1c80f-137">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-137">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="1c80f-138">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-138">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="1c80f-139">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="1c80f-139">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="1c80f-140">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-140">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="1c80f-141">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="1c80f-141">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="1c80f-142">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-142">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="1c80f-143">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-143">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="1c80f-144">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="1c80f-144">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="1c80f-145">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="1c80f-145">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="1c80f-146">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="1c80f-146">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c80f-147">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c80f-147">Az.Cdn</span></span>
* <span data-ttu-id="1c80f-148">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="1c80f-148">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="1c80f-149">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="1c80f-149">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-150">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-150">Az.Compute</span></span>
* <span data-ttu-id="1c80f-151">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="1c80f-151">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="1c80f-152">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-152">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="1c80f-153">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="1c80f-153">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="1c80f-154">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="1c80f-154">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="1c80f-155">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-155">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1c80f-156">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-156">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="1c80f-157">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="1c80f-157">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="1c80f-158">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c80f-158">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="1c80f-159">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c80f-159">Breaking changes</span></span>
    - <span data-ttu-id="1c80f-160">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="1c80f-160">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="1c80f-161">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="1c80f-161">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-162">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-162">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-163">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-163">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-164">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-164">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-165">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="1c80f-165">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="1c80f-166">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="1c80f-166">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="1c80f-167">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="1c80f-167">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="1c80f-168">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="1c80f-168">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="1c80f-169">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="1c80f-169">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="1c80f-170">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="1c80f-170">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c80f-171">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c80f-171">Az.FrontDoor</span></span>
* <span data-ttu-id="1c80f-172">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="1c80f-172">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="1c80f-173">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c80f-173">Az.HDInsight</span></span>
* <span data-ttu-id="1c80f-174">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="1c80f-174">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="1c80f-175">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="1c80f-175">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="1c80f-176">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-176">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="1c80f-177">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-177">Removed five cmdlets:</span></span>
    - <span data-ttu-id="1c80f-178">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="1c80f-178">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="1c80f-179">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="1c80f-179">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="1c80f-180">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="1c80f-180">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="1c80f-181">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c80f-181">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="1c80f-182">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c80f-182">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="1c80f-183">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-183">Added three cmdlets:</span></span>
    - <span data-ttu-id="1c80f-184">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="1c80f-184">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="1c80f-185">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="1c80f-185">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="1c80f-186">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="1c80f-186">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="1c80f-187">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="1c80f-187">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="1c80f-188">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="1c80f-188">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="1c80f-189">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="1c80f-189">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="1c80f-190">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-190">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="1c80f-191">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="1c80f-191">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="1c80f-192">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="1c80f-192">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="1c80f-193">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="1c80f-193">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="1c80f-194">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="1c80f-194">Added some scenario test cases.</span></span>
* <span data-ttu-id="1c80f-195">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="1c80f-195">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-196">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-196">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-197">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="1c80f-197">Breaking changes:</span></span>
    - <span data-ttu-id="1c80f-198">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c80f-198">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c80f-199">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c80f-199">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="1c80f-200">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c80f-200">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c80f-201">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c80f-201">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="1c80f-202">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="1c80f-202">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="1c80f-203">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="1c80f-203">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="1c80f-204">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="1c80f-204">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="1c80f-205">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="1c80f-205">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="1c80f-206">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c80f-206">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c80f-207">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c80f-207">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="1c80f-208">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="1c80f-208">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="1c80f-209">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="1c80f-209">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-210">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-210">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-211">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-211">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-212">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-212">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="1c80f-213">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-213">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="1c80f-214">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-214">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-215">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-215">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-216">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-216">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-217">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-217">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-218">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-218">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-219">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="1c80f-219">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-220">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-220">Az.Resources</span></span>
* <span data-ttu-id="1c80f-221">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="1c80f-221">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-222">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-222">Az.Network</span></span>
* <span data-ttu-id="1c80f-223">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="1c80f-223">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="1c80f-224">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c80f-224">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c80f-225">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-225">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-226">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-226">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-227">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-227">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-228">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-228">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-229">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-229">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="1c80f-230">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="1c80f-230">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="1c80f-231">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="1c80f-231">New cmdlet:</span></span>
        - <span data-ttu-id="1c80f-232">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="1c80f-232">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="1c80f-233">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="1c80f-233">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="1c80f-234">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-234">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="1c80f-235">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-235">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="1c80f-236">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="1c80f-236">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="1c80f-237">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="1c80f-237">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="1c80f-238">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-238">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="1c80f-239">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-239">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="1c80f-240">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-240">New cmdlets added:</span></span>
        - <span data-ttu-id="1c80f-241">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="1c80f-241">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="1c80f-242">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-242">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="1c80f-243">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-243">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="1c80f-244">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-244">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="1c80f-245">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-245">Set-AzVirtualHub</span></span>
* <span data-ttu-id="1c80f-246">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="1c80f-246">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="1c80f-247">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c80f-247">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c80f-248">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="1c80f-248">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="1c80f-249">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="1c80f-249">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="1c80f-250">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="1c80f-250">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="1c80f-251">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="1c80f-251">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="1c80f-252">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-252">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="1c80f-253">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-253">New cmdlets added:</span></span>
        - <span data-ttu-id="1c80f-254">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-254">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="1c80f-255">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c80f-255">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c80f-256">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c80f-256">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c80f-257">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c80f-257">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c80f-258">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c80f-258">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c80f-259">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c80f-259">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="1c80f-260">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="1c80f-260">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="1c80f-261">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="1c80f-261">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="1c80f-262">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-262">New cmdlets added:</span></span>
        - <span data-ttu-id="1c80f-263">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="1c80f-263">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="1c80f-264">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="1c80f-264">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="1c80f-265">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="1c80f-265">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="1c80f-266">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="1c80f-266">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="1c80f-267">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-267">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="1c80f-268">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-268">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="1c80f-269">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c80f-269">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c80f-270">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-270">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="1c80f-271">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-271">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="1c80f-272">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="1c80f-272">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="1c80f-273">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="1c80f-273">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="1c80f-274">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="1c80f-274">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="1c80f-275">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="1c80f-275">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="1c80f-276">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="1c80f-276">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="1c80f-277">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="1c80f-277">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="1c80f-278">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c80f-278">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="1c80f-279">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-279">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="1c80f-280">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-280">New cmdlets added:</span></span>
        - <span data-ttu-id="1c80f-281">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-281">New-AzIpGroup</span></span>
        - <span data-ttu-id="1c80f-282">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-282">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="1c80f-283">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-283">Get-AzIpGroup</span></span>
        - <span data-ttu-id="1c80f-284">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-284">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-285">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-285">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-286">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="1c80f-286">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-287">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-287">Az.Sql</span></span>
* <span data-ttu-id="1c80f-288">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-288">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="1c80f-289">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="1c80f-289">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="1c80f-290">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="1c80f-290">Removed deprecated aliases:</span></span>
* <span data-ttu-id="1c80f-291">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="1c80f-291">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="1c80f-292">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="1c80f-292">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="1c80f-293">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-293">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="1c80f-294">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="1c80f-294">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="1c80f-295">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="1c80f-295">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="1c80f-296">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="1c80f-296">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-297">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-297">Az.Storage</span></span>
* <span data-ttu-id="1c80f-298">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1c80f-298">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="1c80f-299">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-299">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="1c80f-300">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-300">Set-AzStorageAccount</span></span>
* <span data-ttu-id="1c80f-301">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="1c80f-301">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="1c80f-302">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c80f-302">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="1c80f-303">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c80f-303">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="1c80f-304">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-304">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="1c80f-305">Geral</span><span class="sxs-lookup"><span data-stu-id="1c80f-305">General</span></span>
* <span data-ttu-id="1c80f-306">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-306">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c80f-307">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-307">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-308">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="1c80f-308">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="1c80f-309">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-309">Az.ApiManagement</span></span>
* <span data-ttu-id="1c80f-310">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-310">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="1c80f-311">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="1c80f-311">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-312">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-312">Az.Automation</span></span>
* <span data-ttu-id="1c80f-313">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="1c80f-313">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="1c80f-314">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c80f-314">Az.Batch</span></span>
* <span data-ttu-id="1c80f-315">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="1c80f-315">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-316">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-316">Az.Compute</span></span>
* <span data-ttu-id="1c80f-317">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c80f-317">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="1c80f-318">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="1c80f-318">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="1c80f-319">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="1c80f-319">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="1c80f-320">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-320">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-321">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-321">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-322">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="1c80f-322">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="1c80f-323">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="1c80f-323">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="1c80f-324">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-324">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-325">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-325">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-326">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="1c80f-326">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="1c80f-327">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="1c80f-327">Az.HealthcareApis</span></span>
* <span data-ttu-id="1c80f-328">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-328">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="1c80f-329">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="1c80f-329">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="1c80f-330">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="1c80f-330">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="1c80f-331">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="1c80f-331">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-332">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-332">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-333">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="1c80f-333">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="1c80f-334">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="1c80f-334">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-335">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-335">Az.Monitor</span></span>
* <span data-ttu-id="1c80f-336">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="1c80f-336">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="1c80f-337">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="1c80f-337">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="1c80f-338">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="1c80f-338">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="1c80f-339">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1c80f-339">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-340">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-340">Az.Network</span></span>
* <span data-ttu-id="1c80f-341">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="1c80f-341">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="1c80f-342">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c80f-342">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="1c80f-343">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-343">New cmdlets added:</span></span>
        - <span data-ttu-id="1c80f-344">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-344">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="1c80f-345">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-345">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="1c80f-346">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="1c80f-346">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="1c80f-347">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="1c80f-347">Updated cmdlets:</span></span>
        - <span data-ttu-id="1c80f-348">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-348">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c80f-349">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-349">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c80f-350">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-350">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="1c80f-351">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="1c80f-351">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="1c80f-352">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="1c80f-352">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="1c80f-353">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="1c80f-353">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="1c80f-354">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="1c80f-354">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c80f-355">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c80f-355">Az.RedisCache</span></span>
* <span data-ttu-id="1c80f-356">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="1c80f-356">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-357">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-357">Az.Sql</span></span>
* <span data-ttu-id="1c80f-358">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="1c80f-358">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-359">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-359">Az.Storage</span></span>
* <span data-ttu-id="1c80f-360">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-360">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="1c80f-361">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="1c80f-361">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="1c80f-362">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="1c80f-362">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="1c80f-363">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="1c80f-363">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="1c80f-364">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-364">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="1c80f-365">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="1c80f-365">Az.StorageSync</span></span>
* <span data-ttu-id="1c80f-366">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="1c80f-366">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-367">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-367">Az.Websites</span></span>
* <span data-ttu-id="1c80f-368">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="1c80f-368">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="1c80f-369">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-369">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="1c80f-370">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-370">Az.ApiManagement</span></span>
* <span data-ttu-id="1c80f-371">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="1c80f-371">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="1c80f-372">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="1c80f-372">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="1c80f-373">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="1c80f-373">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-374">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-374">Az.Automation</span></span>
* <span data-ttu-id="1c80f-375">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="1c80f-375">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="1c80f-376">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="1c80f-376">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="1c80f-377">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="1c80f-377">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-378">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-378">Az.Compute</span></span>
* <span data-ttu-id="1c80f-379">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-379">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="1c80f-380">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-380">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1c80f-381">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="1c80f-381">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="1c80f-382">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="1c80f-382">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="1c80f-383">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="1c80f-383">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="1c80f-384">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c80f-384">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="1c80f-385">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="1c80f-385">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="1c80f-386">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="1c80f-386">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="1c80f-387">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="1c80f-387">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-388">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-388">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-389">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="1c80f-389">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="1c80f-390">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="1c80f-390">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="1c80f-391">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c80f-391">Az.HDInsight</span></span>
* <span data-ttu-id="1c80f-392">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c80f-392">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-393">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-393">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-394">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-394">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="1c80f-395">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="1c80f-395">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="1c80f-396">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="1c80f-396">New cmdlets are:</span></span>
    - <span data-ttu-id="1c80f-397">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c80f-397">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="1c80f-398">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c80f-398">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="1c80f-399">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c80f-399">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="1c80f-400">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="1c80f-400">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-401">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-401">Az.Monitor</span></span>
* <span data-ttu-id="1c80f-402">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="1c80f-402">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="1c80f-403">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-403">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="1c80f-404">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c80f-404">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="1c80f-405">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-405">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="1c80f-406">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="1c80f-406">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="1c80f-407">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="1c80f-407">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="1c80f-408">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c80f-408">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="1c80f-409">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-409">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="1c80f-410">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="1c80f-410">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="1c80f-411">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="1c80f-411">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="1c80f-412">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="1c80f-412">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="1c80f-413">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="1c80f-413">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="1c80f-414">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="1c80f-414">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="1c80f-415">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="1c80f-415">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="1c80f-416">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="1c80f-416">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="1c80f-417">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="1c80f-417">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="1c80f-418">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="1c80f-418">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="1c80f-419">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c80f-419">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="1c80f-420">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="1c80f-420">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="1c80f-421">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c80f-421">Overall improved help files</span></span>
* <span data-ttu-id="1c80f-422">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="1c80f-422">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-423">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-423">Az.Network</span></span>
* <span data-ttu-id="1c80f-424">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="1c80f-424">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="1c80f-425">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="1c80f-425">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="1c80f-426">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="1c80f-426">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="1c80f-427">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="1c80f-427">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="1c80f-428">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="1c80f-428">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="1c80f-429">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="1c80f-429">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="1c80f-430">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="1c80f-430">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="1c80f-431">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="1c80f-431">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="1c80f-432">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-432">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="1c80f-433">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="1c80f-433">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="1c80f-434">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c80f-434">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="1c80f-435">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="1c80f-435">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="1c80f-436">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-436">New cmdlets</span></span>
        - <span data-ttu-id="1c80f-437">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="1c80f-437">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="1c80f-438">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-438">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="1c80f-439">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c80f-439">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c80f-440">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="1c80f-440">New-VpnSite</span></span>
        - <span data-ttu-id="1c80f-441">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="1c80f-441">Update-VpnSite</span></span>
        - <span data-ttu-id="1c80f-442">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-442">New-VpnConnection</span></span>
        - <span data-ttu-id="1c80f-443">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-443">Update-VpnConnection</span></span>
* <span data-ttu-id="1c80f-444">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="1c80f-444">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-445">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-445">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-446">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="1c80f-446">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="1c80f-447">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="1c80f-447">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-448">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-448">Az.Resources</span></span>
* <span data-ttu-id="1c80f-449">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="1c80f-449">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-450">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-450">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-451">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="1c80f-451">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="1c80f-452">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="1c80f-452">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="1c80f-453">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c80f-453">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c80f-454">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="1c80f-454">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="1c80f-455">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1c80f-455">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="1c80f-456">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="1c80f-456">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="1c80f-457">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c80f-457">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c80f-458">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c80f-458">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c80f-459">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="1c80f-459">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="1c80f-460">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1c80f-460">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="1c80f-461">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="1c80f-461">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="1c80f-462">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="1c80f-462">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="1c80f-463">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="1c80f-463">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="1c80f-464">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="1c80f-464">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="1c80f-465">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="1c80f-465">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="1c80f-466">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="1c80f-466">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1c80f-467">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1c80f-467">Az.SignalR</span></span>
* <span data-ttu-id="1c80f-468">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="1c80f-468">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-469">Az.Sql</span></span>
* <span data-ttu-id="1c80f-470">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="1c80f-470">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="1c80f-471">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="1c80f-471">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="1c80f-472">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-472">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="1c80f-473">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="1c80f-473">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="1c80f-474">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="1c80f-474">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-475">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-475">Az.Storage</span></span>
* <span data-ttu-id="1c80f-476">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="1c80f-476">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="1c80f-477">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="1c80f-477">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="1c80f-478">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-478">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="1c80f-479">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-479">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="1c80f-480">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="1c80f-480">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="1c80f-481">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-481">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="1c80f-482">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="1c80f-482">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="1c80f-483">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c80f-483">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="1c80f-484">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c80f-484">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="1c80f-485">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c80f-485">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="1c80f-486">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="1c80f-486">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-487">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-487">Az.Websites</span></span>
* <span data-ttu-id="1c80f-488">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="1c80f-488">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="1c80f-489">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="1c80f-489">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="1c80f-490">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="1c80f-490">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="1c80f-491">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-491">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="1c80f-492">Geral</span><span class="sxs-lookup"><span data-stu-id="1c80f-492">General</span></span>
* <span data-ttu-id="1c80f-493">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="1c80f-493">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c80f-494">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-494">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-495">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="1c80f-495">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="1c80f-496">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="1c80f-496">Az.Aks</span></span>
* <span data-ttu-id="1c80f-497">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="1c80f-497">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="1c80f-498">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="1c80f-498">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="1c80f-499">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-499">Az.ApiManagement</span></span>
* <span data-ttu-id="1c80f-500">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="1c80f-500">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="1c80f-501">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="1c80f-501">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="1c80f-502">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="1c80f-502">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="1c80f-503">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="1c80f-503">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="1c80f-504">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="1c80f-504">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1c80f-505">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c80f-505">Az.Batch</span></span>
* <span data-ttu-id="1c80f-506">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="1c80f-506">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c80f-507">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c80f-507">Az.Cdn</span></span>
* <span data-ttu-id="1c80f-508">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="1c80f-508">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-509">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-509">Az.Compute</span></span>
* <span data-ttu-id="1c80f-510">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-510">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="1c80f-511">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c80f-511">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="1c80f-512">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="1c80f-512">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="1c80f-513">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="1c80f-513">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="1c80f-514">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="1c80f-514">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="1c80f-515">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c80f-515">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="1c80f-516">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="1c80f-516">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="1c80f-517">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="1c80f-517">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-518">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-518">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-519">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="1c80f-519">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="1c80f-520">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="1c80f-520">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="1c80f-521">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="1c80f-521">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="1c80f-522">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="1c80f-522">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-523">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-523">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-524">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-524">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c80f-525">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-525">Az.EventHub</span></span>
* <span data-ttu-id="1c80f-526">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-526">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="1c80f-527">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="1c80f-527">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="1c80f-528">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="1c80f-528">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="1c80f-529">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="1c80f-529">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="1c80f-530">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1c80f-530">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="1c80f-531">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="1c80f-531">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-532">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-532">Az.Monitor</span></span>
* <span data-ttu-id="1c80f-533">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c80f-533">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-534">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-534">Az.Network</span></span>
* <span data-ttu-id="1c80f-535">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="1c80f-535">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="1c80f-536">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="1c80f-536">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="1c80f-537">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="1c80f-537">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="1c80f-538">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="1c80f-538">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="1c80f-539">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="1c80f-539">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="1c80f-540">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="1c80f-540">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="1c80f-541">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="1c80f-541">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-542">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-542">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c80f-543">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="1c80f-543">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="1c80f-544">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="1c80f-544">Added example</span></span>
    - <span data-ttu-id="1c80f-545">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="1c80f-545">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="1c80f-546">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="1c80f-546">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="1c80f-547">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="1c80f-547">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-548">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-548">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-549">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-549">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-550">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-550">Az.Resources</span></span>
* <span data-ttu-id="1c80f-551">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="1c80f-551">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="1c80f-552">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="1c80f-552">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="1c80f-553">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="1c80f-553">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="1c80f-554">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c80f-554">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c80f-555">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c80f-555">Az.ServiceBus</span></span>
* <span data-ttu-id="1c80f-556">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-556">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="1c80f-557">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="1c80f-557">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="1c80f-558">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="1c80f-558">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-559">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-559">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-560">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="1c80f-560">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="1c80f-561">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="1c80f-561">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="1c80f-562">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="1c80f-562">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="1c80f-563">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="1c80f-563">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="1c80f-564">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="1c80f-564">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="1c80f-565">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="1c80f-565">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-566">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-566">Az.Sql</span></span>
* <span data-ttu-id="1c80f-567">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-567">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-568">Az.Storage</span></span>
* <span data-ttu-id="1c80f-569">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="1c80f-569">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="1c80f-570">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="1c80f-570">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="1c80f-571">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-571">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="1c80f-572">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1c80f-572">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="1c80f-573">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="1c80f-573">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="1c80f-574">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1c80f-574">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-575">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-575">Az.Websites</span></span>
* <span data-ttu-id="1c80f-576">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="1c80f-576">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="1c80f-577">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-577">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-578">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-578">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-579">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c80f-579">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="1c80f-580">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-580">Az.ApplicationInsights</span></span>
* <span data-ttu-id="1c80f-581">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="1c80f-581">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="1c80f-582">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-582">Az.Automation</span></span>
* <span data-ttu-id="1c80f-583">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="1c80f-583">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c80f-584">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-584">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c80f-585">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="1c80f-585">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-586">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-586">Az.Compute</span></span>
* <span data-ttu-id="1c80f-587">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="1c80f-587">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="1c80f-588">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1c80f-588">Az.ContainerRegistry</span></span>
* <span data-ttu-id="1c80f-589">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="1c80f-589">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="1c80f-590">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="1c80f-590">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-591">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-591">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-592">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-592">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="1c80f-593">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="1c80f-593">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c80f-594">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-594">Az.EventHub</span></span>
* <span data-ttu-id="1c80f-595">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="1c80f-595">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="1c80f-596">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="1c80f-596">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c80f-597">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-597">Az.KeyVault</span></span>
* <span data-ttu-id="1c80f-598">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="1c80f-598">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c80f-599">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-599">Az.LogicApp</span></span>
* <span data-ttu-id="1c80f-600">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="1c80f-600">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="1c80f-601">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="1c80f-601">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="1c80f-602">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-602">Az.ManagedServices</span></span>
* <span data-ttu-id="1c80f-603">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="1c80f-603">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-604">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-604">Az.Network</span></span>
* <span data-ttu-id="1c80f-605">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="1c80f-605">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="1c80f-606">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-606">New cmdlets</span></span>
        - <span data-ttu-id="1c80f-607">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c80f-607">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c80f-608">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-608">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="1c80f-609">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-609">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-610">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-610">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-611">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-611">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-612">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-612">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="1c80f-613">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="1c80f-613">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="1c80f-614">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-614">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="1c80f-615">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="1c80f-615">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="1c80f-616">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-616">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="1c80f-617">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="1c80f-617">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="1c80f-618">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="1c80f-618">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="1c80f-619">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="1c80f-619">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="1c80f-620">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="1c80f-620">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="1c80f-621">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="1c80f-621">Updated cmdlets</span></span>
        - <span data-ttu-id="1c80f-622">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-622">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c80f-623">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-623">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="1c80f-624">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-624">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="1c80f-625">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-625">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="1c80f-626">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-626">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="1c80f-627">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c80f-627">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c80f-628">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-628">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="1c80f-629">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-629">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="1c80f-630">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-630">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="1c80f-631">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="1c80f-631">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="1c80f-632">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="1c80f-632">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="1c80f-633">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="1c80f-633">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-634">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-634">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c80f-635">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="1c80f-635">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="1c80f-636">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="1c80f-636">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-637">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-637">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-638">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-638">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="1c80f-639">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-639">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="1c80f-640">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-640">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="1c80f-641">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-641">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="1c80f-642">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-642">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="1c80f-643">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-643">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="1c80f-644">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-644">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="1c80f-645">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-645">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="1c80f-646">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-646">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="1c80f-647">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="1c80f-647">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-648">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-648">Az.Resources</span></span>
- <span data-ttu-id="1c80f-649">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="1c80f-649">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="1c80f-650">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="1c80f-650">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c80f-651">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c80f-651">Az.ServiceBus</span></span>
* <span data-ttu-id="1c80f-652">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="1c80f-652">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="1c80f-653">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="1c80f-653">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-654">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-654">Az.Sql</span></span>
* <span data-ttu-id="1c80f-655">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="1c80f-655">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="1c80f-656">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="1c80f-656">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="1c80f-657">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="1c80f-657">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-658">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-658">Az.Storage</span></span>
* <span data-ttu-id="1c80f-659">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="1c80f-659">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="1c80f-660">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="1c80f-660">Az.StorageSync</span></span>
* <span data-ttu-id="1c80f-661">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="1c80f-661">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="1c80f-662">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="1c80f-662">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-663">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-663">Az.Websites</span></span>
* <span data-ttu-id="1c80f-664">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-664">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="1c80f-665">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-665">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="1c80f-666">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-666">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="1c80f-667">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-667">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-668">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-668">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-669">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="1c80f-669">Add support for profile cmdlets</span></span>
* <span data-ttu-id="1c80f-670">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="1c80f-670">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="1c80f-671">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="1c80f-671">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="1c80f-672">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="1c80f-672">Az.Advisor</span></span>
* <span data-ttu-id="1c80f-673">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="1c80f-673">GA release of Az.Advisor</span></span>
* <span data-ttu-id="1c80f-674">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="1c80f-674">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="1c80f-675">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-675">Az.ApiManagement</span></span>
* <span data-ttu-id="1c80f-676">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="1c80f-676">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="1c80f-677">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="1c80f-677">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="1c80f-678">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="1c80f-678">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="1c80f-679">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="1c80f-679">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="1c80f-680">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="1c80f-680">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="1c80f-681">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c80f-681">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="1c80f-682">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="1c80f-682">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-683">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-683">Az.Automation</span></span>
* <span data-ttu-id="1c80f-684">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="1c80f-684">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-685">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-685">Az.Compute</span></span>
* <span data-ttu-id="1c80f-686">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-686">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-687">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-687">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-688">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="1c80f-688">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c80f-689">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c80f-689">Az.EventGrid</span></span>
* <span data-ttu-id="1c80f-690">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="1c80f-690">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-691">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-691">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-692">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="1c80f-692">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-693">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-693">Az.Network</span></span>
* <span data-ttu-id="1c80f-694">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="1c80f-694">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="1c80f-695">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="1c80f-695">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c80f-696">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-696">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c80f-697">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="1c80f-697">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="1c80f-698">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="1c80f-698">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-699">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-699">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c80f-700">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="1c80f-700">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-701">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-701">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-702">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="1c80f-702">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-703">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-703">Az.Resources</span></span>
    - <span data-ttu-id="1c80f-704">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="1c80f-704">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="1c80f-705">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="1c80f-705">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="1c80f-706">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="1c80f-706">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="1c80f-707">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="1c80f-707">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c80f-708">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c80f-708">Az.ServiceBus</span></span>
* <span data-ttu-id="1c80f-709">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="1c80f-709">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-710">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-710">Az.Sql</span></span>
* <span data-ttu-id="1c80f-711">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="1c80f-711">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="1c80f-712">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-712">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="1c80f-713">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="1c80f-713">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="1c80f-714">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="1c80f-714">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="1c80f-715">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="1c80f-715">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="1c80f-716">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="1c80f-716">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="1c80f-717">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="1c80f-717">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="1c80f-718">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="1c80f-718">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="1c80f-719">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="1c80f-719">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-720">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-720">Az.Storage</span></span>
* <span data-ttu-id="1c80f-721">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="1c80f-721">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="1c80f-722">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1c80f-722">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="1c80f-723">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="1c80f-723">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="1c80f-724">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="1c80f-724">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="1c80f-725">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-725">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="1c80f-726">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-726">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="1c80f-727">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-727">Set-AzStorageAccount</span></span>
* <span data-ttu-id="1c80f-728">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="1c80f-728">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="1c80f-729">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c80f-729">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="1c80f-730">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="1c80f-730">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="1c80f-731">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="1c80f-731">Az.StorageSync</span></span>
* <span data-ttu-id="1c80f-732">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="1c80f-732">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="1c80f-733">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-733">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-734">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-734">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-735">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="1c80f-735">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="1c80f-736">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="1c80f-736">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="1c80f-737">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="1c80f-737">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="1c80f-738">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="1c80f-738">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="1c80f-739">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="1c80f-739">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-740">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-740">Az.Compute</span></span>
* <span data-ttu-id="1c80f-741">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="1c80f-741">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="1c80f-742">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="1c80f-742">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="1c80f-743">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="1c80f-743">Az.Dns</span></span>
* <span data-ttu-id="1c80f-744">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="1c80f-744">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c80f-745">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c80f-745">Az.EventGrid</span></span>
* <span data-ttu-id="1c80f-746">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="1c80f-746">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="1c80f-747">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-747">New cmdlets:</span></span>
    - <span data-ttu-id="1c80f-748">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="1c80f-748">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="1c80f-749">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c80f-749">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="1c80f-750">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="1c80f-750">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="1c80f-751">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-751">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="1c80f-752">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="1c80f-752">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="1c80f-753">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c80f-753">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="1c80f-754">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="1c80f-754">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="1c80f-755">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c80f-755">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="1c80f-756">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="1c80f-756">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="1c80f-757">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c80f-757">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="1c80f-758">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="1c80f-758">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="1c80f-759">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="1c80f-759">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="1c80f-760">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="1c80f-760">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="1c80f-761">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="1c80f-761">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="1c80f-762">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="1c80f-762">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="1c80f-763">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="1c80f-763">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="1c80f-764">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="1c80f-764">Updated cmdlets:</span></span>
    - <span data-ttu-id="1c80f-765">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="1c80f-765">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="1c80f-766">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-766">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="1c80f-767">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-767">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="1c80f-768">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="1c80f-768">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="1c80f-769">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="1c80f-769">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="1c80f-770">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="1c80f-770">Event subscription expiration date,</span></span>
            - <span data-ttu-id="1c80f-771">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-771">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="1c80f-772">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="1c80f-772">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="1c80f-773">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="1c80f-773">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="1c80f-774">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="1c80f-774">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="1c80f-775">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="1c80f-775">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="1c80f-776">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="1c80f-776">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="1c80f-777">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-777">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="1c80f-778">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-778">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c80f-779">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c80f-779">Az.FrontDoor</span></span>
* <span data-ttu-id="1c80f-780">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="1c80f-780">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="1c80f-781">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="1c80f-781">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="1c80f-782">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="1c80f-782">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="1c80f-783">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="1c80f-783">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-784">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-784">Az.Network</span></span>
* <span data-ttu-id="1c80f-785">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c80f-785">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="1c80f-786">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-786">New cmdlets</span></span>
        - <span data-ttu-id="1c80f-787">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="1c80f-787">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="1c80f-788">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="1c80f-788">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="1c80f-789">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-789">New cmdlets</span></span> 
        - <span data-ttu-id="1c80f-790">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="1c80f-790">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="1c80f-791">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-791">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="1c80f-792">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-792">New cmdlets</span></span> 
        - <span data-ttu-id="1c80f-793">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-793">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="1c80f-794">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-794">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="1c80f-795">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="1c80f-795">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="1c80f-796">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-796">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="1c80f-797">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-797">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="1c80f-798">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c80f-798">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="1c80f-799">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-799">New cmdlets</span></span>
        - <span data-ttu-id="1c80f-800">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c80f-800">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c80f-801">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c80f-801">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c80f-802">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="1c80f-802">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="1c80f-803">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-803">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="1c80f-804">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="1c80f-804">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="1c80f-805">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="1c80f-805">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="1c80f-806">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="1c80f-806">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="1c80f-807">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="1c80f-807">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="1c80f-808">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="1c80f-808">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="1c80f-809">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="1c80f-809">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="1c80f-810">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-810">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="1c80f-811">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="1c80f-811">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="1c80f-812">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-812">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="1c80f-813">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="1c80f-813">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="1c80f-814">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-814">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="1c80f-815">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-815">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="1c80f-816">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="1c80f-816">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="1c80f-817">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c80f-817">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="1c80f-818">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c80f-818">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="1c80f-819">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="1c80f-819">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="1c80f-820">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c80f-820">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="1c80f-821">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="1c80f-821">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="1c80f-822">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="1c80f-822">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="1c80f-823">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="1c80f-823">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="1c80f-824">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-824">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="1c80f-825">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-825">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="1c80f-826">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-826">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-827">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-827">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c80f-828">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="1c80f-828">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-829">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-829">Az.Resources</span></span>
* <span data-ttu-id="1c80f-830">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="1c80f-830">Support for additional Template Export options</span></span>
    - <span data-ttu-id="1c80f-831">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-831">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="1c80f-832">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-832">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="1c80f-833">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="1c80f-833">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-834">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-834">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-835">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="1c80f-835">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-836">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-836">Az.Sql</span></span>
* <span data-ttu-id="1c80f-837">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="1c80f-837">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="1c80f-838">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="1c80f-838">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="1c80f-839">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="1c80f-839">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="1c80f-840">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="1c80f-840">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="1c80f-841">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="1c80f-841">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="1c80f-842">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="1c80f-842">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="1c80f-843">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="1c80f-843">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="1c80f-844">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="1c80f-844">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-845">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-845">Az.Storage</span></span>
* <span data-ttu-id="1c80f-846">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1c80f-846">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="1c80f-847">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-847">New-AzStorageAccount</span></span>
* <span data-ttu-id="1c80f-848">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="1c80f-848">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="1c80f-849">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-849">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-850">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-850">Az.Websites</span></span>
* <span data-ttu-id="1c80f-851">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="1c80f-851">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="1c80f-852">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="1c80f-852">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="1c80f-853">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-853">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="1c80f-854">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c80f-854">Az.Cdn</span></span>
* <span data-ttu-id="1c80f-855">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="1c80f-855">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-856">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-856">Az.Compute</span></span>
* <span data-ttu-id="1c80f-857">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="1c80f-857">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="1c80f-858">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c80f-858">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c80f-859">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-859">Az.EventHub</span></span>
* <span data-ttu-id="1c80f-860">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="1c80f-860">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="1c80f-861">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="1c80f-861">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-862">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-862">Az.Network</span></span>
* <span data-ttu-id="1c80f-863">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-863">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="1c80f-864">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="1c80f-864">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c80f-865">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-865">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c80f-866">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="1c80f-866">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-867">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-867">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-868">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="1c80f-868">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c80f-869">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c80f-869">Az.ServiceBus</span></span>
* <span data-ttu-id="1c80f-870">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="1c80f-870">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-871">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-871">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-872">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="1c80f-872">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="1c80f-873">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-873">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-874">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-874">Az.Sql</span></span>
* <span data-ttu-id="1c80f-875">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="1c80f-875">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="1c80f-876">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-876">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="1c80f-877">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="1c80f-877">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="1c80f-878">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="1c80f-878">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-879">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-879">Az.Websites</span></span>
* <span data-ttu-id="1c80f-880">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="1c80f-880">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="1c80f-881">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-881">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="1c80f-882">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-882">Az.ApiManagement</span></span>
* <span data-ttu-id="1c80f-883">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="1c80f-883">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="1c80f-884">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="1c80f-884">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="1c80f-885">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="1c80f-885">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="1c80f-886">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="1c80f-886">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="1c80f-887">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-887">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="1c80f-888">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="1c80f-888">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="1c80f-889">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="1c80f-889">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="1c80f-890">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="1c80f-890">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="1c80f-891">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-891">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="1c80f-892">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="1c80f-892">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="1c80f-893">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="1c80f-893">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="1c80f-894">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="1c80f-894">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="1c80f-895">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="1c80f-895">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="1c80f-896">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="1c80f-896">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="1c80f-897">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="1c80f-897">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="1c80f-898">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="1c80f-898">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="1c80f-899">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="1c80f-899">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="1c80f-900">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="1c80f-900">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="1c80f-901">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="1c80f-901">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="1c80f-902">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="1c80f-902">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="1c80f-903">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="1c80f-903">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="1c80f-904">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="1c80f-904">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="1c80f-905">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-905">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="1c80f-906">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-906">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="1c80f-907">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="1c80f-907">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="1c80f-908">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="1c80f-908">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="1c80f-909">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="1c80f-909">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="1c80f-910">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="1c80f-910">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="1c80f-911">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="1c80f-911">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="1c80f-912">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="1c80f-912">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="1c80f-913">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="1c80f-913">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="1c80f-914">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="1c80f-914">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="1c80f-915">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="1c80f-915">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="1c80f-916">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c80f-916">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="1c80f-917">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="1c80f-917">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="1c80f-918">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="1c80f-918">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="1c80f-919">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="1c80f-919">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="1c80f-920">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="1c80f-920">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="1c80f-921">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="1c80f-921">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="1c80f-922">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c80f-922">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="1c80f-923">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="1c80f-923">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="1c80f-924">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c80f-924">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="1c80f-925">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="1c80f-925">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="1c80f-926">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="1c80f-926">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="1c80f-927">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="1c80f-927">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="1c80f-928">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="1c80f-928">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="1c80f-929">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c80f-929">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="1c80f-930">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="1c80f-930">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="1c80f-931">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="1c80f-931">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="1c80f-932">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="1c80f-932">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="1c80f-933">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="1c80f-933">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="1c80f-934">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="1c80f-934">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="1c80f-935">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="1c80f-935">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="1c80f-936">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="1c80f-936">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="1c80f-937">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="1c80f-937">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="1c80f-938">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="1c80f-938">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="1c80f-939">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="1c80f-939">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="1c80f-940">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c80f-940">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="1c80f-941">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c80f-941">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="1c80f-942">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c80f-942">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="1c80f-943">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="1c80f-943">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="1c80f-944">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c80f-944">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="1c80f-945">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="1c80f-945">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="1c80f-946">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="1c80f-946">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="1c80f-947">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="1c80f-947">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="1c80f-948">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="1c80f-948">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="1c80f-949">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="1c80f-949">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="1c80f-950">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="1c80f-950">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="1c80f-951">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="1c80f-951">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="1c80f-952">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c80f-952">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="1c80f-953">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="1c80f-953">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="1c80f-954">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="1c80f-954">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="1c80f-955">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="1c80f-955">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="1c80f-956">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-956">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="1c80f-957">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="1c80f-957">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="1c80f-958">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="1c80f-958">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="1c80f-959">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="1c80f-959">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-960">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-960">Az.Automation</span></span>
* <span data-ttu-id="1c80f-961">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="1c80f-961">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="1c80f-962">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="1c80f-962">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="1c80f-963">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="1c80f-963">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="1c80f-964">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="1c80f-964">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="1c80f-965">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="1c80f-965">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="1c80f-966">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="1c80f-966">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="1c80f-967">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="1c80f-967">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-968">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-968">Az.Compute</span></span>
* <span data-ttu-id="1c80f-969">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="1c80f-969">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="1c80f-970">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="1c80f-970">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-971">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-971">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-972">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-972">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-973">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-973">Az.Monitor</span></span>
* <span data-ttu-id="1c80f-974">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c80f-974">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-975">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-975">Az.Network</span></span>
* <span data-ttu-id="1c80f-976">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="1c80f-976">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="1c80f-977">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="1c80f-977">Updated cmdlet:</span></span>
        - <span data-ttu-id="1c80f-978">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-978">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="1c80f-979">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1c80f-979">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-980">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-980">Az.Resources</span></span>
* <span data-ttu-id="1c80f-981">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="1c80f-981">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-982">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-982">Az.Sql</span></span>
* <span data-ttu-id="1c80f-983">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="1c80f-983">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="1c80f-984">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-984">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-985">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-985">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-986">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="1c80f-986">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c80f-987">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-987">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c80f-988">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="1c80f-988">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="1c80f-989">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="1c80f-989">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-990">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-990">Az.Compute</span></span>
* <span data-ttu-id="1c80f-991">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="1c80f-991">Proximity placement group feature.</span></span>
    - <span data-ttu-id="1c80f-992">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-992">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="1c80f-993">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-993">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="1c80f-994">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="1c80f-994">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="1c80f-995">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="1c80f-995">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="1c80f-996">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c80f-996">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="1c80f-997">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c80f-997">Breaking changes</span></span>
    - <span data-ttu-id="1c80f-998">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="1c80f-998">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="1c80f-999">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="1c80f-999">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="1c80f-1000">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="1c80f-1000">Az.DeploymentManager</span></span>
* <span data-ttu-id="1c80f-1001">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1001">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="1c80f-1002">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="1c80f-1002">Az.Dns</span></span>
* <span data-ttu-id="1c80f-1003">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="1c80f-1003">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="1c80f-1004">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1004">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="1c80f-1005">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1005">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="1c80f-1006">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1006">Az.FrontDoor</span></span>
* <span data-ttu-id="1c80f-1007">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="1c80f-1007">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="1c80f-1008">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1008">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="1c80f-1009">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c80f-1009">Az.HDInsight</span></span>
* <span data-ttu-id="1c80f-1010">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-1010">Removed two cmdlets:</span></span>
    - <span data-ttu-id="1c80f-1011">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c80f-1011">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="1c80f-1012">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c80f-1012">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="1c80f-1013">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="1c80f-1013">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="1c80f-1014">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="1c80f-1014">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="1c80f-1015">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1015">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="1c80f-1016">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1016">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-1017">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1017">Az.Monitor</span></span>
* <span data-ttu-id="1c80f-1018">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="1c80f-1018">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="1c80f-1019">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="1c80f-1019">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="1c80f-1020">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-1020">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="1c80f-1021">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="1c80f-1021">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="1c80f-1022">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1022">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="1c80f-1023">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="1c80f-1023">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="1c80f-1024">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="1c80f-1024">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="1c80f-1025">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1025">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c80f-1026">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1026">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c80f-1027">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1027">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c80f-1028">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1028">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c80f-1029">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1029">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="1c80f-1030">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="1c80f-1030">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="1c80f-1031">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="1c80f-1031">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1032">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1032">Az.Network</span></span>
* <span data-ttu-id="1c80f-1033">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="1c80f-1033">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="1c80f-1034">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-1034">New cmdlets</span></span>
        - <span data-ttu-id="1c80f-1035">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-1035">New-AzNatGateway</span></span>
        - <span data-ttu-id="1c80f-1036">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-1036">Get-AzNatGateway</span></span>
        - <span data-ttu-id="1c80f-1037">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-1037">Set-AzNatGateway</span></span>
        - <span data-ttu-id="1c80f-1038">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-1038">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="1c80f-1039">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="1c80f-1039">Updated cmdlets</span></span>
        - <span data-ttu-id="1c80f-1040">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="1c80f-1040">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="1c80f-1041">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="1c80f-1041">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="1c80f-1042">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1042">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="1c80f-1043">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1043">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="1c80f-1044">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1044">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c80f-1045">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-1045">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c80f-1046">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1046">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="1c80f-1047">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1047">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="1c80f-1048">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="1c80f-1048">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1049">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1049">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-1050">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1050">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="1c80f-1051">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1051">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="1c80f-1052">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1052">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="1c80f-1053">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1053">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="1c80f-1054">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1054">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="1c80f-1055">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1055">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="1c80f-1056">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="1c80f-1056">Az.Relay</span></span>
* <span data-ttu-id="1c80f-1057">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="1c80f-1057">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c80f-1058">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c80f-1058">Az.ServiceBus</span></span>
* <span data-ttu-id="1c80f-1059">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="1c80f-1059">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-1060">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1060">Az.Storage</span></span>
* <span data-ttu-id="1c80f-1061">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="1c80f-1061">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="1c80f-1062">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1062">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="1c80f-1063">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1063">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="1c80f-1064">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1064">New-AzStorageAccount</span></span>
* <span data-ttu-id="1c80f-1065">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="1c80f-1065">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="1c80f-1066">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1066">New-AzStorageAccount</span></span>
    - <span data-ttu-id="1c80f-1067">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1067">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="1c80f-1068">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1068">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1069">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1069">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1070">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-1070">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="1c80f-1071">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="1c80f-1071">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="1c80f-1072">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1072">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c80f-1073">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c80f-1073">Highlights since the last major release</span></span>
* <span data-ttu-id="1c80f-1074">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="1c80f-1074">General availability of `Az` module</span></span>
* <span data-ttu-id="1c80f-1075">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1c80f-1075">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1c80f-1076">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1c80f-1076">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1c80f-1077">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1077">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1c80f-1078">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c80f-1078">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c80f-1079">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1079">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1c80f-1080">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="1c80f-1080">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1081">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1081">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1082">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="1c80f-1082">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1c80f-1083">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c80f-1083">Az.Batch</span></span>
* <span data-ttu-id="1c80f-1084">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1084">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c80f-1085">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c80f-1085">Az.Cdn</span></span>
* <span data-ttu-id="1c80f-1086">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1086">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c80f-1087">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1087">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c80f-1088">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1088">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1089">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1089">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1090">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="1c80f-1090">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="1c80f-1091">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1091">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c80f-1092">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c80f-1092">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-1093">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-1093">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-1094">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1094">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1095">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1095">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-1096">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1096">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c80f-1097">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c80f-1097">Az.EventGrid</span></span>
* <span data-ttu-id="1c80f-1098">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1098">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c80f-1099">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1099">Az.EventHub</span></span>
* <span data-ttu-id="1c80f-1100">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="1c80f-1100">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="1c80f-1101">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1c80f-1101">Az.HDInsight</span></span>
* <span data-ttu-id="1c80f-1102">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1102">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-1103">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1103">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-1104">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1104">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c80f-1105">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-1105">Az.KeyVault</span></span>
* <span data-ttu-id="1c80f-1106">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1106">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c80f-1107">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c80f-1107">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="1c80f-1108">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1c80f-1108">Az.MachineLearning</span></span>
* <span data-ttu-id="1c80f-1109">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1109">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="1c80f-1110">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1c80f-1110">Az.Media</span></span>
* <span data-ttu-id="1c80f-1111">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1111">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-1112">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1112">Az.Monitor</span></span>
  * <span data-ttu-id="1c80f-1113">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="1c80f-1113">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="1c80f-1114">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="1c80f-1114">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="1c80f-1115">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="1c80f-1115">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="1c80f-1116">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1c80f-1116">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1c80f-1117">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1c80f-1117">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1c80f-1118">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1c80f-1118">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="1c80f-1119">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="1c80f-1119">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1120">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1120">Az.Network</span></span>
* <span data-ttu-id="1c80f-1121">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1121">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c80f-1122">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c80f-1122">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="1c80f-1123">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="1c80f-1123">Az.NotificationHubs</span></span>
* <span data-ttu-id="1c80f-1124">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1124">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-1125">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-1125">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c80f-1126">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1126">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="1c80f-1127">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1c80f-1127">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="1c80f-1128">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1128">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1129">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1129">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-1130">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1130">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c80f-1131">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1131">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="1c80f-1132">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="1c80f-1132">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="1c80f-1133">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="1c80f-1133">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c80f-1134">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c80f-1134">Az.RedisCache</span></span>
* <span data-ttu-id="1c80f-1135">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1135">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1136">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1136">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1137">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c80f-1137">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1138">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1138">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1139">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="1c80f-1139">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="1c80f-1140">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1140">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c80f-1141">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1141">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="1c80f-1142">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1142">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="1c80f-1143">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1143">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="1c80f-1144">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1144">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="1c80f-1145">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="1c80f-1145">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1146">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1146">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1147">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="1c80f-1147">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="1c80f-1148">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1148">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1c80f-1149">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1149">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="1c80f-1150">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1150">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="1c80f-1151">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1151">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c80f-1152">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c80f-1152">Highlights since the last major release</span></span>
* <span data-ttu-id="1c80f-1153">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="1c80f-1153">General availability of `Az` module</span></span>
* <span data-ttu-id="1c80f-1154">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1c80f-1154">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1c80f-1155">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1c80f-1155">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1c80f-1156">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1156">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1c80f-1157">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c80f-1157">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c80f-1158">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1158">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1c80f-1159">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="1c80f-1159">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1160">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1160">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1161">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="1c80f-1161">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1c80f-1162">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1162">Az.AnalysisServices</span></span>
* <span data-ttu-id="1c80f-1163">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="1c80f-1163">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="1c80f-1164">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="1c80f-1164">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-1165">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1165">Az.Automation</span></span>
* <span data-ttu-id="1c80f-1166">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1166">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="1c80f-1167">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1167">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="1c80f-1168">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1168">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1169">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1169">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1170">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-1170">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1c80f-1171">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1171">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="1c80f-1172">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1172">Az.ContainerInstance</span></span>
* <span data-ttu-id="1c80f-1173">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="1c80f-1173">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-1174">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-1174">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-1175">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="1c80f-1175">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="1c80f-1176">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1176">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1177">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1177">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1178">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1178">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="1c80f-1179">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1179">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="1c80f-1180">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="1c80f-1180">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="1c80f-1181">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1c80f-1181">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="1c80f-1182">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="1c80f-1182">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="1c80f-1183">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1c80f-1183">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1184">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1184">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1185">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1185">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-1186">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1186">Az.Storage</span></span>
* <span data-ttu-id="1c80f-1187">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1187">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="1c80f-1188">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1c80f-1188">New-AzStorageContext</span></span>
* <span data-ttu-id="1c80f-1189">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="1c80f-1189">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="1c80f-1190">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1c80f-1190">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1c80f-1191">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1c80f-1191">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1c80f-1192">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1192">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="1c80f-1193">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1193">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="1c80f-1194">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="1c80f-1194">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="1c80f-1195">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-1195">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1c80f-1196">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-1196">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1c80f-1197">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-1197">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="1c80f-1198">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1c80f-1198">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="1c80f-1199">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1199">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1c80f-1200">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="1c80f-1200">Highlights since the last major release</span></span>
* <span data-ttu-id="1c80f-1201">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="1c80f-1201">General availability of `Az` module</span></span>
* <span data-ttu-id="1c80f-1202">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1c80f-1202">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1c80f-1203">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1c80f-1203">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1c80f-1204">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1204">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1c80f-1205">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c80f-1205">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c80f-1206">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1206">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1c80f-1207">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="1c80f-1207">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-1208">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1208">Az.Automation</span></span>
* <span data-ttu-id="1c80f-1209">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="1c80f-1209">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="1c80f-1210">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="1c80f-1210">Dynamic grouping</span></span>
    * <span data-ttu-id="1c80f-1211">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="1c80f-1211">Pre-Post script</span></span>
    * <span data-ttu-id="1c80f-1212">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="1c80f-1212">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1213">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1213">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1214">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="1c80f-1214">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="1c80f-1215">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1215">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c80f-1216">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-1216">Az.KeyVault</span></span>
* <span data-ttu-id="1c80f-1217">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-1217">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1218">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1218">Az.Network</span></span>
* <span data-ttu-id="1c80f-1219">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="1c80f-1219">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="1c80f-1220">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="1c80f-1220">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1221">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1221">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-1222">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="1c80f-1222">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="1c80f-1223">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="1c80f-1223">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1224">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1224">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1225">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-1225">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="1c80f-1226">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="1c80f-1226">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1227">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1227">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1228">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1228">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-1229">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1229">Az.Storage</span></span>
* <span data-ttu-id="1c80f-1230">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1c80f-1230">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="1c80f-1231">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1231">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1c80f-1232">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1232">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1c80f-1233">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1233">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1c80f-1234">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="1c80f-1234">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="1c80f-1235">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="1c80f-1235">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="1c80f-1236">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1236">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1237">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1237">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1238">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1238">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="1c80f-1239">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1239">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1240">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1240">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1241">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="1c80f-1241">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="1c80f-1242">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1242">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-1243">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1243">Az.Automation</span></span>
* <span data-ttu-id="1c80f-1244">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1244">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="1c80f-1245">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1245">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="1c80f-1246">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="1c80f-1246">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c80f-1247">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c80f-1247">Az.Cdn</span></span>
* <span data-ttu-id="1c80f-1248">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1248">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1249">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1249">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1250">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="1c80f-1250">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-1251">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-1251">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-1252">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="1c80f-1252">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c80f-1253">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-1253">Az.LogicApp</span></span>
* <span data-ttu-id="1c80f-1254">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="1c80f-1254">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1255">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1255">Az.Network</span></span>
* <span data-ttu-id="1c80f-1256">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1256">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1257">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1257">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-1258">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1258">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="1c80f-1259">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="1c80f-1259">SDK Update</span></span>
* <span data-ttu-id="1c80f-1260">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="1c80f-1260">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="1c80f-1261">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="1c80f-1261">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1262">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1262">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1263">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="1c80f-1263">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="1c80f-1264">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="1c80f-1264">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="1c80f-1265">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="1c80f-1265">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="1c80f-1266">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="1c80f-1266">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="1c80f-1267">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="1c80f-1267">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="1c80f-1268">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="1c80f-1268">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1269">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1269">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1270">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1270">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="1c80f-1271">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1271">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-1272">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1272">Az.Storage</span></span>
* <span data-ttu-id="1c80f-1273">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1273">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="1c80f-1274">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1274">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="1c80f-1275">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1275">Az.AnalysisServices</span></span>
* <span data-ttu-id="1c80f-1276">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="1c80f-1276">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-1277">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1277">Az.Automation</span></span>
* <span data-ttu-id="1c80f-1278">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1278">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="1c80f-1279">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1279">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="1c80f-1280">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1280">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c80f-1281">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1281">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c80f-1282">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1282">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1283">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1283">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1284">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="1c80f-1284">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="1c80f-1285">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="1c80f-1285">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="1c80f-1286">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1286">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="1c80f-1287">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1287">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1288">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1288">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-1289">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="1c80f-1289">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1c80f-1290">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1290">Az.EventHub</span></span>
* <span data-ttu-id="1c80f-1291">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1291">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="1c80f-1292">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-1292">Az.KeyVault</span></span>
* <span data-ttu-id="1c80f-1293">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="1c80f-1293">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c80f-1294">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-1294">Az.LogicApp</span></span>
* <span data-ttu-id="1c80f-1295">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="1c80f-1295">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="1c80f-1296">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1296">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="1c80f-1297">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="1c80f-1297">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="1c80f-1298">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c80f-1298">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1c80f-1299">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c80f-1299">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1c80f-1300">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c80f-1300">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1c80f-1301">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1c80f-1301">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="1c80f-1302">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="1c80f-1302">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="1c80f-1303">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1303">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1c80f-1304">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1304">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1c80f-1305">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1305">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1c80f-1306">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1306">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="1c80f-1307">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-1307">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1c80f-1308">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1308">Az.Monitor</span></span>
* <span data-ttu-id="1c80f-1309">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="1c80f-1309">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1310">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1310">Az.Network</span></span>
* <span data-ttu-id="1c80f-1311">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="1c80f-1311">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-1312">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-1312">Az.OperationalInsights</span></span>
* <span data-ttu-id="1c80f-1313">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1313">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="1c80f-1314">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1314">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="1c80f-1315">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1315">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="1c80f-1316">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1316">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1317">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1c80f-1317">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1c80f-1318">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1c80f-1318">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="1c80f-1319">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="1c80f-1319">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="1c80f-1320">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="1c80f-1320">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1321">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1321">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1322">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="1c80f-1322">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="1c80f-1323">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="1c80f-1323">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1324">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1324">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1325">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="1c80f-1325">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="1c80f-1326">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1326">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1327">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1327">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1328">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c80f-1328">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1c80f-1329">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1329">Az.AnalysisServices</span></span>
<span data-ttu-id="1c80f-1330">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1330">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1331">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1331">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1332">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="1c80f-1332">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="1c80f-1333">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="1c80f-1333">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="1c80f-1334">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1334">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1335">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1335">Az.RecoveryServices</span></span>
<span data-ttu-id="1c80f-1336">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1336">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1337">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1337">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1338">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="1c80f-1338">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="1c80f-1339">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1c80f-1339">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1c80f-1340">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="1c80f-1340">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="1c80f-1341">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1c80f-1341">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1342">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1342">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1343">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1343">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="1c80f-1344">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="1c80f-1344">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="1c80f-1345">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="1c80f-1345">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="1c80f-1346">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1346">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1347">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1347">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1348">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="1c80f-1348">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1c80f-1349">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1349">Az.AnalysisServices</span></span>
* <span data-ttu-id="1c80f-1350">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="1c80f-1350">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1351">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1351">Az.RecoveryServices</span></span>
* <span data-ttu-id="1c80f-1352">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="1c80f-1352">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="1c80f-1353">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1353">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1354">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1354">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1355">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="1c80f-1355">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1c80f-1356">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1356">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c80f-1357">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="1c80f-1357">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="1c80f-1358">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="1c80f-1358">Az.Aks</span></span>
* <span data-ttu-id="1c80f-1359">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1359">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1c80f-1360">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1360">Az.Automation</span></span>
* <span data-ttu-id="1c80f-1361">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="1c80f-1361">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="1c80f-1362">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1362">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1c80f-1363">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1c80f-1363">Az.Cdn</span></span>
* <span data-ttu-id="1c80f-1364">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1364">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1365">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1365">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1366">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1366">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="1c80f-1367">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="1c80f-1367">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="1c80f-1368">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="1c80f-1368">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="1c80f-1369">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1c80f-1369">Az.ContainerRegistry</span></span>
* <span data-ttu-id="1c80f-1370">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1370">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1c80f-1371">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1c80f-1371">Az.DataFactory</span></span>
* <span data-ttu-id="1c80f-1372">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="1c80f-1372">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1373">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1373">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-1374">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="1c80f-1374">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="1c80f-1375">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="1c80f-1375">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="1c80f-1376">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1376">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-1377">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1377">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-1378">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1378">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1c80f-1379">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-1379">Az.KeyVault</span></span>
* <span data-ttu-id="1c80f-1380">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1380">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1381">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1381">Az.Network</span></span>
* <span data-ttu-id="1c80f-1382">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1382">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1383">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1383">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1384">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1384">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="1c80f-1385">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1385">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="1c80f-1386">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="1c80f-1386">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="1c80f-1387">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="1c80f-1387">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="1c80f-1388">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="1c80f-1388">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="1c80f-1389">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1389">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="1c80f-1390">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="1c80f-1390">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-1391">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-1391">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-1392">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="1c80f-1392">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="1c80f-1393">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1393">Fix some error messages.</span></span>
* <span data-ttu-id="1c80f-1394">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1394">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="1c80f-1395">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1395">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1c80f-1396">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1c80f-1396">Az.SignalR</span></span>
* <span data-ttu-id="1c80f-1397">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1397">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1398">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1399">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1399">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c80f-1400">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="1c80f-1400">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="1c80f-1401">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="1c80f-1401">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="1c80f-1402">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="1c80f-1402">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-1403">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1403">Az.Storage</span></span>
* <span data-ttu-id="1c80f-1404">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1404">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c80f-1405">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1405">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="1c80f-1406">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="1c80f-1406">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="1c80f-1407">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="1c80f-1407">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="1c80f-1408">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1c80f-1408">Az.TrafficManager</span></span>
* <span data-ttu-id="1c80f-1409">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1409">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1410">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1410">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1411">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1411">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1c80f-1412">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1412">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="1c80f-1413">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="1c80f-1413">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="1c80f-1414">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1c80f-1414">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1c80f-1415">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1415">Az.Accounts</span></span>
* <span data-ttu-id="1c80f-1416">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="1c80f-1416">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1417">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1418">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1418">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="1c80f-1419">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="1c80f-1419">Updated the description of ID in help files</span></span>
* <span data-ttu-id="1c80f-1420">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1420">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1421">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1421">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-1422">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1422">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="1c80f-1423">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="1c80f-1423">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1c80f-1424">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1c80f-1424">Az.EventGrid</span></span>
* <span data-ttu-id="1c80f-1425">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1425">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="1c80f-1426">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="1c80f-1426">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="1c80f-1427">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="1c80f-1427">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1c80f-1428">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="1c80f-1428">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1c80f-1429">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="1c80f-1429">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1c80f-1430">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1430">Dead letter endpoint.</span></span>
    - <span data-ttu-id="1c80f-1431">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="1c80f-1431">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1c80f-1432">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="1c80f-1432">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1c80f-1433">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="1c80f-1433">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1c80f-1434">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1434">Dead letter endpoint.</span></span>
* <span data-ttu-id="1c80f-1435">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1435">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="1c80f-1436">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1436">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1c80f-1437">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1437">Az.IotHub</span></span>
* <span data-ttu-id="1c80f-1438">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="1c80f-1438">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1c80f-1439">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1c80f-1439">Az.LogicApp</span></span>
* <span data-ttu-id="1c80f-1440">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="1c80f-1440">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1441">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1441">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1442">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1442">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="1c80f-1443">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="1c80f-1443">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="1c80f-1444">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="1c80f-1444">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1c80f-1445">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="1c80f-1445">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="1c80f-1446">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1446">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="1c80f-1447">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="1c80f-1447">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1c80f-1448">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1c80f-1448">Az.SignalR</span></span>
* <span data-ttu-id="1c80f-1449">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1449">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1450">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1450">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1451">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1451">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1c80f-1452">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1452">Az.Storage</span></span>
* <span data-ttu-id="1c80f-1453">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="1c80f-1453">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="1c80f-1454">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1c80f-1454">New-AzStorageContext</span></span>
* <span data-ttu-id="1c80f-1455">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="1c80f-1455">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="1c80f-1456">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="1c80f-1456">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1457">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1457">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1458">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1458">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="1c80f-1459">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1459">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="1c80f-1460">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1460">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="1c80f-1461">Geral</span><span class="sxs-lookup"><span data-stu-id="1c80f-1461">General</span></span>

- <span data-ttu-id="1c80f-1462">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="1c80f-1462">General Availability of Az Module</span></span>
- <span data-ttu-id="1c80f-1463">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="1c80f-1463">Online help for each module</span></span>
- <span data-ttu-id="1c80f-1464">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="1c80f-1464">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="1c80f-1465">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="1c80f-1465">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="1c80f-1466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1466">Az.Accounts</span></span>
- <span data-ttu-id="1c80f-1467">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1467">Changed from Az.Profile</span></span>
- <span data-ttu-id="1c80f-1468">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="1c80f-1468">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1c80f-1469">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-1469">Az.ApiManagement</span></span>
- <span data-ttu-id="1c80f-1470">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="1c80f-1470">Fixes for #7002</span></span>
- <span data-ttu-id="1c80f-1471">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1471">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="1c80f-1472">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1c80f-1472">Az.Batch</span></span>
- <span data-ttu-id="1c80f-1473">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1473">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="1c80f-1474">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1474">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="1c80f-1475">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1475">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="1c80f-1476">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="1c80f-1476">Az.Billing</span></span>
- <span data-ttu-id="1c80f-1477">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1477">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="1c80f-1478">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1478">Az.CognitivServices</span></span>
- <span data-ttu-id="1c80f-1479">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1479">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="1c80f-1480">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="1c80f-1480">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1c80f-1481">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1481">Az.ContainerInstance</span></span>
- <span data-ttu-id="1c80f-1482">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="1c80f-1482">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="1c80f-1483">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1c80f-1483">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="1c80f-1484">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1484">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1485">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1485">Az.DataLakeStore</span></span>
- <span data-ttu-id="1c80f-1486">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1486">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="1c80f-1487">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1487">Az.Monitor</span></span>
- <span data-ttu-id="1c80f-1488">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1488">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="1c80f-1489">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1c80f-1489">Az.KeyVault</span></span>
- <span data-ttu-id="1c80f-1490">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="1c80f-1490">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="1c80f-1491">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1c80f-1491">Az.MachineLearning</span></span>
- <span data-ttu-id="1c80f-1492">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1492">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="1c80f-1493">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1c80f-1493">Az.Media</span></span>
- <span data-ttu-id="1c80f-1494">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="1c80f-1494">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1c80f-1495">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1495">Az.Network</span></span>
<span data-ttu-id="1c80f-1496">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="1c80f-1496">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="1c80f-1497">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="1c80f-1497">New cmdlets added:</span></span>
        - <span data-ttu-id="1c80f-1498">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1498">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c80f-1499">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1499">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c80f-1500">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1500">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c80f-1501">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1501">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c80f-1502">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1502">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1c80f-1503">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1503">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="1c80f-1504">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1504">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="1c80f-1505">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c80f-1505">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="1c80f-1506">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1506">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="1c80f-1507">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1c80f-1507">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="1c80f-1508">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1508">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1c80f-1509">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1c80f-1509">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1c80f-1510">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-1510">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="1c80f-1511">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-1511">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="1c80f-1512">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1512">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="1c80f-1513">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="1c80f-1513">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="1c80f-1514">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1c80f-1514">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1c80f-1515">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1c80f-1515">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1c80f-1516">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1c80f-1516">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="1c80f-1517">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="1c80f-1517">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="1c80f-1518">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1518">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="1c80f-1519">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-1519">Az.OperationalInsights</span></span>
- <span data-ttu-id="1c80f-1520">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1520">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="1c80f-1521">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1521">Az.Profile</span></span>
- <span data-ttu-id="1c80f-1522">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1c80f-1522">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1523">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1523">Az.RecoveryServices</span></span>
- <span data-ttu-id="1c80f-1524">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1524">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="1c80f-1525">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1525">Az.Resources</span></span>
- <span data-ttu-id="1c80f-1526">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1526">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1c80f-1527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-1527">Az.ServiceFabric</span></span>
- <span data-ttu-id="1c80f-1528">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="1c80f-1528">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="1c80f-1529">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1529">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="1c80f-1530">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="1c80f-1530">Az.SIgnalR</span></span>
- <span data-ttu-id="1c80f-1531">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="1c80f-1531">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="1c80f-1532">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1532">Az.Sql</span></span>
- <span data-ttu-id="1c80f-1533">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="1c80f-1533">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="1c80f-1534">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="1c80f-1534">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="1c80f-1535">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1535">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="1c80f-1536">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1536">Az.Storage</span></span>
- <span data-ttu-id="1c80f-1537">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1537">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1c80f-1538">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1538">Az.Websites</span></span>
- <span data-ttu-id="1c80f-1539">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="1c80f-1539">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="1c80f-1540">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1540">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="1c80f-1541">Geral</span><span class="sxs-lookup"><span data-stu-id="1c80f-1541">General</span></span>

* <span data-ttu-id="1c80f-1542">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="1c80f-1542">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="1c80f-1543">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1543">Az.Compute</span></span>

* <span data-ttu-id="1c80f-1544">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1544">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1545">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1545">Az.DataLakeStore</span></span>

* <span data-ttu-id="1c80f-1546">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="1c80f-1546">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="1c80f-1547">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1547">Az.FrontDoor</span></span>

* <span data-ttu-id="1c80f-1548">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="1c80f-1548">Fixed some broken links</span></span>
    - <span data-ttu-id="1c80f-1549">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1549">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="1c80f-1550">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1550">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1c80f-1551">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1551">Az.RecoveryServices</span></span>

* <span data-ttu-id="1c80f-1552">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1552">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="1c80f-1553">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1553">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="1c80f-1554">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1554">Az.Resources</span></span>

* <span data-ttu-id="1c80f-1555">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="1c80f-1555">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="1c80f-1556">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1556">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="1c80f-1557">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1557">Az.Sql</span></span>

* <span data-ttu-id="1c80f-1558">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="1c80f-1558">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="1c80f-1559">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="1c80f-1559">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="1c80f-1560">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1560">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="1c80f-1561">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1561">Az.Storage</span></span>

* <span data-ttu-id="1c80f-1562">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1c80f-1562">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="1c80f-1563">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="1c80f-1563">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="1c80f-1564">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1564">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1c80f-1565">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="1c80f-1565">Support Static Website configuration</span></span>
    - <span data-ttu-id="1c80f-1566">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1c80f-1566">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="1c80f-1567">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1c80f-1567">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1c80f-1568">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1568">Az.Websites</span></span>

* <span data-ttu-id="1c80f-1569">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="1c80f-1569">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="1c80f-1570">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1570">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="1c80f-1571">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1571">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="1c80f-1572">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1572">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1c80f-1573">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1c80f-1573">Az.ApiManagement</span></span>
* <span data-ttu-id="1c80f-1574">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1574">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="1c80f-1575">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1c80f-1575">Az.Automation</span></span>
* <span data-ttu-id="1c80f-1576">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="1c80f-1576">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="1c80f-1577">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="1c80f-1577">Added Update Management cmdlets</span></span>
* <span data-ttu-id="1c80f-1578">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="1c80f-1578">Added Source Control cmdlets</span></span>
* <span data-ttu-id="1c80f-1579">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="1c80f-1579">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="1c80f-1580">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="1c80f-1580">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="1c80f-1581">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1581">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1582">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="1c80f-1582">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="1c80f-1583">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1583">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1c80f-1584">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1584">Az.ContainerInstance</span></span>
* <span data-ttu-id="1c80f-1585">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1585">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="1c80f-1586">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1c80f-1586">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="1c80f-1587">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="1c80f-1587">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1c80f-1588">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1588">Az.Network</span></span>
* <span data-ttu-id="1c80f-1589">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="1c80f-1589">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="1c80f-1590">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="1c80f-1590">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="1c80f-1591">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1591">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="1c80f-1592">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="1c80f-1592">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="1c80f-1593">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1c80f-1593">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1c80f-1594">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1594">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="1c80f-1595">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1595">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="1c80f-1596">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1c80f-1596">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="1c80f-1597">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="1c80f-1597">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="1c80f-1598">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="1c80f-1598">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="1c80f-1599">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="1c80f-1599">Az.Relay</span></span>
* <span data-ttu-id="1c80f-1600">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1600">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="1c80f-1601">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1601">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1602">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="1c80f-1602">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="1c80f-1603">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="1c80f-1603">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="1c80f-1604">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="1c80f-1604">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1c80f-1605">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-1605">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-1606">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="1c80f-1606">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="1c80f-1607">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1607">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1608">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1608">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="1c80f-1609">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1609">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c80f-1610">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1610">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c80f-1611">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1611">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c80f-1612">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1c80f-1612">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1c80f-1613">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c80f-1613">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1c80f-1614">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c80f-1614">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1c80f-1615">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c80f-1615">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1c80f-1616">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1c80f-1616">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="1c80f-1617">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1617">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="1c80f-1618">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1618">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="1c80f-1619">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1619">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="1c80f-1620">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1620">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1c80f-1621">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1621">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1c80f-1622">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1622">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="1c80f-1623">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1623">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="1c80f-1624">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="1c80f-1624">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="1c80f-1625">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1625">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1c80f-1626">Geral</span><span class="sxs-lookup"><span data-stu-id="1c80f-1626">General</span></span>
* <span data-ttu-id="1c80f-1627">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="1c80f-1627">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="1c80f-1628">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1628">Az.Profile</span></span>
* <span data-ttu-id="1c80f-1629">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c80f-1629">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="1c80f-1630">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="1c80f-1630">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="1c80f-1631">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="1c80f-1631">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="1c80f-1632">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="1c80f-1632">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="1c80f-1633">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="1c80f-1633">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="1c80f-1634">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="1c80f-1634">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="1c80f-1635">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="1c80f-1635">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="1c80f-1636">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1636">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c80f-1637">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1637">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1638">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1638">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1639">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="1c80f-1639">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="1c80f-1640">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="1c80f-1640">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="1c80f-1641">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1641">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1642">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1642">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-1643">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1643">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="1c80f-1644">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1644">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="1c80f-1645">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="1c80f-1645">Az.Insights</span></span>
* <span data-ttu-id="1c80f-1646">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="1c80f-1646">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="1c80f-1647">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="1c80f-1647">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="1c80f-1648">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="1c80f-1648">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="1c80f-1649">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="1c80f-1649">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1650">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1650">Az.Network</span></span>
* <span data-ttu-id="1c80f-1651">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="1c80f-1651">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="1c80f-1652">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-1652">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="1c80f-1653">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-1653">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="1c80f-1654">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1c80f-1654">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="1c80f-1655">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-1655">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="1c80f-1656">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="1c80f-1656">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="1c80f-1657">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1c80f-1657">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1c80f-1658">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1c80f-1658">Az.PolicyInsights</span></span>
* <span data-ttu-id="1c80f-1659">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="1c80f-1659">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1660">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1660">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1661">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="1c80f-1661">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="1c80f-1662">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1662">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1c80f-1663">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1c80f-1663">Az.ServiceBus</span></span>
* <span data-ttu-id="1c80f-1664">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1664">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1c80f-1665">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1c80f-1665">Az.ServiceFabric</span></span>
* <span data-ttu-id="1c80f-1666">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1666">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="1c80f-1667">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1667">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="1c80f-1668">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="1c80f-1668">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="1c80f-1669">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="1c80f-1669">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="1c80f-1670">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1670">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="1c80f-1671">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1671">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="1c80f-1672">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1672">Az.Profile</span></span>
* <span data-ttu-id="1c80f-1673">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="1c80f-1673">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="1c80f-1674">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="1c80f-1674">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1675">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1675">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1676">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="1c80f-1676">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="1c80f-1677">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1677">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1c80f-1678">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1c80f-1678">Az.DataLakeStore</span></span>
* <span data-ttu-id="1c80f-1679">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="1c80f-1679">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="1c80f-1680">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1680">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="1c80f-1681">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1681">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1c80f-1682">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1682">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1c80f-1683">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1683">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1684">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1684">Az.Network</span></span>
* <span data-ttu-id="1c80f-1685">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1685">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="1c80f-1686">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1686">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1687">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1687">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1688">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1688">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="1c80f-1689">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="1c80f-1689">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="1c80f-1690">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1690">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="1c80f-1691">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1691">Azure.Storage</span></span>
* <span data-ttu-id="1c80f-1692">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="1c80f-1692">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="1c80f-1693">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1693">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="1c80f-1694">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1c80f-1694">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1c80f-1695">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1695">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="1c80f-1696">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="1c80f-1696">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="1c80f-1697">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1c80f-1697">Az.CognitiveServices</span></span>
* <span data-ttu-id="1c80f-1698">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1698">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1c80f-1699">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1c80f-1699">Az.Compute</span></span>
* <span data-ttu-id="1c80f-1700">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="1c80f-1700">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="1c80f-1701">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1701">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="1c80f-1702">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="1c80f-1702">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="1c80f-1703">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1c80f-1703">Az.DataFactoryV2</span></span>
* <span data-ttu-id="1c80f-1704">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1704">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1c80f-1705">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1c80f-1705">Az.Network</span></span>
* <span data-ttu-id="1c80f-1706">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1706">Added NetworkProfile functionality.</span></span> <span data-ttu-id="1c80f-1707">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="1c80f-1707">new cmdlets added</span></span>
    - <span data-ttu-id="1c80f-1708">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1708">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c80f-1709">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1709">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c80f-1710">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1710">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c80f-1711">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1c80f-1711">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="1c80f-1712">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-1712">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="1c80f-1713">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-1713">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="1c80f-1714">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="1c80f-1714">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="1c80f-1715">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="1c80f-1715">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="1c80f-1716">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="1c80f-1716">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1c80f-1717">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1c80f-1717">Az.RedisCache</span></span>
* <span data-ttu-id="1c80f-1718">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="1c80f-1718">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="1c80f-1719">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="1c80f-1719">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="1c80f-1720">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1c80f-1720">Az.Resources</span></span>
* <span data-ttu-id="1c80f-1721">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="1c80f-1721">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1c80f-1722">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="1c80f-1722">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="1c80f-1723">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1c80f-1723">Az.Sql</span></span>
* <span data-ttu-id="1c80f-1724">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="1c80f-1724">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1c80f-1725">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1c80f-1725">Az.Websites</span></span>
* <span data-ttu-id="1c80f-1726">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="1c80f-1726">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="1c80f-1727">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="1c80f-1727">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="1c80f-1728">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1c80f-1728">0.2.0 - September 2018</span></span>
 <span data-ttu-id="1c80f-1729">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="1c80f-1729">Initial Release</span></span>
