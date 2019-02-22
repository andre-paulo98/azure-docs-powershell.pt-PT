---
title: Alterações recentes ao Microsoft Azure PowerShell 6.0.0
description: Este guia de migração contém uma lista de alterações recentes realizadas no Azure PowerShell no lançamento da versão 6.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: 39d9fa6e354c3c3448053c9cdc98fdc7f55b068d
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153551"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-600"></a><span data-ttu-id="d49db-103">Alterações recentes ao Microsoft Azure PowerShell 6.0.0</span><span class="sxs-lookup"><span data-stu-id="d49db-103">Breaking changes for Microsoft Azure PowerShell 6.0.0</span></span>

<span data-ttu-id="d49db-104">Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d49db-104">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="d49db-105">Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço.</span><span class="sxs-lookup"><span data-stu-id="d49db-105">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="d49db-106">Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.</span><span class="sxs-lookup"><span data-stu-id="d49db-106">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="d49db-107">Índice</span><span class="sxs-lookup"><span data-stu-id="d49db-107">Table of Contents</span></span>

- [<span data-ttu-id="d49db-108">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="d49db-108">General breaking changes</span></span>](#general-breaking-changes)
    - [<span data-ttu-id="d49db-109">Versão mínima do PowerShell necessária bumped para 5.0</span><span class="sxs-lookup"><span data-stu-id="d49db-109">Minimum PowerShell version required bumped to 5.0</span></span>](#minimum-powershell-version-required-bumped-to-50)
    - [<span data-ttu-id="d49db-110">Gravação automática do contexto ativada por predefinição</span><span class="sxs-lookup"><span data-stu-id="d49db-110">Context autosaved enabled by default</span></span>](#context-autosave-enabled-by-default)
    - [<span data-ttu-id="d49db-111">Remoção de alias de Etiquetas</span><span class="sxs-lookup"><span data-stu-id="d49db-111">Removal of Tags alias</span></span>](#removal-of-tags-alias)
- [<span data-ttu-id="d49db-112">Alterações interruptivas aos cmdlets AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d49db-112">Breaking changes to AzureRM.Compute cmdlets</span></span>](#breaking-changes-to-azurermcompute-cmdlets)
- [<span data-ttu-id="d49db-113">Alterações interruptivas aos cmdlets AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d49db-113">Breaking changes to AzureRM.DataLakeStore cmdlets</span></span>](#breaking-changes-to-azurermdatalakestore-cmdlets)
- [<span data-ttu-id="d49db-114">Alterações interruptivas aos cmdlets AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="d49db-114">Breaking changes to AzureRM.Dns cmdlets</span></span>](#breaking-changes-to-azurermdns-cmdlets)
- [<span data-ttu-id="d49db-115">Alterações interruptivas aos cmdlets AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d49db-115">Breaking changes to AzureRM.Insights cmdlets</span></span>](#breaking-changes-to-azurerminsights-cmdlets)
- [<span data-ttu-id="d49db-116">Alterações interruptivas aos cmdlets AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d49db-116">Breaking changes to AzureRM.KeyVault cmdlets</span></span>](#breaking-changes-to-azurermkeyvault-cmdlets)
- [<span data-ttu-id="d49db-117">Alterações interruptivas aos cmdlets AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d49db-117">Breaking changes to AzureRM.Network cmdlets</span></span>](#breaking-changes-to-azurermnetwork-cmdlets)
- [<span data-ttu-id="d49db-118">Alterações interruptivas aos cmdlets AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d49db-118">Breaking changes to AzureRM.RedisCache cmdlets</span></span>](#breaking-changes-to-azurermrediscache-cmdlets)
- [<span data-ttu-id="d49db-119">Alterações interruptivas aos cmdlets AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d49db-119">Breaking changes to AzureRM.Resources cmdlets</span></span>](#breaking-changes-to-azurermresources-cmdlets)
- [<span data-ttu-id="d49db-120">Alterações interruptivas aos cmdlets AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d49db-120">Breaking changes to AzureRM.Storage cmdlets</span></span>](#breaking-changes-to-azurermstorage-cmdlets)
- [<span data-ttu-id="d49db-121">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-121">Removed modules</span></span>](#removed-modules)
    - [`AzureRM.ServerManagement`](#azurermservermanagement)
    - [`AzureRM.SiteRecovery`](#azurermsiterecovery)

## <a name="general-breaking-changes"></a><span data-ttu-id="d49db-122">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="d49db-122">General breaking changes</span></span>

### <a name="minimum-powershell-version-required-bumped-to-50"></a><span data-ttu-id="d49db-123">Versão mínima do PowerShell necessária bumped para 5.0</span><span class="sxs-lookup"><span data-stu-id="d49db-123">Minimum PowerShell version required bumped to 5.0</span></span>

<span data-ttu-id="d49db-124">Anteriormente, o Azure PowerShell precisava de, _pelo menos_, a versão 3.0 do PowerShell para executar qualquer cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d49db-124">Previously, Azure PowerShell required _at least_ version 3.0 of PowerShell to run any cmdlet.</span></span> <span data-ttu-id="d49db-125">Daqui para a frente, este requisito será acionado para a versão 5.0 do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d49db-125">Moving forward, this requirement will be raised to version 5.0 of PowerShell.</span></span> <span data-ttu-id="d49db-126">Para obter informações sobre a atualização para o PowerShell 5.0, veja [esta tabela](https://docs.microsoft.com/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="d49db-126">For information on upgrading to PowerShell 5.0, please see [this table](https://docs.microsoft.com/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

### <a name="context-autosave-enabled-by-default"></a><span data-ttu-id="d49db-127">Gravação automática do contexto ativada por predefinição</span><span class="sxs-lookup"><span data-stu-id="d49db-127">Context autosave enabled by default</span></span>

<span data-ttu-id="d49db-128">A gravação automática do contexto é o armazenamento de informações de início de sessão do Azure, que podem ser utilizadas entre sessões do PowerShell novas e diferentes.</span><span class="sxs-lookup"><span data-stu-id="d49db-128">Context autosave is the storage of Azure sign in information that can be used between new and different PowerShell sessions.</span></span> <span data-ttu-id="d49db-129">Para obter mais informações sobre a gravação automática do contexto, veja [este documento](https://docs.microsoft.com/powershell/azure/context-persistence).</span><span class="sxs-lookup"><span data-stu-id="d49db-129">For more information on context autosave, please see [this document](https://docs.microsoft.com/powershell/azure/context-persistence).</span></span>

<span data-ttu-id="d49db-130">Anteriormente, a gravação automática do contexto estava desativada por predefinição, o que significa que as informações de autenticação do Azure do utilizador não eram armazenadas entre sessões até executarem o cmdlet `Enable-AzureRmContextAutosave` para ativar a persistência de contexto.</span><span class="sxs-lookup"><span data-stu-id="d49db-130">Previously by default, context autosave was disabled, which meant the user's Azure authentication information was not stored between sessions until they ran the `Enable-AzureRmContextAutosave` cmdlet to turn on context persistence.</span></span> <span data-ttu-id="d49db-131">Daqui para a frente, a gravação automática do contexto estará ativada por predefinição, o que significa que os utilizadores _sem definições guardadas da gravação automática do contexto_ terão os respetivos contextos armazenados quando iniciarem sessão pela próxima vez.</span><span class="sxs-lookup"><span data-stu-id="d49db-131">Moving forward, context autosave will be enabled by default, which means that users _with no saved context autosave settings_ will have their context stored the next time they sign in.</span></span> <span data-ttu-id="d49db-132">Os utilizadores podem optar ativamente por não participar desta funcionalidade através do cmdlet `Disable-AzureRmContextAutosave`.</span><span class="sxs-lookup"><span data-stu-id="d49db-132">Users can opt out of this functionality by using the `Disable-AzureRmContextAutosave` cmdlet.</span></span>

<span data-ttu-id="d49db-133">_Nota_: os utilizadores que anteriormente desativaram a gravação automática do contexto ou os utilizadores com gravação automática do contexto ativado e contextos existentes não serão afetados por esta alteração</span><span class="sxs-lookup"><span data-stu-id="d49db-133">_Note_: users that previously disabled context autosave or users with context autosave enabled and existing contexts will not be affected by this change</span></span>

### <a name="removal-of-tags-alias"></a><span data-ttu-id="d49db-134">Remoção de alias de Etiquetas</span><span class="sxs-lookup"><span data-stu-id="d49db-134">Removal of Tags alias</span></span>

<span data-ttu-id="d49db-135">O alias `Tags` para o parâmetro `Tag` foi removido entre vários cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d49db-135">The alias `Tags` for the `Tag` parameter has been removed across numerous cmdlets.</span></span> <span data-ttu-id="d49db-136">Segue-se uma lista de módulos (e os cmdlets correspondentes) afetados por este problema:</span><span class="sxs-lookup"><span data-stu-id="d49db-136">Below is a list of modules (and the corresponding cmdlets) affected by this:</span></span>

#### `AzureRM.ApiManagement`

- `New-AzureRmApiManagement`
- `New-AzureRmApiManagementProperty`
- `Set-AzureRmApiManagementProperty`

#### `AzureRM.Automation`
- `Set-AzureRmAutomationRunbook`

#### `AzureRM.Cdn`
- `New-AzureRmCdnEndpoint`
- `New-AzureRmCdnProfile`

#### `AzureRM.Compute`
- `New-AzureRmVM`
- `Update-AzureRmVM`

#### `AzureRM.DataFactories`
- `New-AzureRmDataFactories`

#### `AzureRM.DataLakeAnalytics`
- `New-AzureRmDataLakeAnalyticsAccount`

#### `AzureRM.DataLakeStore`
- `New-AzureRmDataLakeStoreAccount`
- `Set-AzureRmDataLakeStoreAccount`

#### `AzureRM.MachineLearning`
- `Update-AzureRmMlCommitmentPlan`

#### `AzureRM.Media`
- `Set-AzureRmMediaService`

#### `AzureRM.OperationalInsights`
- `New-AzureRmOperationalInsightsSavedSearch`
- `New-AzureRmOperationalInsightsWorkspace`
- `Set-AzureRmOperationalInsightsSavedSearch`
- `Set-AzureRmOperationalInsightsWorkspace`

## <a name="breaking-changes-to-azurermcompute-cmdlets"></a><span data-ttu-id="d49db-137">Alterações interruptivas aos cmdlets AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d49db-137">Breaking changes to AzureRM.Compute cmdlets</span></span>

<span data-ttu-id="d49db-138">**Diversos**</span><span class="sxs-lookup"><span data-stu-id="d49db-138">**Miscellaneous**</span></span>
- <span data-ttu-id="d49db-139">A propriedade de nome de sku aninhada nos tipos `PSDisk` e `PSSnapshot` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-139">The sku name property nested in types `PSDisk` and `PSSnapshot` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

```powershell-interactive
$disk = Get-AzureRmDisk -ResourceGroupName "MyResourceGroup" -DiskName "MyDiskName"
$disk.Sku.Name       # This will now return Standard_LRS or Premium_LRS

$snapshot = Get-AzureRmSnapshot -ResourceGroupName "MyResourceGroup" -SnapshotName "MySnapshotName"
$snapshot.Sku.Name   # This will now return Standard_LRS or Premium_LRS
```

- <span data-ttu-id="d49db-140">A propriedade do tipo de conta de armazenamento aninhada nos tipos `PSVirtualMachine``PSVirtualMachineScaleSet` e `PSImage` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-140">The storage account type property nested in types `PSVirtualMachine`, `PSVirtualMachineScaleSet` and `PSImage` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

```powershell-interactive
$vm = Get-AzureRmVM -ResourceGroupName "MyResourceGroup" -Name "MyVM"
$vm.StorageProfile.DataDisks[0].ManagedDisk.StorageAccountType   # This will now return Standard_LRS or Premium_LRS
```

<span data-ttu-id="d49db-141">**Add-AzureRmImageDataDisk**</span><span class="sxs-lookup"><span data-stu-id="d49db-141">**Add-AzureRmImageDataDisk**</span></span>
- <span data-ttu-id="d49db-142">Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-142">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-143">**Add-AzureRmVMDataDisk**</span><span class="sxs-lookup"><span data-stu-id="d49db-143">**Add-AzureRmVMDataDisk**</span></span>
- <span data-ttu-id="d49db-144">Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-144">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-145">**Add-AzureRmVmssDataDisk**</span><span class="sxs-lookup"><span data-stu-id="d49db-145">**Add-AzureRmVmssDataDisk**</span></span>
- <span data-ttu-id="d49db-146">Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-146">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-147">**New-AzureRmAvailabilitySet**</span><span class="sxs-lookup"><span data-stu-id="d49db-147">**New-AzureRmAvailabilitySet**</span></span>
- <span data-ttu-id="d49db-148">O parâmetro `Managed` foi removido em favor de `Sku`</span><span class="sxs-lookup"><span data-stu-id="d49db-148">The parameter `Managed` was removed in favor of `Sku`</span></span>

```powershell-interactive
# Old
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Managed

# New
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Sku "Aligned"
```

<span data-ttu-id="d49db-149">**New-AzureRmDiskConfig**</span><span class="sxs-lookup"><span data-stu-id="d49db-149">**New-AzureRmDiskConfig**</span></span>
- <span data-ttu-id="d49db-150">Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-150">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-151">**New-AzureRmDiskUpdateConfig**</span><span class="sxs-lookup"><span data-stu-id="d49db-151">**New-AzureRmDiskUpdateConfig**</span></span>
- <span data-ttu-id="d49db-152">Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-152">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-153">**New-AzureRmSnapshotConfig**</span><span class="sxs-lookup"><span data-stu-id="d49db-153">**New-AzureRmSnapshotConfig**</span></span>
- <span data-ttu-id="d49db-154">Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-154">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-155">**New-AzureRmSnapshotUpdateConfig**</span><span class="sxs-lookup"><span data-stu-id="d49db-155">**New-AzureRmSnapshotUpdateConfig**</span></span>
- <span data-ttu-id="d49db-156">Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-156">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-157">**Set-AzureRmImageOsDisk**</span><span class="sxs-lookup"><span data-stu-id="d49db-157">**Set-AzureRmImageOsDisk**</span></span>
- <span data-ttu-id="d49db-158">Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-158">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-159">**Set-AzureRmVMAEMExtension**</span><span class="sxs-lookup"><span data-stu-id="d49db-159">**Set-AzureRmVMAEMExtension**</span></span>
- <span data-ttu-id="d49db-160">O parâmetro `DisableWAD` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-160">The parameter `DisableWAD` was removed</span></span>
    -  <span data-ttu-id="d49db-161">O Diagnóstico do Azure do Windows está desativado por predefinição</span><span class="sxs-lookup"><span data-stu-id="d49db-161">Windows Azure Diagnostics is disabled by default</span></span>

<span data-ttu-id="d49db-162">**Set-AzureRmVMDataDisk**</span><span class="sxs-lookup"><span data-stu-id="d49db-162">**Set-AzureRmVMDataDisk**</span></span>
- <span data-ttu-id="d49db-163">Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-163">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-164">**Set-AzureRmVMOSDisk**</span><span class="sxs-lookup"><span data-stu-id="d49db-164">**Set-AzureRmVMOSDisk**</span></span>
- <span data-ttu-id="d49db-165">Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-165">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-166">**Set-AzureRmVmssStorageProfile**</span><span class="sxs-lookup"><span data-stu-id="d49db-166">**Set-AzureRmVmssStorageProfile**</span></span>
- <span data-ttu-id="d49db-167">Os valores aceites para o parâmetro `ManagedDisk` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-167">The accepted values for parameter `ManagedDisk` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="d49db-168">**Update-AzureRmVmss**</span><span class="sxs-lookup"><span data-stu-id="d49db-168">**Update-AzureRmVmss**</span></span>
- <span data-ttu-id="d49db-169">Os valores aceites para o parâmetro `ManagedDiskStorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente</span><span class="sxs-lookup"><span data-stu-id="d49db-169">The accepted values for parameter `ManagedDiskStorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

## <a name="breaking-changes-to-azurermdatalakestore-cmdlets"></a><span data-ttu-id="d49db-170">Alterações interruptivas aos cmdlets AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d49db-170">Breaking changes to AzureRM.DataLakeStore cmdlets</span></span>

<span data-ttu-id="d49db-171">**Export-AzureRmDataLakeStoreItem**</span><span class="sxs-lookup"><span data-stu-id="d49db-171">**Export-AzureRmDataLakeStoreItem**</span></span>
- <span data-ttu-id="d49db-172">Os parâmetros `PerFileThreadCount` e `ConcurrentFileCount` foram removidos.</span><span class="sxs-lookup"><span data-stu-id="d49db-172">Parameters `PerFileThreadCount` and `ConcurrentFileCount` were removed.</span></span> <span data-ttu-id="d49db-173">Utilize o parâmetro `Concurrency` daqui para a frente</span><span class="sxs-lookup"><span data-stu-id="d49db-173">Please use the `Concurrency` parameter moving forward</span></span>

```powershell-interactive
# Old
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -Concurrency 160
```

<span data-ttu-id="d49db-174">**Import-AzureRmDataLakeStoreItem**</span><span class="sxs-lookup"><span data-stu-id="d49db-174">**Import-AzureRmDataLakeStoreItem**</span></span>
- <span data-ttu-id="d49db-175">Os parâmetros `PerFileThreadCount` e `ConcurrentFileCount` foram removidos.</span><span class="sxs-lookup"><span data-stu-id="d49db-175">Parameters `PerFileThreadCount` and `ConcurrentFileCount` were removed.</span></span> <span data-ttu-id="d49db-176">Utilize o parâmetro `Concurrency` daqui para a frente</span><span class="sxs-lookup"><span data-stu-id="d49db-176">Please use the `Concurrency` parameter moving forward</span></span>

```powershell-interactive
# Old
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -Concurrency 160
```

<span data-ttu-id="d49db-177">**Remove-AzureRmDataLakeStoreItem**</span><span class="sxs-lookup"><span data-stu-id="d49db-177">**Remove-AzureRmDataLakeStoreItem**</span></span>
- <span data-ttu-id="d49db-178">O parâmetro `Clean` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-178">Parameter `Clean` was removed</span></span>

```powershell-interactive
# Old
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse -Clean

# New
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse
```

## <a name="breaking-changes-to-azurermdns-cmdlets"></a><span data-ttu-id="d49db-179">Alterações interruptivas aos cmdlets AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="d49db-179">Breaking changes to AzureRM.Dns cmdlets</span></span>

<span data-ttu-id="d49db-180">**New-AzureRmDnsRecordSet**</span><span class="sxs-lookup"><span data-stu-id="d49db-180">**New-AzureRmDnsRecordSet**</span></span>
- <span data-ttu-id="d49db-181">O parâmetro `Force` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-181">The parameter `Force` was removed</span></span>

<span data-ttu-id="d49db-182">**Remove-AzureRmDnsRecordSet**</span><span class="sxs-lookup"><span data-stu-id="d49db-182">**Remove-AzureRmDnsRecordSet**</span></span>
- <span data-ttu-id="d49db-183">O parâmetro `Force` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-183">The parameter `Force` was removed</span></span>

<span data-ttu-id="d49db-184">**Remove-AzureRmDnsZone**</span><span class="sxs-lookup"><span data-stu-id="d49db-184">**Remove-AzureRmDnsZone**</span></span>
- <span data-ttu-id="d49db-185">O parâmetro `Force` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-185">The parameter `Force` was removed</span></span>

## <a name="breaking-changes-to-azurerminsights-cmdlets"></a><span data-ttu-id="d49db-186">Alterações interruptivas aos cmdlets AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d49db-186">Breaking changes to AzureRM.Insights cmdlets</span></span>

<span data-ttu-id="d49db-187">**Add-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="d49db-187">**Add-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="d49db-188">Os aliases de parâmetro `AutoscaleProfiles` e `Notifications` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-188">The parameter aliases `AutoscaleProfiles` and `Notifications` were removed</span></span>

<span data-ttu-id="d49db-189">**Add-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="d49db-189">**Add-AzureRmLogProfile**</span></span>
- <span data-ttu-id="d49db-190">Os aliases de parâmetro `Categories` e `Locations` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-190">The parameter aliases `Categories` and `Locations` were removed</span></span>

<span data-ttu-id="d49db-191">**Add-AzureRmMetricAlertRule**</span><span class="sxs-lookup"><span data-stu-id="d49db-191">**Add-AzureRmMetricAlertRule**</span></span>
- <span data-ttu-id="d49db-192">Os aliases de parâmetro `Actions` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-192">The parameter alias `Actions` was removed</span></span>

<span data-ttu-id="d49db-193">**Add-AzureRmWebtestAlertRule**</span><span class="sxs-lookup"><span data-stu-id="d49db-193">**Add-AzureRmWebtestAlertRule**</span></span>
- <span data-ttu-id="d49db-194">Os aliases de parâmetro `Actions` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-194">The parameter alias `Actions` was removed</span></span>

<span data-ttu-id="d49db-195">**Get-AzureRmLog**</span><span class="sxs-lookup"><span data-stu-id="d49db-195">**Get-AzureRmLog**</span></span>
- <span data-ttu-id="d49db-196">Os aliases de parâmetro `MaxRecords` e `MaxEvents` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-196">The parameter aliases `MaxRecords` and `MaxEvents` were removed</span></span>

<span data-ttu-id="d49db-197">**Get-AzureRmMetricDefinition**</span><span class="sxs-lookup"><span data-stu-id="d49db-197">**Get-AzureRmMetricDefinition**</span></span>
- <span data-ttu-id="d49db-198">Os aliases de parâmetro `MetricNames` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-198">The parameter alias `MetricNames` was removed</span></span>

<span data-ttu-id="d49db-199">**New-AzureRmAlertRuleEmail**</span><span class="sxs-lookup"><span data-stu-id="d49db-199">**New-AzureRmAlertRuleEmail**</span></span>
- <span data-ttu-id="d49db-200">Os aliases de parâmetro `CustomEmails` e `SendToServiceOwners` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-200">The parameter aliases `CustomEmails` and `SendToServiceOwners` were removed</span></span>

<span data-ttu-id="d49db-201">**New-AzureRmAlertRuleWebhook**</span><span class="sxs-lookup"><span data-stu-id="d49db-201">**New-AzureRmAlertRuleWebhook**</span></span>
- <span data-ttu-id="d49db-202">Os aliases de parâmetro `Properties` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-202">The parameter alias `Properties` was removed</span></span>

<span data-ttu-id="d49db-203">**New-AzureRmAutoscaleNotification**</span><span class="sxs-lookup"><span data-stu-id="d49db-203">**New-AzureRmAutoscaleNotification**</span></span>
- <span data-ttu-id="d49db-204">Os aliases de parâmetro `CustomEmails`, `SendEmailToSubscriptionCoAdministrators` e `Webhooks` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-204">The parameter aliases `CustomEmails`, `SendEmailToSubscriptionCoAdministrators` and `Webhooks` were removed</span></span>

<span data-ttu-id="d49db-205">**New-AzureRmAutoscaleProfile**</span><span class="sxs-lookup"><span data-stu-id="d49db-205">**New-AzureRmAutoscaleProfile**</span></span>
- <span data-ttu-id="d49db-206">Os aliases de parâmetro `Rules`, `ScheduleDays` , `ScheduleHours` e `ScheduleMinutes`foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-206">The parameter aliases `Rules`, `ScheduleDays`, `ScheduleHours` and `ScheduleMinutes` were removed</span></span>

<span data-ttu-id="d49db-207">**New-AzureRmAutoscaleWebhook**</span><span class="sxs-lookup"><span data-stu-id="d49db-207">**New-AzureRmAutoscaleWebhook**</span></span>
- <span data-ttu-id="d49db-208">Os aliases de parâmetro `Properties` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-208">The parameter alias `Properties` was removed</span></span>

## <a name="breaking-changes-to-azurermkeyvault-cmdlets"></a><span data-ttu-id="d49db-209">Alterações interruptivas aos cmdlets AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d49db-209">Breaking changes to AzureRM.KeyVault cmdlets</span></span>

<span data-ttu-id="d49db-210">**Add-AzureKeyVaultCertificate**</span><span class="sxs-lookup"><span data-stu-id="d49db-210">**Add-AzureKeyVaultCertificate**</span></span>
- <span data-ttu-id="d49db-211">O parâmetro `CertificatePolicy` tornou-se obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d49db-211">The `CertificatePolicy` parameter has become mandatory.</span></span>

<span data-ttu-id="d49db-212">**Set-AzureKeyVaultManagedStorageSasDefinition**</span><span class="sxs-lookup"><span data-stu-id="d49db-212">**Set-AzureKeyVaultManagedStorageSasDefinition**</span></span>
- <span data-ttu-id="d49db-213">O cmdlet já não aceita parâmetros individuais que compõem o token de acesso; em vez disso, o cmdlet substitui parâmetros de token explícitos, como `Service` ou `Permissions`, com um parâmetro `TemplateUri` genérico correspondente a um token de acesso de exemplo definido noutro local (possivelmente através de cmdlets do PowerShell de Armazenamento ou composto manualmente de acordo com a documentação de Armazenamento.) O cmdlet mantém o parâmetro `ValidityPeriod`.</span><span class="sxs-lookup"><span data-stu-id="d49db-213">The cmdlet no longer accepts individual parameters that compose the access token; instead, the cmdlet replaces explicit token parameters, such as `Service` or `Permissions`, with a generic `TemplateUri` parameter, corresponding to a sample access token defined elsewhere (presumably using Storage PowerShell cmdlets, or composed manually according to the Storage documentation.) The cmdlet retains the `ValidityPeriod` parameter.</span></span>

<span data-ttu-id="d49db-214">Para obter mais informações sobre a composição de tokens de acesso partilhado para o Armazenamento do Azure, veja as páginas de documentação, respetivamente:</span><span class="sxs-lookup"><span data-stu-id="d49db-214">For more information on composing shared access tokens for Azure Storage, please refer to the documentation pages, respectively:</span></span>
- [<span data-ttu-id="d49db-215">Construir um Serviço SAS</span><span class="sxs-lookup"><span data-stu-id="d49db-215">Constructing a Service SAS</span></span>](https://docs.microsoft.com/rest/api/storageservices/Constructing-a-Service-SAS)
- [<span data-ttu-id="d49db-216">Construir uma Conta SAS</span><span class="sxs-lookup"><span data-stu-id="d49db-216">Constructing an Account SAS</span></span>](https://docs.microsoft.com/rest/api/storageservices/constructing-an-account-sas)

```powershell-interactive
# Old
$sas = Set-AzureKeyVaultManagedStorageSasDefinition -VaultName myVault -Name myKey -Service Blob -Permissions 'rcw' -ValidityPeriod 180d

# New
$sctx=New-AzureStorageContext -StorageAccountName $sa.StorageAccountName -Protocol Https -StorageAccountKey Key1
$start=[System.DateTime]::Now.AddDays(-1)
$end=[System.DateTime]::Now.AddMonths(1)
$at=New-AzureStorageAccountSasToken -Service blob -ResourceType Service,Container,Object -Permission "racwdlup" -Protocol HttpsOnly -StartTime $start -ExpiryTime $end -Context $sctx
$sas=Set-AzureKeyVaultManagedStorageSasDefinition -AccountName $sa.StorageAccountName -VaultName $kv.VaultName -Name accountsas -TemplateUri $at -SasType 'account' -ValidityPeriod ([System.Timespan]::FromDays(30))
```

<span data-ttu-id="d49db-217">**Set-AzureKeyVaultCertificateIssuer**</span><span class="sxs-lookup"><span data-stu-id="d49db-217">**Set-AzureKeyVaultCertificateIssuer**</span></span>
- <span data-ttu-id="d49db-218">O parâmetro `IssuerProvider` tornou-se obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d49db-218">The `IssuerProvider` parameter has become mandatory.</span></span>

<span data-ttu-id="d49db-219">**Undo-AzureKeyVaultCertificateRemoval**</span><span class="sxs-lookup"><span data-stu-id="d49db-219">**Undo-AzureKeyVaultCertificateRemoval**</span></span>
- <span data-ttu-id="d49db-220">O resultado deste cmdlet foi alterado de `CertificateBundle` para `PSKeyVaultCertificate`.</span><span class="sxs-lookup"><span data-stu-id="d49db-220">The output of this cmdlet has changed from `CertificateBundle` to `PSKeyVaultCertificate`.</span></span>

<span data-ttu-id="d49db-221">**Undo-AzureRmKeyVaultRemoval**</span><span class="sxs-lookup"><span data-stu-id="d49db-221">**Undo-AzureRmKeyVaultRemoval**</span></span>
- <span data-ttu-id="d49db-222">`ResourceGroupName` foi removido do conjunto de parâmetros `InputObject` e, em vez disso, é obtido a partir da propriedade `InputObject` do parâmetro `ResourceId`.</span><span class="sxs-lookup"><span data-stu-id="d49db-222">`ResourceGroupName` has been removed from the `InputObject` parameter set, and is instead obtained from the `InputObject` parameter's `ResourceId` property.</span></span>

<span data-ttu-id="d49db-223">**Set-AzureRmKeyVaultAccessPolicy**</span><span class="sxs-lookup"><span data-stu-id="d49db-223">**Set-AzureRmKeyVaultAccessPolicy**</span></span>
- <span data-ttu-id="d49db-224">A permissão `all` foi removida de `PermissionsToKeys`, `PermissionsToSecrets` e `PermissionsToCertificates`.</span><span class="sxs-lookup"><span data-stu-id="d49db-224">The `all` permission was removed from `PermissionsToKeys`, `PermissionsToSecrets`, and `PermissionsToCertificates`.</span></span>

<span data-ttu-id="d49db-225">**Geral**</span><span class="sxs-lookup"><span data-stu-id="d49db-225">**General**</span></span>
- <span data-ttu-id="d49db-226">A propriedade `ValueFromPipelineByPropertyName` foi removida de todos os cmdlets onde a tubagem por `InputObject` foi ativada.</span><span class="sxs-lookup"><span data-stu-id="d49db-226">The `ValueFromPipelineByPropertyName` property was removed from all cmdlets where piping by `InputObject` was enabled.</span></span>  <span data-ttu-id="d49db-227">Os cmdlets afetados são:</span><span class="sxs-lookup"><span data-stu-id="d49db-227">The cmdlets affected are:</span></span>
    - `Add-AzureKeyVaultCertificate`
    - `Add-AzureKeyVaultCertificateContact`
    - `Add-AzureKeyVaultKey`
    - `Backup-AzureKeyVaultKey`
    - `Backup-AzureKeyVaultSecret`
    - `Get-AzureKeyVaultCertficate`
    - `Get-AzureKeyVaultCertificateContact`
    - `Get-AzureKeyVaultCertificateIssuer`
    - `Get-AzureKeyVaultCertificateOperation`
    - `Get-AzureKeyVaultCertificatePolicy`
    - `Get-AzureKeyVaultKey`
    - `Get-AzureKeyVaultManagedStorageAccount`
    - `Get-AzureKeyVaultManagedStorageSasDefinition`
    - `Get-AzureKeyVaultSecret`
    - `Remove-AzureRmKeyVault`
    - `Remove-AzureRmKeyVaultAccessPolicy`
    - `Remove-AzureKeyVaultCertificate`
    - `Remove-AzureKeyVaultCertificateContact`
    - `Remove-AzureKeyVaultCertificateIssuer`
    - `Remove-AzureKeyVaultCertificateOperation`
    - `Remove-AzureKeyVaultKey`
    - `Remove-AzureKeyVaultManagedStorageAccount`
    - `Remove-AzureKeyVaultManagedStorageSasDefinition`
    - `Remove-AzureKeyVaultSecret`
    - `Restore-AzureKeyVaultKey`
    - `Restore-AzureKeyVaultSecret`
    - `Set-AzureRmKeyVaultAccessPolicy`
    - `Set-AzureKeyVaultCertificateAttribute`
    - `Set-AzureKeyVaultCertificateIssuer`
    - `Set-AzureKeyVaultCertificatePolicy`
    - `Set-AzureKeyVaultKeyAttribute`
    - `Set-AzureKeyVaultManagedStorageSasDefinition`
    - `Set-AzureKeyVaultSecret`
    - `Set-AzureKeyVaultSecretAttribute`
    - `Stop-AzureKeyVaultCertificateOperation`
    - `Undo-AzureKeyVaultCertificateRemoval`
    - `Undo-AzureKeyVaultKeyRemoval`
    - `Undo-AzureRmKeyVaultRemoval`
    - `Undo-AzureKeyVaultSecretRemoval`
    - `Update-AzureKeyVaultManagedStorageAccount`
    - `Update-AzureKeyVaultManagedStorageAccountKey`

- <span data-ttu-id="d49db-228">`ConfirmImpact` níveis foram removidos de todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d49db-228">`ConfirmImpact` levels were removed from all cmdlets.</span></span>  <span data-ttu-id="d49db-229">Os cmdlets afetados são:</span><span class="sxs-lookup"><span data-stu-id="d49db-229">The cmdlets affected are:</span></span>
    - `Remove-AzureRmKeyVault`
    - `Remove-AzureKeyVaultCertificate`
    - `Remove-AzureKeyVaultCertificateIssuer`
    - `Remove-AzureKeyVaultCertificateOperation`
    - `Remove-AzureKeyVaultKey`
    - `Remove-AzureKeyVaultManagedStorageAccount`
    - `Remove-AzureKeyVaultManagedStorageSasDefinition`
    - `Remove-AzureKeyVaultSecret`
    - `Stop-AzureKeyVaultCertificateOperation`
    - `Update-AzureKeyVaultManagedStorageAccountKey`

- <span data-ttu-id="d49db-230">O `IKeyVaultDataServiceClient` foi atualizado para todas as operações de Certificado devolverem PSTypes em vez de tipos de SDK.</span><span class="sxs-lookup"><span data-stu-id="d49db-230">The `IKeyVaultDataServiceClient` was updated so all Certificate operations return PSTypes instead of SDK types.</span></span> <span data-ttu-id="d49db-231">Isto inclui:</span><span class="sxs-lookup"><span data-stu-id="d49db-231">This includes:</span></span>
    - `SetCertificateContacts`
    - `GetCertificateContacts`
    - `GetCertificate`
    - `GetDeletedCertificate`
    - `MergeCertificate`
    - `ImportCertificate`
    - `DeleteCertificate`
    - `RecoverCertificate`
    - `EnrollCertificate`
    - `UpdateCertificate`
    - `GetCertificateOperation`
    - `DeleteCertificateOperation`
    - `CancelCertificateOperation`
    - `GetCertificatePolicy`
    - `UpdateCertificatePolicy`
    - `GetCertificateIssuer`
    - `SetCertificateIssuer`
    - `DeleteCertificateIssuer`

## <a name="breaking-changes-to-azurermnetwork-cmdlets"></a><span data-ttu-id="d49db-232">Alterações interruptivas aos cmdlets AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d49db-232">Breaking changes to AzureRM.Network cmdlets</span></span>


<span data-ttu-id="d49db-233">**Add-AzureRmApplicationGatewayBackendHttpSettings**</span><span class="sxs-lookup"><span data-stu-id="d49db-233">**Add-AzureRmApplicationGatewayBackendHttpSettings**</span></span>
- <span data-ttu-id="d49db-234">O parâmetro `ProbeEnabled` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-234">The parameter `ProbeEnabled` was removed</span></span>

<span data-ttu-id="d49db-235">**Add-AzureRmVirtualNetworkPeering**</span><span class="sxs-lookup"><span data-stu-id="d49db-235">**Add-AzureRmVirtualNetworkPeering**</span></span>
- <span data-ttu-id="d49db-236">Os aliases de parâmetro `AlloowGatewayTransit` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-236">The parameter alias `AlloowGatewayTransit` was removed</span></span>

<span data-ttu-id="d49db-237">**New-AzureRmApplicationGatewayBackendHttpSettings**</span><span class="sxs-lookup"><span data-stu-id="d49db-237">**New-AzureRmApplicationGatewayBackendHttpSettings**</span></span>
- <span data-ttu-id="d49db-238">O parâmetro `ProbeEnabled` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-238">The parameter `ProbeEnabled` was removed</span></span>

<span data-ttu-id="d49db-239">**Set-AzureRmApplicationGatewayBackendHttpSettings**</span><span class="sxs-lookup"><span data-stu-id="d49db-239">**Set-AzureRmApplicationGatewayBackendHttpSettings**</span></span>
- <span data-ttu-id="d49db-240">O parâmetro `ProbeEnabled` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-240">The parameter `ProbeEnabled` was removed</span></span>

## <a name="breaking-changes-to-azurermrediscache-cmdlets"></a><span data-ttu-id="d49db-241">Alterações interruptivas aos cmdlets AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d49db-241">Breaking changes to AzureRM.RedisCache cmdlets</span></span>

<span data-ttu-id="d49db-242">**New-AzureRmRedisCache**</span><span class="sxs-lookup"><span data-stu-id="d49db-242">**New-AzureRmRedisCache**</span></span>
- <span data-ttu-id="d49db-243">Os parâmetros `Subnet` e `VirtualNetwork` foram removidos em favor de `SubnetId`</span><span class="sxs-lookup"><span data-stu-id="d49db-243">The parameters `Subnet` and `VirtualNetwork` were removed in favor of `SubnetId`</span></span>
- <span data-ttu-id="d49db-244">O parâmetro `RedisVersion` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-244">The parameter `RedisVersion` was removed</span></span>
- <span data-ttu-id="d49db-245">O parâmetro `MaxMemoryPolicy` foi removido em favor de `RedisConfiguration`</span><span class="sxs-lookup"><span data-stu-id="d49db-245">The parameter `MaxMemoryPolicy` was removed in favor of `RedisConfiguration`</span></span>

```powershell-interactive
# Old
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -MaxMemoryPolicy "allkeys-lru"

# New
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

<span data-ttu-id="d49db-246">**Set-AzureRmRedisCache**</span><span class="sxs-lookup"><span data-stu-id="d49db-246">**Set-AzureRmRedisCache**</span></span>
- <span data-ttu-id="d49db-247">O parâmetro `MaxMemoryPolicy` foi removido em favor de `RedisConfiguration`</span><span class="sxs-lookup"><span data-stu-id="d49db-247">The parameter `MaxMemoryPolicy` was removed in favor of `RedisConfiguration`</span></span>

```powershell-interactive
# Old
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -MaxMemoryPolicy "allkeys-lru"

# New
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

## <a name="breaking-changes-to-azurermresources-cmdlets"></a><span data-ttu-id="d49db-248">Alterações interruptivas aos cmdlets AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d49db-248">Breaking changes to AzureRM.Resources cmdlets</span></span>

<span data-ttu-id="d49db-249">**Find-AzureRmResource**</span><span class="sxs-lookup"><span data-stu-id="d49db-249">**Find-AzureRmResource**</span></span>
- <span data-ttu-id="d49db-250">Este cmdlet foi removido e a funcionalidade foi movida para `Get-AzureRmResource`</span><span class="sxs-lookup"><span data-stu-id="d49db-250">This cmdlet was removed and the functionality was moved into `Get-AzureRmResource`</span></span>

```powershell-interactive
# Old
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupNameContains "ResourceGroup"
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceNameContains "test"

# New
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupName "*ResourceGroup*"
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -Name "*test*"
```

<span data-ttu-id="d49db-251">**Find-AzureRmResourceGroup**</span><span class="sxs-lookup"><span data-stu-id="d49db-251">**Find-AzureRmResourceGroup**</span></span>
- <span data-ttu-id="d49db-252">Este cmdlet foi removido e a funcionalidade foi movida para `Get-AzureRmResourceGroup`</span><span class="sxs-lookup"><span data-stu-id="d49db-252">This cmdlet was removed and the functionality was moved into `Get-AzureRmResourceGroup`</span></span>

```powershell-interactive
# Old
Find-AzureRmResourceGroup
Find-AzureRmResourceGroup -Tag @{ "testtag" = $null }
Find-AzureRmResourceGroup -Tag @{ "testtag" = "testval" }

# New
Get-AzureRmResourceGroup
Get-AzureRmResourceGroup -Tag @{ "testtag" = $null }
Get-AzureRmResourceGroup -Tag @{ "testtag" = "testval" }
```

<span data-ttu-id="d49db-253">**Get-AzureRmRoleDefinition**</span><span class="sxs-lookup"><span data-stu-id="d49db-253">**Get-AzureRmRoleDefinition**</span></span>
- <span data-ttu-id="d49db-254">O parâmetro `AtScopeAndBelow` foi removido.</span><span class="sxs-lookup"><span data-stu-id="d49db-254">Parameter `AtScopeAndBelow` was removed.</span></span>

```powershell-interactive

# Old
Get-AzureRmRoleDefinition [other required parameters] -AtScopeAndBelow

# New
Get-AzureRmRoleDefinition [other required parameters]
```

## <a name="breaking-changes-to-azurermstorage-cmdlets"></a><span data-ttu-id="d49db-255">Alterações interruptivas aos cmdlets AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d49db-255">Breaking changes to AzureRM.Storage cmdlets</span></span>

<span data-ttu-id="d49db-256">**New-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="d49db-256">**New-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="d49db-257">O parâmetro `EnableEncryptionService` foi removido</span><span class="sxs-lookup"><span data-stu-id="d49db-257">The parameter `EnableEncryptionService` was removed</span></span>

<span data-ttu-id="d49db-258">**Set-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="d49db-258">**Set-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="d49db-259">Os parâmetros `EnableEncryptionService` e `DisableEncryptionService` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-259">The parameters `EnableEncryptionService` and `DisableEncryptionService` were removed</span></span>

## <a name="removed-modules"></a><span data-ttu-id="d49db-260">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="d49db-260">Removed modules</span></span>

### `AzureRM.ServerManagement`

<span data-ttu-id="d49db-261">O serviço de Ferramentas de Gestão do Servidor foi [extinto no ano passado](https://blogs.technet.microsoft.com/servermanagement/2017/05/17/smt-preview-service-is-being-retired-on-june-30-2017/) e, consequentemente, o módulo correspondente para SMT, `AzureRM.ServerManagement`, foi removido do `AzureRM` e deixará de ser enviado daqui para a frente.</span><span class="sxs-lookup"><span data-stu-id="d49db-261">The Server Management Tools service was [retired last year](https://blogs.technet.microsoft.com/servermanagement/2017/05/17/smt-preview-service-is-being-retired-on-june-30-2017/), and as a result, the corresponding module for SMT, `AzureRM.ServerManagement`, was removed from `AzureRM` and will stop shipping moving forward.</span></span>

### `AzureRM.SiteRecovery`

<span data-ttu-id="d49db-262">O módulo `AzureRM.SiteRecovery` está a ser substituído por `AzureRM.RecoveryServices.SiteRecovery`, que é um superconjunto funcional do módulo `AzureRM.SiteRecovery` e inclui um novo conjunto de cmdlets equivalentes.</span><span class="sxs-lookup"><span data-stu-id="d49db-262">The `AzureRM.SiteRecovery` module is being superseded by `AzureRM.RecoveryServices.SiteRecovery`, which is a functional superset of the `AzureRM.SiteRecovery` module and includes a new set of equivalent cmdlets.</span></span> <span data-ttu-id="d49db-263">Pode encontrar a lista completa de mapeamentos dos cmdlets antigos para os novos abaixo:</span><span class="sxs-lookup"><span data-stu-id="d49db-263">The full list of mappings from old to new cmdlets can be found below:</span></span>

| <span data-ttu-id="d49db-264">Cmdlet preterido</span><span class="sxs-lookup"><span data-stu-id="d49db-264">Deprecated cmdlet</span></span>                                        | <span data-ttu-id="d49db-265">Cmdlet equivalente</span><span class="sxs-lookup"><span data-stu-id="d49db-265">Equivalent cmdlet</span></span>                                                | <span data-ttu-id="d49db-266">Aliases</span><span class="sxs-lookup"><span data-stu-id="d49db-266">Aliases</span></span>                                  |
|----------------------------------------------------------|------------------------------------------------------------------|------------------------------------------|
| `Edit-AzureRmSiteRecoveryRecoveryPlan`                   | `Edit-AzureRmRecoveryServicesAsrRecoveryPlan`                    | `Edit-ASRRecoveryPlan`                   |
| `Get-AzureRmSiteRecoveryFabric`                          | `Get-AzureRmRecoveryServicesAsrFabric`                           | `Get-ASRFabric`                          |
| `Get-AzureRmSiteRecoveryJob`                             | `Get-AzureRmRecoveryServicesAsrJob`                              | `Get-ASRJob`                             |
| `Get-AzureRmSiteRecoveryNetwork`                         | `Get-AzureRmRecoveryServicesAsrNetwork`                          | `Get-ASRNetwork`                         |
| `Get-AzureRmSiteRecoveryNetworkMapping`                  | `Get-AzureRmRecoveryServicesAsrNetworkMapping`                   | `Get-ASRNetworkMapping`                  |
| `Get-AzureRmSiteRecoveryPolicy`                          | `Get-AzureRmRecoveryServicesAsrPolicy`                           | `Get-ASRPolicy`                          |
| `Get-AzureRmSiteRecoveryProtectableItem`                 | `Get-AzureRmRecoveryServicesAsrProtectableItem`                  | `Get-ASRProtectableItem`                 |
| `Get-AzureRmSiteRecoveryProtectionContainer`             | `Get-AzureRmRecoveryServicesAsrProtectionContainer`              | `Get-ASRProtectionContainer`             |
| `Get-AzureRmSiteRecoveryProtectionContainerMapping`      | `Get-AzureRmRecoveryServicesAsrProtectionContainerMapping`       | `Get-ASRProtectionContainerMapping`      |
| `Get-AzureRmSiteRecoveryProtectionEntity`                | `Get-AzureRmRecoveryServicesAsrProtectableItem`                  | `Get-ASRProtectableItem`                 |
| `Get-AzureRmSiteRecoveryRecoveryPlan`                    | `Get-AzureRmRecoveryServicesAsrRecoveryPlan`                     | `Get-ASRRecoveryPlan`                    |
| `Get-AzureRmSiteRecoveryRecoveryPoint`                   | `Get-AzureRmRecoveryServicesAsrRecoveryPoint`                    | `Get-ASRRecoveryPoint`                   |
| `Get-AzureRmSiteRecoveryReplicationProtectedItem`        | `Get-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Get-ASRReplicationProtectedItem`        |
| `Get-AzureRmSiteRecoveryServer`                          | `Get-AzureRmRecoveryServicesAsrServicesProvider`                 | `Get-ASRServicesProvider`                |
| `Get-AzureRmSiteRecoveryServicesProvider`                | `Get-AzureRmRecoveryServicesAsrServicesProvider`                 | `Get-ASRServicesProvider`                |
| `Get-AzureRmSiteRecoverySite`                            | `Get-AzureRmRecoveryServicesAsrFabric`                           | `Get-ASRFabric`                          |
| `Get-AzureRmSiteRecoveryStorageClassification`           | `Get-AzureRmRecoveryServicesAsrStorageClassification`            | `Get-ASRStorageClassification`           |
| `Get-AzureRmSiteRecoveryStorageClassificationMapping`    | `Get-AzureRmRecoveryServicesAsrStorageClassificationMapping`     | `Get-ASRStorageClassificationMapping`    |
| `Get-AzureRmSiteRecoveryVault`                           | `Get-AzureRmRecoveryServicesVault`                               |                                          |
| `Get-AzureRmSiteRecoveryVaultSettings`                   | `Get-AzureRmRecoveryServicesAsrVaultContext`                     |                                          |
| `Get-AzureRmSiteRecoveryVaultSettingsFile`               | `Get-AzureRmRecoveryServicesVaultSettingsFile`                   |                                          |
| `Get-AzureRmSiteRecoveryVM`                              | `Get-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Get-ASRReplicationProtectedItem`        |
| `Import-AzureRmSiteRecoveryVaultSettingsFile`            | `Import-AzureRmRecoveryServicesAsrVaultSettingsFile`             |                                          |
| `New-AzureRmSiteRecoveryFabric`                          | `New-AzureRmRecoveryServicesAsrFabric`                           | `New-ASRFabric`                          |
| `New-AzureRmSiteRecoveryNetworkMapping`                  | `New-AzureRmRecoveryServicesAsrNetworkMapping`                   | `New-ASRNetworkMapping`                  |
| `New-AzureRmSiteRecoveryPolicy`                          | `New-AzureRmRecoveryServicesAsrPolicy`                           | `New-ASRPolicy`                          |
| `New-AzureRmSiteRecoveryProtectionContainerMapping`      | `New-AzureRmRecoveryServicesAsrProtectionContainerMapping`       | `New-ASRProtectionContainerMapping`      |
| `New-AzureRmSiteRecoveryRecoveryPlan`                    | `New-AzureRmRecoveryServicesAsrRecoveryPlan`                     | `New-ASRRecoveryPlan`                    |
| `New-AzureRmSiteRecoveryReplicationProtectedItem`        | `New-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `New-ASRReplicationProtectedItem`        |
| `New-AzureRmSiteRecoverySite`                            | `New-AzureRmRecoveryServicesAsrFabric`                           | `New-ASRFabric`                          |
| `New-AzureRmSiteRecoveryStorageClassificationMapping`    | `New-AzureRmRecoveryServicesAsrStorageClassificationMapping`     | `New-ASRStorageClassificationMapping`    |
| `New-AzureRmSiteRecoveryVault`                           | `New-AzureRmRecoveryServicesVault`                               |                                          |
| `Remove-AzureRmSiteRecoveryFabric`                       | `Remove-AzureRmRecoveryServicesAsrFabric`                        | `Remove-ASRFabric`                       |
| `Remove-AzureRmSiteRecoveryNetworkMapping`               | `Remove-AzureRmRecoveryServicesAsrNetworkMapping`                | `Remove-ASRNetworkMapping`               |
| `Remove-AzureRmSiteRecoveryPolicy`                       | `Remove-AzureRmRecoveryServicesAsrPolicy`                        | `Remove-ASRPolicy`                       |
| `Remove-AzureRmSiteRecoveryProtectionContainerMapping`   | `Remove-AzureRmRecoveryServicesAsrProtectionContainerMapping`    | `Remove-ASRProtectionContainerMapping`   |
| `Remove-AzureRmSiteRecoveryRecoveryPlan`                 | `Remove-AzureRmRecoveryServicesAsrRecoveryPlan`                  | `Remove-ASRRecoveryPlan`                 |
| `Remove-AzureRmSiteRecoveryReplicationProtectedItem`     | `Remove-AzureRmRecoveryServicesAsrReplicationProtectedItem`      | `Remove-ASRReplicationProtectedItem`     |
| `Remove-AzureRmSiteRecoveryServer`                       | `Remove-AzureRmRecoveryServicesAsrServicesProvider`              |                                          |
| `Remove-AzureRmSiteRecoveryServicesProvider`             | `Remove-AzureRmRecoveryServicesAsrServicesProvider`              | `Remove-ASRServicesProvider`             |
| `Remove-AzureRmSiteRecoverySite`                         | `Remove-AzureRmRecoveryServicesAsrFabric`                        | `Remove-ASRFabric`                       |
| `Remove-AzureRmSiteRecoveryStorageClassificationMapping` | `Remove-AzureRmRecoveryServicesAsrStorageClassificationMapping`  | `Remove-ASRStorageClassificationMapping` |
| `Remove-AzureRmSiteRecoveryVault`                        | `Remove-AzureRmRecoveryServicesVault`                            |                                          |
| `Restart-AzureRmSiteRecoveryJob`                         | `Restart-AzureRmRecoveryServicesAsrJob`                          | `Restart-ASRJob`                         |
| `Resume-AzureRmSiteRecoveryJob`                          | `Resume-AzureRmRecoveryServicesAsrJob`                           | `Resume-ASRJob`                          |
| `Set-AzureRmSiteRecoveryProtectionEntity`                | `New-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `New-ASRReplicationProtectedItem`        |
| `Set-AzureRmSiteRecoveryReplicationProtectedItem`        | `Set-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Set-ASRReplicationProtectedItem`        |
| `Set-AzureRmSiteRecoveryVaultSettings`                   | `Set-AzureRmRecoveryServicesAsrVaultContext`                     | `Set-ASRVaultContext`                    |
| `Set-AzureRmSiteRecoveryVM`                              | `Set-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Set-ASRReplicationProtectedItem`        |
| `Start-AzureRmSiteRecoveryApplyRecoveryPoint`            | `Start-AzureRmRecoveryServicesAsrApplyRecoveryPoint`             | `Start-ASRApplyRecoveryPoint`            |
| `Start-AzureRmSiteRecoveryCommitFailoverJob`             | `Start-AzureRmRecoveryServicesAsrCommitFailoverJob`              | `Start-ASRCommitFailoverJob`             |
| `Start-AzureRmSiteRecoveryPlannedFailoverJob`            | `Start-AzureRmRecoveryServicesAsrPlannedFailoverJob`             | `Start-ASRPlannedFailoverJob`            |
| `Start-AzureRmSiteRecoveryPolicyAssociationJob`          | `New-AzureRmRecoveryServicesAsrProtectionContainerMapping`       | `New-ASRProtectionContainerMapping`      |
| `Start-AzureRmSiteRecoveryPolicyDissociationJob`         | `Remove-AzureRmRecoveryServicesAsrProtectionContainerMapping`    | `Remove-ASRProtectionContainerMapping`   |
| `Start-AzureRmSiteRecoveryTestFailoverJob`               | `Start-AzureRmRecoveryServicesAsrTestFailoverJob`                | `Start-ASRTestFailoverJob`               |
| `Start-AzureRmSiteRecoveryUnplannedFailoverJob`          | `Start-AzureRmRecoveryServicesAsrUnplannedFailoverJob`           | `Start-ASRUnplannedFailoverJob`          |
| `Stop-AzureRmSiteRecoveryJob`                            | `Stop-AzureRmRecoveryServicesAsrJob`                             | `Stop-ASRJob`                            |
| `Update-AzureRmSiteRecoveryPolicy`                       | `Update-AzureRmRecoveryServicesAsrPolicy`                        | `Update-ASRPolicy`                       |
| `Update-AzureRmSiteRecoveryProtectionDirection`          | `Update-AzureRmRecoveryServicesAsrProtectionDirection`           | `Update-ASRProtectionDirection`          |
| `Update-AzureRmSiteRecoveryRecoveryPlan`                 | `Update-AzureRmRecoveryServicesAsrRecoveryPlan`                  | `Update-ASRRecoveryPlan`                 |
| `Update-AzureRmSiteRecoveryServer`                       | `Update-AzureRmRecoveryServicesAsrServicesProvider`              | `Update-ASRServicesProvider`             |
| `Update-AzureRmSiteRecoveryServicesProvider`             | `Update-AzureRmRecoveryServicesAsrvCenter`                       | `Update-ASRvCenter`                      |
