---
title: Guia de migração para o Az 3.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 3.0.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/04/2019
ms.openlocfilehash: 06be35bc3573d00d90a8cf2d822ac051ab72f6bb
ms.sourcegitcommit: 5523170e571fbd1dc93bd0fa4223aba3b324d3b0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/25/2020
ms.locfileid: "85363459"
---
# <a name="migration-guide-for-az-300"></a><span data-ttu-id="18b25-103">Guia de migração para o Az 3.0.0</span><span class="sxs-lookup"><span data-stu-id="18b25-103">Migration Guide for Az 3.0.0</span></span>

<span data-ttu-id="18b25-104">Este documento descreve as alterações realizadas entre as versões 2.0.0 e 3.0.0 do Az</span><span class="sxs-lookup"><span data-stu-id="18b25-104">This document describes the changes between the 2.0.0 and 3.0.0 versions of Az</span></span>

<!-- TOC -->

- [<span data-ttu-id="18b25-105">Guia de migração para o Az 3.0.0</span><span class="sxs-lookup"><span data-stu-id="18b25-105">Migration Guide for Az 3.0.0</span></span>](#migration-guide-for-az-300)
  - [<span data-ttu-id="18b25-106">Batch</span><span class="sxs-lookup"><span data-stu-id="18b25-106">Batch</span></span>](#batch)
    - [`Get-AzBatchNodeAgentSku`](#get-azbatchnodeagentsku)
    - [<span data-ttu-id="18b25-107">Incompatibilidade com as versões anteriores do `Az.Resources`</span><span class="sxs-lookup"><span data-stu-id="18b25-107">Incompatibility with previous versions of `Az.Resources`</span></span>](#previous-version-incompatibility-with-azresources-module)
  - [<span data-ttu-id="18b25-108">Computação</span><span class="sxs-lookup"><span data-stu-id="18b25-108">Compute</span></span>](#compute)
    - [`New-AzDiskConfig`](#new-azdiskconfig)
  - [<span data-ttu-id="18b25-109">HDInsight</span><span class="sxs-lookup"><span data-stu-id="18b25-109">HDInsight</span></span>](#hdinsight)
    - [`Get-AzHDInsightJobOutput`](#get-azhdinsightjoboutput)
    - [`Add-AzHDInsightConfigValues`](#add-azhdinsightconfigvalues)
    - [`Disable-AzHDInsightMonitoring`](#disable-azhdinsightmonitoring)
    - [`Enable-AzHDInsightMonitoring`](#enable-azhdinsightmonitoring)
    - [`Get-AzHDInsightMonitoring`](#get-azhdinsightmonitoring)
    - [`Get-AzHDInsightProperty`](#get-azhdinsightproperty)
    - [`Grant-AzHDInsightRdpServicesAccess`](#grant-azhdinsightrdpservicesaccess)
    - [`Remove-AzHDInsightCluster`](#remove-azhdinsightcluster)
    - [`Revoke-AzHDInsightRdpServicesAccess`](#revoke-azhdinsightrdpservicesaccess)
    - [`Set-AzHDInsightGatewayCredential`](#set-azhdinsightgatewaycredential)
  - [<span data-ttu-id="18b25-110">IotHub</span><span class="sxs-lookup"><span data-stu-id="18b25-110">IotHub</span></span>](#iothub)
    - [`New-AzIotHubImportDevices`](#new-aziothubimportdevices)
    - [`New-AzIotHubExportDevices`](#new-aziothubexportdevices)
    - [`Add-AzIotHubEventHubConsumerGroup`](#add-aziothubeventhubconsumergroup)
    - [`Get-AzIotHubEventHubConsumerGroup`](#get-aziothubeventhubconsumergroup)
    - [`Remove-AzIotHubEventHubConsumerGroup`](#remove-aziothubeventhubconsumergroup)
    - [`Set-AzIotHub`](#set-aziothub)
  - [<span data-ttu-id="18b25-111">RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="18b25-111">RecoveryServices</span></span>](#recoveryservices)
    - [`Edit-AzRecoveryServicesAsrRecoveryPlan`](#edit-azrecoveryservicesasrrecoveryplan)
    - [`Get-AzRecoveryServicesAsrRecoveryPlan`](#get-azrecoveryservicesasrrecoveryplan)
    - [`New-AzRecoveryServicesAsrReplicationProtectedItem`](#new-azrecoveryservicesasrreplicationprotecteditem)
  - [<span data-ttu-id="18b25-112">Recursos</span><span class="sxs-lookup"><span data-stu-id="18b25-112">Resources</span></span>](#resources)
    - [<span data-ttu-id="18b25-113">Incompatibilidade com as versões anteriores do `Az.Batch`</span><span class="sxs-lookup"><span data-stu-id="18b25-113">Incompatibility with previous versions of `Az.Batch`</span></span>](#previous-version-incompatibility-with-azbatch-module)
  - [<span data-ttu-id="18b25-114">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="18b25-114">ServiceFabric</span></span>](#servicefabric)
    - [`Add-ServiceFabricApplicationCertificate`](#add-servicefabricapplicationcertificate)
  - [<span data-ttu-id="18b25-115">Sql</span><span class="sxs-lookup"><span data-stu-id="18b25-115">Sql</span></span>](#sql)
    - [`Get-AzSqlDatabaseSecureConnectionPolicy`](#get-azsqldatabasesecureconnectionpolicy)
    - [`Get-AzSqlDatabaseIndexRecommendations`](#get-azsqldatabaseindexrecommendations)
    - [`Get-AzSqlDatabaseRestorePoints`](#get-azsqldatabaserestorepoints)
    - [`Get-AzSqlDatabaseAuditing`](#get-azsqldatabaseauditing)
    - [`Set-AzSqlDatabaseAuditing`](#set-azsqldatabaseauditing)
    - [`Get-AzSqlServerAuditing`](#get-azsqlserverauditing)
    - [`Set-AzSqlServerAuditing`](#set-azsqlserverauditing)
    - [`Get-AzSqlServerAdvancedThreatProtectionSettings`](#get-azsqlserveradvancedthreatprotectionsettings)
    - [`Clear-AzSqlServerAdvancedThreatProtectionSettings`](#clear-azsqlserveradvancedthreatprotectionsettings)
    - [`Update-AzSqlServerAdvancedThreatProtectionSettings`](#update-azsqlserveradvancedthreatprotectionsettings)
    - [`Get-AzSqlDatabaseAdvancedThreatProtectionSettings`](#get-azsqldatabaseadvancedthreatprotectionsettings)
    - [`Update-AzSqlDatabaseAdvancedThreatProtectionSettings`](#update-azsqldatabaseadvancedthreatprotectionsettings)
    - [`Clear-AzSqlDatabaseAdvancedThreatProtectionSettings`](#clear-azsqldatabaseadvancedthreatprotectionsettings)
    - [`Update-AzSqlDatabaseVulnerabilityAssessmentSettings`](#update-azsqldatabasevulnerabilityassessmentsettings)
    - [`Get-AzSqlDatabaseVulnerabilityAssessmentSettings`](#get-azsqldatabasevulnerabilityassessmentsettings)
    - [`Clear-AzSqlDatabaseVulnerabilityAssessmentSettings`](#clear-azsqldatabasevulnerabilityassessmentsettings)
    - [`Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`](#update-azsqlinstancedatabasevulnerabilityassessmentsettings)
    - [`Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`](#get-azsqlinstancedatabasevulnerabilityassessmentsettings)
    - [`Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`](#clear-azsqlinstancedatabasevulnerabilityassessmentsettings)
    - [`Update-AzSqlInstanceVulnerabilityAssessmentSettings`](#update-azsqlinstancevulnerabilityassessmentsettings)
    - [`Get-AzSqlInstanceVulnerabilityAssessmentSettings`](#get-azsqlinstancevulnerabilityassessmentsettings)
    - [`Clear-AzSqlInstanceVulnerabilityAssessmentSettings`](#clear-azsqlinstancevulnerabilityassessmentsettings)
    - [`Update-AzSqlServerVulnerabilityAssessmentSettings`](#update-azsqlservervulnerabilityassessmentsettings)
    - [`Get-AzSqlServerVulnerabilityAssessmentSettings`](#get-azsqlservervulnerabilityassessmentsettings)
    - [`Clear-AzSqlServerVulnerabilityAssessmentSettings`](#clear-azsqlservervulnerabilityassessmentsettings)
    - [`Get-AzSqlServerAdvancedThreatProtectionPolicy`](#get-azsqlserveradvancedthreatprotectionpolicy)
    - [`Get-AzSqlServerThreatDetectionPolicy`](#get-azsqlserverthreatdetectionpolicy)
    - [`Remove-AzSqlServerThreatDetectionPolicy`](#remove-azsqlserverthreatdetectionpolicy)
    - [`Set-AzSqlServerThreatDetectionPolicy`](#set-azsqlserverthreatdetectionpolicy)
    - [`Get-AzSqlDatabaseThreatDetectionPolicy`](#get-azsqldatabasethreatdetectionpolicy)
    - [`Set-AzSqlDatabaseThreatDetectionPolicy`](#set-azsqldatabasethreatdetectionpolicy)
    - [`Remove-AzSqlDatabaseThreatDetectionPolicy`](#remove-azsqldatabasethreatdetectionpolicy)

<!-- /TOC -->


## <a name="batch"></a><span data-ttu-id="18b25-116">Batch</span><span class="sxs-lookup"><span data-stu-id="18b25-116">Batch</span></span>

### `Get-AzBatchNodeAgentSku`
- <span data-ttu-id="18b25-117">`Get-AzBatchNodeAgentSku` foi removido e substituído por `Get-AzBatchSupportedImage`.</span><span class="sxs-lookup"><span data-stu-id="18b25-117">Removed `Get-AzBatchNodeAgentSku` and replaced it with  `Get-AzBatchSupportedImage`.</span></span>
- <span data-ttu-id="18b25-118">`Get-AzBatchSupportedImage` devolve os mesmos dados que `Get-AzBatchNodeAgentSku`, mas num formato mais amigável.</span><span class="sxs-lookup"><span data-stu-id="18b25-118">`Get-AzBatchSupportedImage` returns the same data as `Get-AzBatchNodeAgentSku` but in a more friendly format.</span></span>
- <span data-ttu-id="18b25-119">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="18b25-119">New non-verified images are also now returned.</span></span> <span data-ttu-id="18b25-120">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="18b25-120">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-121">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-121">Before</span></span>
```powershell
$Context = Get-AzBatchAccountKeys -AccountName "ContosoBatchAccount"
Get-AzBatchNodeAgentSku -BatchContext $Context
```

#### <a name="after"></a><span data-ttu-id="18b25-122">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-122">After</span></span>
```powershell
$Context = Get-AzBatchAccountKey -AccountName "ContosoBatchAccount"
Get-AzBatchSupportedImage -BatchContext $Context
```
### <a name="previous-version-incompatibility-with-azresources-module"></a><span data-ttu-id="18b25-123">Incompatibilidade com as versões anteriores do módulo Az.Resources</span><span class="sxs-lookup"><span data-stu-id="18b25-123">Previous Version Incompatibility with Az.Resources Module</span></span>
<span data-ttu-id="18b25-124">A versão 2.0.1 do módulo "Az.Batch" é incompatível com as versões anteriores (versão 1.7.0 ou anterior) do módulo "AZ.Resources".</span><span class="sxs-lookup"><span data-stu-id="18b25-124">Version 2.0.1 of the ‘Az.Batch’ module is incompatible with earlier versions (version 1.7.0 or earlier) of the ‘Az.Resources’ module.</span></span>  <span data-ttu-id="18b25-125">Isto resultará na incapacidade de importar a versão 1.7.0 do módulo "Az.Resources" quando a versão 2.0.1 do módulo "Az.Batch" for importada.</span><span class="sxs-lookup"><span data-stu-id="18b25-125">This will result in being unable to import  version 1.7.0 of the ‘Az.Resources’ module when version 2.0.1 of the ‘Az.Batch’ module is imported.</span></span>  <span data-ttu-id="18b25-126">Para corrigir este problema, basta atualizar o módulo "Az.Resources" para a versão 1.7.1 ou posterior, ou simplesmente instalar a versão mais recente do módulo "Az".</span><span class="sxs-lookup"><span data-stu-id="18b25-126">To fix this issue, simply update the ‘Az.Resources’ module to version 1.7.1 or greater, or simply install the latest version of the ‘Az’ module.</span></span>

## <a name="compute"></a><span data-ttu-id="18b25-127">Computação</span><span class="sxs-lookup"><span data-stu-id="18b25-127">Compute</span></span>

### `New-AzDiskConfig`
<span data-ttu-id="18b25-128">É utilizado o parâmetro `UploadSizeInBytes` em vez de `DiskSizeGB` para `New-AzDiskConfig` quando CreateOption for Upload</span><span class="sxs-lookup"><span data-stu-id="18b25-128">`UploadSizeInBytes` parameter is used instead of `DiskSizeGB` for `New-AzDiskConfig` when CreateOption is Upload</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-129">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-129">Before</span></span>
```powershell
$diskconfig = New-AzDiskConfig -Location 'Central US' -DiskSizeGB 1023 -SkuName Standard_LRS -OsType Windows -CreateOption Upload -DiskIOPSReadWrite 500 -DiskMBpsReadWrite 8
```

#### <a name="after"></a><span data-ttu-id="18b25-130">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-130">After</span></span>
```powershell
$diskconfig = New-AzDiskConfig -Location 'Central US' -UploadSizeInBytes 1023 * 1024 * 1024 * 1024 -SkuName Standard_LRS -OsType Windows -CreateOption Upload -DiskIOPSReadWrite 500 -DiskMBpsReadWrite 8
```

## <a name="hdinsight"></a><span data-ttu-id="18b25-131">HDInsight</span><span class="sxs-lookup"><span data-stu-id="18b25-131">HDInsight</span></span>

### `Get-AzHDInsightJobOutput`
- <span data-ttu-id="18b25-132">Foi atualizado o cmdlet `Get-AzHDInsightJobOutput` para suportar acesso granular baseado em funções à chave de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="18b25-132">Updated the `Get-AzHDInsightJobOutput` cmdlet to support granular role-based access to the storage key.</span></span>
- <span data-ttu-id="18b25-133">Os utilizadores com as funções Operador de Clusters, Contribuidor ou Proprietário do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="18b25-133">Users with HDInsight Cluster Operator, Contributor, or Owner roles will not be affected.</span></span>
- <span data-ttu-id="18b25-134">Os utilizadores apenas com a função Leitor terão de especificar o parâmetro `DefaultStorageAccountKey` explicitamente.</span><span class="sxs-lookup"><span data-stu-id="18b25-134">Users with only the Reader role will need to specify `DefaultStorageAccountKey` parameter explicitly.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-135">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-135">Before</span></span>
```powershell
Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId
```

#### <a name="after"></a><span data-ttu-id="18b25-136">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-136">After</span></span>
```powershell
Get-AzHDInsightJobOutput -ClusterName $clusterName -JobId $jobId -DefaultStorageAccountKey $storageAccountKey
```

### `Add-AzHDInsightConfigValues`
<span data-ttu-id="18b25-137">O cmdlet `Add-AzHDInsightConfigValue` removeu o alias para `Add-AzHDInsightConfigValues`.</span><span class="sxs-lookup"><span data-stu-id="18b25-137">Cmdlet `Add-AzHDInsightConfigValue` removed alias to `Add-AzHDInsightConfigValues`.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-138">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-138">Before</span></span>
<span data-ttu-id="18b25-139">Utilização de alias preterido</span><span class="sxs-lookup"><span data-stu-id="18b25-139">Using deprecated alias</span></span>
```powershell
Add-AzHDInsightConfigValues
```

#### <a name="after"></a><span data-ttu-id="18b25-140">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-140">After</span></span>
```powershell
Add-AzHDInsightConfigValue
```


### `Disable-AzHDInsightMonitoring`
<span data-ttu-id="18b25-141">Foi adicionado um novo cmdlet `Disable-AzHDInsightMonitoring`.</span><span class="sxs-lookup"><span data-stu-id="18b25-141">Added a new `Disable-AzHDInsightMonitoring` cmdlet.</span></span> <span data-ttu-id="18b25-142">Utilize este cmdlet para desativar a monitorização num cluster do HDInsight (substitui `Disable-AzHDInsightOperationsManagementSuite` e `Disable-AzHDInsightOMS`).</span><span class="sxs-lookup"><span data-stu-id="18b25-142">Use this cmdlet to disable monitoring in a HDInsight cluster (replaces `Disable-AzHDInsightOperationsManagementSuite` and `Disable-AzHDInsightOMS`).</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-143">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-143">Before</span></span>
```powershell
Disable-AzHDInsightOMS -Name testcluster
```
```powershell
Disable-AzHDInsightOperationsManagementSuite -Name testcluster
```

#### <a name="after"></a><span data-ttu-id="18b25-144">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-144">After</span></span>
```powershell
Disable-AzHDInsightMonitoring -Name testcluster
```


### `Enable-AzHDInsightMonitoring`
<span data-ttu-id="18b25-145">Foi adicionado um novo cmdlet `Enable-AzHDInsightMonitoring`.</span><span class="sxs-lookup"><span data-stu-id="18b25-145">Added a new `Enable-AzHDInsightMonitoring` cmdlet.</span></span> <span data-ttu-id="18b25-146">Utilize este cmdlet para ativar a monitorização num cluster do HDInsight (substitui `Enable-AzHDInsightOperationsManagementSuite` e `Enable-AzHDInsightOMS`).</span><span class="sxs-lookup"><span data-stu-id="18b25-146">Use this cmdlet to enable monitoring in a HDInsight cluster (replaces `Enable-AzHDInsightOperationsManagementSuite` and `Enable-AzHDInsightOMS`).</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-147">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-147">Before</span></span>
```powershell
Enable-AzHDInsightOMS Enable-AzHDInsightMonitoring -Name testcluster -WorkspaceId 1d364e89-bb71-4503-aa3d-a23535aea7bd -PrimaryKey <key for workspace 1d364e89-bb71-4503-aa3d-a23535aea7bd>
```
```powershell
Enable-AzHDInsightOperationsManagementSuite Enable-AzHDInsightMonitoring -Name testcluster -WorkspaceId 1d364e89-bb71-4503-aa3d-a23535aea7bd -PrimaryKey <key for workspace 1d364e89-bb71-4503-aa3d-a23535aea7bd>
```

#### <a name="after"></a><span data-ttu-id="18b25-148">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-148">After</span></span>
```powershell
Enable-AzHDInsightMonitoring Enable-AzHDInsightMonitoring -Name testcluster -WorkspaceId 1d364e89-bb71-4503-aa3d-a23535aea7bd -PrimaryKey <key for workspace 1d364e89-bb71-4503-aa3d-a23535aea7bd>
```

### `Get-AzHDInsightMonitoring`
<span data-ttu-id="18b25-149">Foi adicionado um novo cmdlet `Get-AzHDInsightMonitoring`.</span><span class="sxs-lookup"><span data-stu-id="18b25-149">Added a new `Get-AzHDInsightMonitoring` cmdlet.</span></span> <span data-ttu-id="18b25-150">Utilize este cmdlet para obter o estado de monitorização da instalação num cluster do Azure HDInsight (substitui `Get-AzHDInsightOperationsManagementSuite` e `Get-AzHDInsightOMS`).</span><span class="sxs-lookup"><span data-stu-id="18b25-150">Use this cmdlet to get the status of monitoring installation in an Azure HDInsight cluster (replaces `Get-AzHDInsightOperationsManagementSuite` and `Get-AzHDInsightOMS`).</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-151">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-151">Before</span></span>
```powershell
Get-AzHDInsightOMS -Name testcluster
```
```powershell
Get-AzHDInsightOperationsManagementSuite -Name testcluster
```

#### <a name="after"></a><span data-ttu-id="18b25-152">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-152">After</span></span>
```powershell
Get-AzHDInsightMonitoring -Name testcluster
```

### `Get-AzHDInsightProperty`
<span data-ttu-id="18b25-153">O cmdlet `Get-HDInsightProperty` removeu o alias para `Get-AzHDInsightProperties`.</span><span class="sxs-lookup"><span data-stu-id="18b25-153">Cmdlet `Get-HDInsightProperty` removed alias to `Get-AzHDInsightProperties`.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-154">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-154">Before</span></span>
<span data-ttu-id="18b25-155">Utilização de alias preterido</span><span class="sxs-lookup"><span data-stu-id="18b25-155">Using deprecated alias</span></span>
```powershell
Get-AzHDInsightProperties -Location "East US 2"
```

#### <a name="after"></a><span data-ttu-id="18b25-156">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-156">After</span></span>
```powershell
Get-AzHDInsightProperty -Location "East US 2"
```

### `Grant-AzHDInsightRdpServicesAccess`
<span data-ttu-id="18b25-157">Foram removidos os cmdlets `Grant-AzHDInsightRdpServicesAccess` e `Revoke-AzHDInsightRdpServicesAccess`.</span><span class="sxs-lookup"><span data-stu-id="18b25-157">Removed the `Grant-AzHDInsightRdpServicesAccess` and `Revoke-AzHDInsightRdpServicesAccess` cmdlets.</span></span> <span data-ttu-id="18b25-158">Deixaram de ser necessários porque os clusters que utilizam o tipo de SO Windows não são suportados.</span><span class="sxs-lookup"><span data-stu-id="18b25-158">These are no longer necessary because clusters using Windows OS type are not supported.</span></span> <span data-ttu-id="18b25-159">Em vez disso, crie um cluster com o tipo de SO Linux.</span><span class="sxs-lookup"><span data-stu-id="18b25-159">Please create a cluster using Linux OS type instead.</span></span>

### `Remove-AzHDInsightCluster`
<span data-ttu-id="18b25-160">O tipo de saída de `Remove-AzHDInsightCluster` foi alterado de `Microsoft.Azure.Management.HDInsight.Models.ClusterGetResponse` para `bool`.</span><span class="sxs-lookup"><span data-stu-id="18b25-160">The output type of `Remove-AzHDInsightCluster` changed from `Microsoft.Azure.Management.HDInsight.Models.ClusterGetResponse` to `bool`.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-161">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-161">Before</span></span>
```powershell
$cluster = Remove-AzHDInsightCluster -ClusterName "your-hadoop-001"
```

#### <a name="after"></a><span data-ttu-id="18b25-162">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-162">After</span></span>
```powershell
Remove-AzHDInsightCluster -ClusterName "your-hadoop-001" -PassThru
True
```

### `Revoke-AzHDInsightRdpServicesAccess`
<span data-ttu-id="18b25-163">O cmdlet foi preterido.</span><span class="sxs-lookup"><span data-stu-id="18b25-163">The cmdlet is deprecated.</span></span> <span data-ttu-id="18b25-164">Não existe substituição para o cmdlet.</span><span class="sxs-lookup"><span data-stu-id="18b25-164">There is no replacement for it.</span></span>

### `Set-AzHDInsightGatewayCredential`
<span data-ttu-id="18b25-165">O tipo de saída de `Set-AzHDInsightGatewayCredential` foi alterado de `HttpConnectivitySettings` para `AzureHDInsightGatewaySettings`.</span><span class="sxs-lookup"><span data-stu-id="18b25-165">The output type of `Set-AzHDInsightGatewayCredential` changed from `HttpConnectivitySettings` to `AzureHDInsightGatewaySettings`.</span></span>



## <a name="iothub"></a><span data-ttu-id="18b25-166">IotHub</span><span class="sxs-lookup"><span data-stu-id="18b25-166">IotHub</span></span>

### `New-AzIotHubImportDevices`
<span data-ttu-id="18b25-167">Este alias foi removido. Em vez disso, utilize `New-AzIotHubImportDevice`.</span><span class="sxs-lookup"><span data-stu-id="18b25-167">This alias is removed, please use `New-AzIotHubImportDevice` instead.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-168">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-168">Before</span></span>
```powershell
New-AzIotHubImportDevices -ResourceGroupName "myresourcegroup" -Name "myiothub" -InputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -OutputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D"
```

#### <a name="after"></a><span data-ttu-id="18b25-169">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-169">After</span></span>
```powershell
New-AzIotHubImportDevice -ResourceGroupName "myresourcegroup" -Name "myiothub" -InputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -OutputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D"
```

### `New-AzIotHubExportDevices`
<span data-ttu-id="18b25-170">Este alias foi removido. Em vez disso, utilize `New-AzIotHubExportDevice`.</span><span class="sxs-lookup"><span data-stu-id="18b25-170">This alias is removed, please use `New-AzIotHubExportDevice` instead.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-171">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-171">Before</span></span>
```powershell
New-AzIotHubExportDevices -ResourceGroupName "myresourcegroup" -Name "myiothub" -ExportBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -ExcludeKeys
```

#### <a name="after"></a><span data-ttu-id="18b25-172">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-172">After</span></span>
```powershell
New-AzIotHubExportDevice -ResourceGroupName "myresourcegroup" -Name "myiothub" -ExportBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -ExcludeKeys
```

### `Add-AzIotHubEventHubConsumerGroup`
<span data-ttu-id="18b25-173">O parâmetro `EventHubEndPointName` foi preterido sem ser substituído, uma vez que o IotHub inclui apenas um ponto final incorporado ("events") que pode processar as mensagens do sistema e do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18b25-173">Parameter `EventHubEndPointName` is deprecated without being replaced as IotHub comes with only one built-in endpoint("events") which could handle system and device messages.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-174">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-174">Before</span></span>
```powershell
Add-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName "myconsumergroup" -EventHubEndpointName "/EventHubEndpointName"
```

#### <a name="after"></a><span data-ttu-id="18b25-175">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-175">After</span></span>
```powershell
Add-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName "myconsumergroup"
```

### `Get-AzIotHubEventHubConsumerGroup`
<span data-ttu-id="18b25-176">O parâmetro `EventHubEndPointName` foi preterido sem ser substituído, uma vez que o IotHub inclui apenas um ponto final incorporado ("events") que pode processar as mensagens do sistema e do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18b25-176">Parameter `EventHubEndPointName` is deprecated without being replaced as IotHub comes with only one built-in endpoint("events") which could handle system and device messages.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-177">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-177">Before</span></span>
```powershell
Get-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubEndpointName "/EventHubEndpointName"
```

#### <a name="after"></a><span data-ttu-id="18b25-178">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-178">After</span></span>
```powershell
Get-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub"
```

### `Remove-AzIotHubEventHubConsumerGroup`
<span data-ttu-id="18b25-179">O parâmetro `EventHubEndPointName` foi preterido sem ser substituído, uma vez que o IotHub inclui apenas um ponto final incorporado ("events") que pode processar as mensagens do sistema e do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18b25-179">Parameter `EventHubEndPointName` is deprecated without being replaced as IotHub comes with only one built-in endpoint("events") which could handle system and device messages.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-180">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-180">Before</span></span>
```powershell
Remove-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName myconsumergroup -EventHubEndpointName "/EventHubEndpointName"
```

#### <a name="after"></a><span data-ttu-id="18b25-181">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-181">After</span></span>
```powershell
Remove-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName myconsumergroup
```

### `Set-AzIotHub`
<span data-ttu-id="18b25-182">O parâmetro `OperationsMonitoringProperties` foi preterido sem ser substituído, uma vez que o IotHub deixou de utilizar um ponto final incorporado ("operationsMonitoringEvents").</span><span class="sxs-lookup"><span data-stu-id="18b25-182">Parameter `OperationsMonitoringProperties` is deprecated without being replaced as IotHub is no longer using built-in endpoint("operationsMonitoringEvents").</span></span>



## <a name="recoveryservices"></a><span data-ttu-id="18b25-183">RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="18b25-183">RecoveryServices</span></span>

### `Edit-AzRecoveryServicesAsrRecoveryPlan`
<span data-ttu-id="18b25-184">`ASRRecoveryPlanGroup.ReplicationProtectedItems`, `ASRRecoveryPlanGroup.StartGroupActions` e `ASRRecoveryPlanGroup.EndGroupActions` foram removidos da saída.</span><span class="sxs-lookup"><span data-stu-id="18b25-184">`ASRRecoveryPlanGroup.ReplicationProtectedItems`, `ASRRecoveryPlanGroup.StartGroupActions` and `ASRRecoveryPlanGroup.EndGroupActions` is removed from output.</span></span>

### `Get-AzRecoveryServicesAsrRecoveryPlan`
<span data-ttu-id="18b25-185">`ASRRecoveryPlanGroup.ReplicationProtectedItems`, `ASRRecoveryPlanGroup.StartGroupActions` e `ASRRecoveryPlanGroup.EndGroupActions` foram removidos da saída.</span><span class="sxs-lookup"><span data-stu-id="18b25-185">`ASRRecoveryPlanGroup.ReplicationProtectedItems`, `ASRRecoveryPlanGroup.StartGroupActions` and `ASRRecoveryPlanGroup.EndGroupActions` is removed from output.</span></span>

### `New-AzRecoveryServicesAsrReplicationProtectedItem`
<span data-ttu-id="18b25-186">O parâmetro IncludeDiskId foi alterado para suportar a escrita direta num disco gerido no Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="18b25-186">Parameter IncludeDiskId is changed to support directly writing to a managed disk in Azure Site Recovery.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-187">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-187">Before</span></span>
```powershell
$job = New-AzRecoveryServicesAsrReplicationProtectedItem -RecoveryAzureStorageAccountId $recoveryAzureStorageAccountId -IncludeDiskId $includeDiskId -VMwareToAzure -Account $fabric.FabricSpecificDetails.RunAsAccounts[0] -RecoveryResourceGroupId $RecoveryResourceGroupId -RecoveryAzureNetworkId $RecoveryAzureNetworkId -name $name -ProcessServer $fabric.FabricSpecificDetails.ProcessServers[0] -ProtectableItem $protectableItem -ProtectionContainerMapping $pcm -RecoveryAzureSubnetName $RecoveryAzureSubnetName -RecoveryVmName $RecoveryVmName -LogStorageAccountId $LogStorageAccountId
```

#### <a name="after"></a><span data-ttu-id="18b25-188">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-188">After</span></span>
```powershell
$disk1 = New-AzRecoveryServicesAsrInMageAzureV2DiskInput -DiskId $diskId -LogStorageAccountId $logStorageAccountId -DiskType $diskType
$disk2 = New-AzRecoveryServicesAsrInMageAzureV2DiskInput -DiskId $diskId2 -LogStorageAccountId $logStorageAccountId -DiskType $diskType2
$job = New-AzRecoveryServicesAsrReplicationProtectedItem -VMwareToAzure -Account $fabric.FabricSpecificDetails.RunAsAccounts[0] -RecoveryResourceGroupId $RecoveryResourceGroupId -RecoveryAzureNetworkId $RecoveryAzureNetworkId -name $name -ProcessServer $fabric.FabricSpecificDetails.ProcessServers[0] -ProtectableItem $protectableItem -ProtectionContainerMapping $pcm -RecoveryAzureSubnetName $RecoveryAzureSubnetName -RecoveryVmName $RecoveryVmName -LogStorageAccountId $LogStorageAccountId -InMageAzureV2DiskInput $disk1,$disk2
```

## <a name="resources"></a><span data-ttu-id="18b25-189">Recursos</span><span class="sxs-lookup"><span data-stu-id="18b25-189">Resources</span></span>

### <a name="previous-version-incompatibility-with-azbatch-module"></a><span data-ttu-id="18b25-190">Incompatibilidade com as versões anteriores do módulo Az.Batch</span><span class="sxs-lookup"><span data-stu-id="18b25-190">Previous Version Incompatibility with Az.Batch Module</span></span>
<span data-ttu-id="18b25-191">A versão 1.7.1 do módulo "Az.Resources" é incompatível com as versões anteriores (versão 1.1.2 ou anterior) do módulo "AZ.Batch".</span><span class="sxs-lookup"><span data-stu-id="18b25-191">Version 1.7.1 of the ‘Az.Resources’ module is incompatible with earlier versions (version 1.1.2 or earlier) of the ‘Az.Batch’ module.</span></span>  <span data-ttu-id="18b25-192">Isto resultará na incapacidade de importar a versão 1.1.2 do módulo "Az.Batch" quando a versão 1.7.1 do módulo "Az.Resources" for importada.</span><span class="sxs-lookup"><span data-stu-id="18b25-192">This will result in being unable to import  version 1.1.2 of the ‘Az.Batch’ module when version 1.7.1 of the ‘Az.Resources’ module is imported.</span></span>  <span data-ttu-id="18b25-193">Para corrigir este problema, atualize o módulo "Az.Batch" para a versão 2.0.1 ou posterior, ou instale simplesmente a versão mais recente do módulo "Az".</span><span class="sxs-lookup"><span data-stu-id="18b25-193">To fix this issue, update the ‘Az.Batch’ module to version 2.0.1 or greater, or simply install the latest version of the ‘Az’ module.</span></span>

## <a name="servicefabric"></a><span data-ttu-id="18b25-194">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="18b25-194">ServiceFabric</span></span>

### `Add-ServiceFabricApplicationCertificate`
<span data-ttu-id="18b25-195">`Add-ServiceFabricApplicationCertificate` foi removido porque este cenário é abrangido por `Add-AzVmssSecret`.</span><span class="sxs-lookup"><span data-stu-id="18b25-195">Removed `Add-ServiceFabricApplicationCertificate` as this scenario is covered by `Add-AzVmssSecret`.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-196">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-196">Before</span></span>
```powershell
Add-AzServiceFabricApplicationCertificate -ResourceGroupName "Group1" -Name "Contoso01SFCluster" -SecretIdentifier "http://keyVaultName.vault.contoso.net/secrets/secretName/secretVersion"
```

#### <a name="after"></a><span data-ttu-id="18b25-197">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-197">After</span></span>
```powershell
$Vault = Get-AzKeyVault -VaultName "ContosoVault"
$CertConfig = New-AzVmssVaultCertificateConfig -CertificateUrl "http://keyVaultName.vault.contoso.net/secrets/secretName/secretVersion" -CertificateStore "Certificates"
$VMSS = New-AzVmssConfig
Add-AzVmssSecret -VirtualMachineScaleSet $VMSS -SourceVaultId $Vault.ResourceId -VaultCertificate $CertConfig
```


## <a name="sql"></a><span data-ttu-id="18b25-198">SQL</span><span class="sxs-lookup"><span data-stu-id="18b25-198">Sql</span></span>

### `Get-AzSqlDatabaseSecureConnectionPolicy`
<span data-ttu-id="18b25-199">Tenha em atenção que a ligação segura foi preterida, pelo que o comando foi removido.</span><span class="sxs-lookup"><span data-stu-id="18b25-199">Note that secure connection is deprecated and so command is removed.</span></span> <span data-ttu-id="18b25-200">Utilize o painel da base de dados SQL no portal do Azure para ver as cadeias de ligação</span><span class="sxs-lookup"><span data-stu-id="18b25-200">Please use the SQL database blade in the Azure portal to view the connection strings</span></span>

### `Get-AzSqlDatabaseIndexRecommendations`
<span data-ttu-id="18b25-201">O alias `Get-AzSqlDatabaseIndexRecommendations` foi removido.</span><span class="sxs-lookup"><span data-stu-id="18b25-201">`Get-AzSqlDatabaseIndexRecommendations` alias is removed.</span></span> <span data-ttu-id="18b25-202">Em vez disso, utilize `Get-AzSqlDatabaseIndexRecommendation`.</span><span class="sxs-lookup"><span data-stu-id="18b25-202">Use `Get-AzSqlDatabaseIndexRecommendation` instead.</span></span>

### `Get-AzSqlDatabaseRestorePoints`
<span data-ttu-id="18b25-203">O alias `Get-AzSqlDatabaseRestorePoints` foi removido.</span><span class="sxs-lookup"><span data-stu-id="18b25-203">`Get-AzSqlDatabaseRestorePoints` alias is removed.</span></span> <span data-ttu-id="18b25-204">Em vez disso, utilize `Get-AzSqlDatabaseRestorePoint`.</span><span class="sxs-lookup"><span data-stu-id="18b25-204">Use `Get-AzSqlDatabaseRestorePoint` instead.</span></span>

### `Get-AzSqlDatabaseAuditing`
- <span data-ttu-id="18b25-205">O cmdlet `Get-AzSqlDatabaseAudit` está a substituir este cmdlet.</span><span class="sxs-lookup"><span data-stu-id="18b25-205">The cmdlet `Get-AzSqlDatabaseAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="18b25-206">O tipo de saída está a ser alterado do tipo existente "Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel" para o novo tipo "Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseAuditingSettingsModel" e estão a ser removidas as propriedades `AuditState` e `StorageAccountName`.</span><span class="sxs-lookup"><span data-stu-id="18b25-206">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseAuditingSettingsModel', removing properties `AuditState` and `StorageAccountName`.</span></span> <span data-ttu-id="18b25-207">e `StorageAccountSubscriptionId`.</span><span class="sxs-lookup"><span data-stu-id="18b25-207">and `StorageAccountSubscriptionId`.</span></span>  <span data-ttu-id="18b25-208">Os scripts podem obter informações da conta de armazenamento a partir da nova propriedade `StorageAccountResourceId`.</span><span class="sxs-lookup"><span data-stu-id="18b25-208">Scripts can retrieve storage account information from the new `StorageAccountResourceId` property.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-209">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-209">Before</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseAuditing -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
DatabaseName                 : database01
AuditAction                  : {}
AuditActionGroup             : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP,
                                BATCH_COMPLETED_GROUP, ...}
ResourceGroupName            : resourcegroup01
ServerName                   : server01
AuditState                   : Enabled
StorageAccountName           : mystorage
StorageKeyType               : Primary
RetentionInDays              : 0
StorageAccountSubscriptionId : 7fe3301d-31d3-4668-af5e-211a890ba6e3
PredicateExpression          : statement <> 'select 1'
```

#### <a name="after"></a><span data-ttu-id="18b25-210">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-210">After</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseAudit -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
ServerName                          : server01
DatabaseName                        : database01
AuditAction                         : {}
ResourceGroupName                   : resourcegroup01
AuditActionGroup                    : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP,
                                       BATCH_COMPLETED_GROUP, ...}
PredicateExpression                 : statement <> 'select 1'
BlobStorageTargetState              : Enabled
StorageAccountResourceId            : /subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage
StorageKeyType                      : Primary
RetentionInDays                     : 0
EventHubTargetState                 : Enabled
EventHubName                        : eventHubName
EventHubAuthorizationRuleResourceId : EventHubAuthorizationRuleResourceId
LogAnalyticsTargetState             : Enabled
WorkspaceResourceId                 : "/subscriptions/4b9e8510-67ab-4e9a-95a9-e2f1e570ea9c/resourceGroups/insights-integration/providers/Microsoft.OperationalInsights/workspaces/viruela2"
```

### `Set-AzSqlDatabaseAuditing`
- <span data-ttu-id="18b25-211">O cmdlet `Set-AzSqlDatabaseAudit` está a substituir este cmdlet.</span><span class="sxs-lookup"><span data-stu-id="18b25-211">The cmdlet `Set-AzSqlDatabaseAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="18b25-212">O tipo de saída está a ser alterado do tipo existente "Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel" para o novo tipo "bool"</span><span class="sxs-lookup"><span data-stu-id="18b25-212">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'bool'</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-213">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-213">Before</span></span>
```powershell
Set-AzSqlDatabaseAuditing -State Enabled -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -StorageAccountName "Storage22" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-214">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-214">After</span></span>
```powershell
Set-AzSqlDatabaseAudit -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01" -BlobStorageTargetState Enabled -StorageAccountResourceId "/subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage"
```

### `Get-AzSqlServerAuditing`
- <span data-ttu-id="18b25-215">O cmdlet `Get-AzSqlServerAudit` está a substituir este cmdlet.</span><span class="sxs-lookup"><span data-stu-id="18b25-215">The cmdlet `Get-AzSqlServerAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="18b25-216">O tipo de saída está a ser alterado do tipo existente "Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel" para o novo tipo "Microsoft.Azure.Commands.Sql.Auditing.Model.ServerAuditingSettingsModel".</span><span class="sxs-lookup"><span data-stu-id="18b25-216">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'Microsoft.Azure.Commands.Sql.Auditing.Model.ServerAuditingSettingsModel'.</span></span>  <span data-ttu-id="18b25-217">As propriedades `AuditState`, `StorageAccountName` e `StorageAccountSubscriptionId` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="18b25-217">Properties `AuditState`, `StorageAccountName`, and `StorageAccountSubscriptionId` are removed.</span></span>  <span data-ttu-id="18b25-218">Os scripts que utilizam as propriedades `StorageAccountName` e `StorageAccountSubscriptionId` podem obter estas informações a partir da nova propriedade `StorageAccountResourceId`.</span><span class="sxs-lookup"><span data-stu-id="18b25-218">Scripts that use `StorageAccountName` and `StorageAccountSubscriptionId` proeprties can retrieve this information from the new `StorageAccountResourceId` property.</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-219">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-219">Before</span></span>
```powershell
PS C:\> Get-AzSqlServerAuditing -ResourceGroupName "resourcegroup01" -ServerName "server01"
AuditActionGroup             : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP, BATCH_COMPLETED_GROUP, ...}
ResourceGroupName            : resourcegroup01
ServerName                   : server01
AuditState                   : Enabled
StorageAccountName           : mystorage
StorageKeyType               : Primary
RetentionInDays              : 0
StorageAccountSubscriptionId : 7fe3301d-31d3-4668-af5e-211a890ba6e3
PredicateExpression          : statement <> 'select 1'
```

#### <a name="after"></a><span data-ttu-id="18b25-220">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-220">After</span></span>
```powershell
PS C:\> Get-AzSqlServerAudit -ResourceGroupName "resourcegroup01" -ServerName "server01"
ServerName                          : server01
ResourceGroupName                   : resourcegroup01
AuditActionGroup                    : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP, BATCH_COMPLETED_GROUP, ...}
PredicateExpression                 : statement <> 'select 1'
BlobStorageTargetState              : Enabled
StorageAccountResourceId            : /subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage
StorageKeyType                      : Primary
RetentionInDays                     : 0
EventHubTargetState                 : Enabled
EventHubName                        : eventHubName
EventHubAuthorizationRuleResourceId : EventHubAuthorizationRuleResourceId
LogAnalyticsTargetState             : Enabled
WorkspaceResourceId                 : "/subscriptions/4b9e8510-67ab-4e9a-95a9-e2f1e570ea9c/resourceGroups/insights-integration/providers/Microsoft.OperationalInsights/workspaces/viruela2"
```

### `Set-AzSqlServerAuditing`
- <span data-ttu-id="18b25-221">O cmdlet `Set-AzSqlServerAudit` está a substituir este cmdlet.</span><span class="sxs-lookup"><span data-stu-id="18b25-221">The cmdlet `Set-AzSqlServerAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="18b25-222">O tipo de saída está a ser alterado do tipo existente "Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel" para o novo tipo "bool"</span><span class="sxs-lookup"><span data-stu-id="18b25-222">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'bool'</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-223">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-223">Before</span></span>
```powershell
Set-AzSqlServerAuditing -State Enabled -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -StorageAccountName "Storage22"
```

#### <a name="after"></a><span data-ttu-id="18b25-224">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-224">After</span></span>
```powershell
PS C:\> Set-AzSqlServerAudit -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -BlobStorageTargetState Enabled -StorageAccountResourceId "/subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage"
```

### `Get-AzSqlServerAdvancedThreatProtectionSettings`
<span data-ttu-id="18b25-225">O cmdlet `Get-AzSqlServerAdvancedThreatProtectionSettings` foi substituído por `Get-AzSqlServerAdvancedThreatProtectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-225">Cmdlet `Get-AzSqlServerAdvancedThreatProtectionSettings` is replaced by `Get-AzSqlServerAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-226">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-226">Before</span></span>
```powershell
Get-AzSqlServerAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

#### <a name="after"></a><span data-ttu-id="18b25-227">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-227">After</span></span>
```powershell
Get-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

### `Clear-AzSqlServerAdvancedThreatProtectionSettings`
<span data-ttu-id="18b25-228">O cmdlet `Clear-AzSqlServerAdvancedThreatProtectionSettings` foi substituído por `Clear-AzSqlServerAdvancedThreatProtectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-228">Cmdlet `Clear-AzSqlServerAdvancedThreatProtectionSettings` is replaced by `Clear-AzSqlServerAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-229">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-229">Before</span></span>
```powershell
Clear-AzSqlServerAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

#### <a name="after"></a><span data-ttu-id="18b25-230">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-230">After</span></span>
```powershell
Clear-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

### `Update-AzSqlServerAdvancedThreatProtectionSettings`
<span data-ttu-id="18b25-231">O cmdlet `Update-AzSqlServerAdvancedThreatProtectionSettings` foi substituído por `Update-AzSqlServerAdvancedThreatProtectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-231">Cmdlet `Update-AzSqlServerAdvancedThreatProtectionSettings` is replaced by `Update-AzSqlServerAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-232">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-232">Before</span></span>
```powershell
Update-AzSqlServerAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="18b25-233">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-233">After</span></span>
```powershell
Update-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Get-AzSqlDatabaseAdvancedThreatProtectionSettings`
<span data-ttu-id="18b25-234">O cmdlet `Get-AzSqlDatabaseAdvancedThreatProtectionSettings` foi substituído por `Get-AzSqlDatabaseAdvancedThreatProtectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-234">Cmdlet `Get-AzSqlDatabaseAdvancedThreatProtectionSettings` is replaced by `Get-AzSqlDatabaseAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-235">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-235">Before</span></span>
```powershell
Get-AzSqlDatabaseAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-236">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-236">After</span></span>
```powershell
Get-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

### `Update-AzSqlDatabaseAdvancedThreatProtectionSettings`
<span data-ttu-id="18b25-237">O cmdlet `Update-AzSqlDatabaseAdvancedThreatProtectionSettings` foi substituído por `Update-AzSqlDatabaseAdvancedThreatProtectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-237">Cmdlet `Update-AzSqlDatabaseAdvancedThreatProtectionSettings` is repleaced by `Update-AzSqlDatabaseAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-238">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-238">Before</span></span>
```powershell
Update-AzSqlDatabaseAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="18b25-239">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-239">After</span></span>
```powershell
Update-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Clear-AzSqlDatabaseAdvancedThreatProtectionSettings`
<span data-ttu-id="18b25-240">O cmdlet `Clear-AzSqlDatabaseAdvancedThreatProtectionSettings` foi substituído por `Clear-AzSqlDatabaseAdvancedThreatProtectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-240">Cmdlet `Clear-AzSqlDatabaseAdvancedThreatProtectionSettings` is repleaced by `Clear-AzSqlDatabaseAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-241">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-241">Before</span></span>
```powershell
Clear-AzSqlDatabaseAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-242">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-242">After</span></span>
```powershell
Clear-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

### `Update-AzSqlDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-243">O cmdlet `Update-AzSqlDatabaseVulnerabilityAssessmentSettings` foi substituído por `Update-AzSqlDatabaseVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-243">Cmdlet `Update-AzSqlDatabaseVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-244">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-244">Before</span></span>
```powershell
Update-AzSqlDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="18b25-245">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-245">After</span></span>
```powershell
Update-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```


### `Get-AzSqlDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-246">O cmdlet `Get-AzSqlDatabaseVulnerabilityAssessmentSettings` foi substituído por `Get-AzSqlDatabaseVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-246">Cmdlet `Get-AzSqlDatabaseVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-247">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-247">Before</span></span>
```powershell
Get-AzSqlDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-248">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-248">After</span></span>
```powershell
Get-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-249">O cmdlet `Clear-AzSqlDatabaseVulnerabilityAssessmentSettings` foi substituído por `Clear-AzSqlDatabaseVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-249">Cmdlet `Clear-AzSqlDatabaseVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-250">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-250">Before</span></span>
```powershell
Clear-AzSqlDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-251">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-251">After</span></span>
```powershell
Clear-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-252">O cmdlet `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` foi substituído por `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-252">Cmdlet `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-253">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-253">Before</span></span>
```powershell
Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="18b25-254">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-254">After</span></span>
```powershell
Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

### `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-255">O cmdlet `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` foi substituído por `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-255">Cmdlet `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-256">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-256">Before</span></span>
```powershell
Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-257">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-257">After</span></span>
```powershell
Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-258">O cmdlet `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` foi substituído por `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-258">Cmdlet `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-259">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-259">Before</span></span>
```powershell
Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-260">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-260">After</span></span>
```powershell
Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Update-AzSqlInstanceVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-261">O cmdlet `Update-AzSqlInstanceVulnerabilityAssessmentSettings` foi substituído por `Update-AzSqlInstanceVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-261">Cmdlet `Update-AzSqlInstanceVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlInstanceVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-262">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-262">Before</span></span>
```powershell
Update-AzSqlInstanceVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="18b25-263">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-263">After</span></span>
```powershell
Update-AzSqlInstanceVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

### `Get-AzSqlInstanceVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-264">O cmdlet `Get-AzSqlInstanceVulnerabilityAssessmentSettings` foi substituído por `Get-AzSqlInstanceVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-264">Cmdlet `Get-AzSqlInstanceVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlInstanceVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-265">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-265">Before</span></span>
```powershell
Get-AzSqlInstanceVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-266">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-266">After</span></span>
```powershell
Get-AzSqlInstanceVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlInstanceVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-267">O cmdlet `Clear-AzSqlInstanceVulnerabilityAssessmentSettings` foi substituído por `Clear-AzSqlInstanceVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-267">Cmdlet `Clear-AzSqlInstanceVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlInstanceVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-268">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-268">Before</span></span>
```powershell
Clear-AzSqlInstanceVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-269">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-269">After</span></span>
```powershell
Clear-AzSqlInstanceVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Update-AzSqlServerVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-270">O cmdlet `Update-AzSqlServerVulnerabilityAssessmentSettings` foi substituído por `Update-AzSqlServerVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-270">Cmdlet `Update-AzSqlServerVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlServerVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-271">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-271">Before</span></span>
```powershell
Update-AzSqlServerVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="18b25-272">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-272">After</span></span>
```powershell
Update-AzSqlServerVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

### `Get-AzSqlServerVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-273">O cmdlet `Get-AzSqlServerVulnerabilityAssessmentSettings` foi substituído por `Get-AzSqlServerVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-273">Cmdlet `Get-AzSqlServerVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlServerVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-274">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-274">Before</span></span>
```powershell
Get-AzSqlServerVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-275">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-275">After</span></span>
```powershell
Get-AzSqlServerVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlServerVulnerabilityAssessmentSettings`
<span data-ttu-id="18b25-276">O cmdlet `Clear-AzSqlServerVulnerabilityAssessmentSettings` foi substituído por `Clear-AzSqlServerVulnerabilityAssessmentSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-276">Cmdlet `Clear-AzSqlServerVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlServerVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-277">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-277">Before</span></span>
```powershell
Clear-AzSqlServerVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-278">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-278">After</span></span>
```powershell
Clear-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Get-AzSqlServerAdvancedThreatProtectionPolicy`
<span data-ttu-id="18b25-279">O cmdlet `Get-AzSqlServerAdvancedThreatProtectionPolicy` foi eliminado e não foi substituído por nenhum cmdlet</span><span class="sxs-lookup"><span data-stu-id="18b25-279">Cmdlet `Get-AzSqlServerAdvancedThreatProtectionPolicy` is deleted and no cmdlet is repleaced it</span></span>

### `Get-AzSqlServerThreatDetectionPolicy`
<span data-ttu-id="18b25-280">O cmdlet `Get-AzSqlServerThreatDetectionPolicy` foi substituído por `Get-AzSqlServerThreatDetectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-280">Cmdlet `Get-AzSqlServerThreatDetectionPolicy` is repleaced by `Get-AzSqlServerThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-281">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-281">Before</span></span>
```powershell
PS C:\> Get-AzSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

#### <a name="after"></a><span data-ttu-id="18b25-282">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-282">After</span></span>
```powershell
PS C:\> Get-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

### `Remove-AzSqlServerThreatDetectionPolicy`
<span data-ttu-id="18b25-283">O cmdlet `Remove-AzSqlServerThreatDetectionPolicy` foi substituído por `Clear-AzSqlServerThreatDetectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-283">Cmdlet `Remove-AzSqlServerThreatDetectionPolicy` is repleaced by `Clear-AzSqlServerThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-284">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-284">Before</span></span>
```powershell
Remove-AzSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

#### <a name="after"></a><span data-ttu-id="18b25-285">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-285">After</span></span>
```powershell
Clear-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

### `Set-AzSqlServerThreatDetectionPolicy`
<span data-ttu-id="18b25-286">O cmdlet `Set-AzSqlServerThreatDetectionPolicy` foi substituído por `Update-AzSqlServerThreatDetectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-286">Cmdlet `Set-AzSqlServerThreatDetectionPolicy` is repleaced by `Update-AzSqlServerThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-287">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-287">Before</span></span>
```powershell
Set-AzSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="18b25-288">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-288">After</span></span>
```powershell
Update-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Get-AzSqlDatabaseThreatDetectionPolicy`
<span data-ttu-id="18b25-289">O cmdlet `Get-AzSqlDatabaseThreatDetectionPolicy` foi substituído por `Get-AzSqlDatabaseThreatDetectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-289">Cmdlet `Get-AzSqlDatabaseThreatDetectionPolicy` is repleaced by `Get-AzSqlDatabaseThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-290">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-290">Before</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName   "Database01"
DatabaseName                 : Database01
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

#### <a name="after"></a><span data-ttu-id="18b25-291">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-291">After</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"   -DatabaseName "Database01"
DatabaseName                 : Database01
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

### `Set-AzSqlDatabaseThreatDetectionPolicy`
<span data-ttu-id="18b25-292">O cmdlet `Set-AzSqlDatabaseThreatDetectionPolicy` foi substituído por `Update-AzSqlDatabaseThreatDetectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-292">Cmdlet `Set-AzSqlDatabaseThreatDetectionPolicy` is repleaced by `Update-AzSqlDatabaseThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-293">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-293">Before</span></span>
```powershell
Set-AzSqlDatabaseThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="18b25-294">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-294">After</span></span>
```powershell
Update-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Remove-AzSqlDatabaseThreatDetectionPolicy`
<span data-ttu-id="18b25-295">O cmdlet `Remove-AzSqlDatabaseThreatDetectionPolicy` foi substituído por `Clear-AzSqlDatabaseThreatDetectionSetting`</span><span class="sxs-lookup"><span data-stu-id="18b25-295">Cmdlet `Remove-AzSqlDatabaseThreatDetectionPolicy` is repleaced by `Clear-AzSqlDatabaseThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="18b25-296">Antes</span><span class="sxs-lookup"><span data-stu-id="18b25-296">Before</span></span>
```powershell
Remove-AzSqlDatabaseThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="18b25-297">Depois</span><span class="sxs-lookup"><span data-stu-id="18b25-297">After</span></span>
```powershell
Clear-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```