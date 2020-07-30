---
title: Guia de migração para o Az 2.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 2.0.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/24/2019
ms.openlocfilehash: 91362f3cc6b35e96a543c1304fb55acbf373d291
ms.sourcegitcommit: 5523170e571fbd1dc93bd0fa4223aba3b324d3b0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/25/2020
ms.locfileid: "85363456"
---
# <a name="migration-guide-for-az-200"></a><span data-ttu-id="8e1c9-103">Guia de migração para o Az 2.0.0</span><span class="sxs-lookup"><span data-stu-id="8e1c9-103">Migration Guide for Az 2.0.0</span></span>

<span data-ttu-id="8e1c9-104">Este documento descreve as alterações realizadas entre as versões 1.0.0 e 2.0.0 do Az</span><span class="sxs-lookup"><span data-stu-id="8e1c9-104">This document describes the changes between the 1.0.0 and 2.0.0 versions of Az</span></span> 

## <a name="table-of-contents"></a><span data-ttu-id="8e1c9-105">Índice</span><span class="sxs-lookup"><span data-stu-id="8e1c9-105">Table of Contents</span></span>
- [<span data-ttu-id="8e1c9-106">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="8e1c9-106">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="8e1c9-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8e1c9-107">Az.Compute</span></span>](#azcompute)
  - [<span data-ttu-id="8e1c9-108">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8e1c9-108">Az.HDInsight</span></span>](#azhdinsight)
  - [<span data-ttu-id="8e1c9-109">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8e1c9-109">Az.Storage</span></span>](#azstorage)

## <a name="module-breaking-changes"></a><span data-ttu-id="8e1c9-110">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="8e1c9-110">Module breaking changes</span></span>

### <a name="azcompute"></a><span data-ttu-id="8e1c9-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8e1c9-111">Az.Compute</span></span>

- <span data-ttu-id="8e1c9-112">Foi removido o parâmetro `Managed` dos cmdlets `New-AzAvailabilitySet` e `Update-AzAvailabilitySet` em favor da utilização de ```Sku = Aligned```</span><span class="sxs-lookup"><span data-stu-id="8e1c9-112">Removed `Managed` Parameter from `New-AzAvailabilitySet` and `Update-AzAvailabilitySet` cmdlets in favor of using ```Sku = Aligned```</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-113">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-113">Before</span></span>

  ```powershell
  Update-AzAvailabilitySet -Managed
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-114">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-114">After</span></span>

  ```powershell
  Update-AzAvailabilitySet -Sku Aligned
  ```
- <span data-ttu-id="8e1c9-115">Para consistência, foi removido o parâmetro `Image` dos parâmetros "ByName" e "ByResourceId" definidos em `Update-AzImage`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-115">For consistency, removed `Image` parameter from 'ByName' and 'ByResourceId' parameter sets in `Update-AzImage`</span></span> 
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-116">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-116">Before</span></span>

  <span data-ttu-id="8e1c9-117">Tenha em atenção que o código abaixo funciona, mas o parâmetro ImageName transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-117">Note that the below code is functional, but the passed-in ImageName is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Image $Image -Tag $tags

  Update-AzImage -ResourceId $Id -Image $Image -Tag $tags
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-118">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-118">After</span></span>

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Tag $tags

  Update-AzImage -ResourceId $Id -Tag $tags
  ```

- <span data-ttu-id="8e1c9-119">Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Restart-AzVM`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-119">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Restart-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-120">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-120">Before</span></span>

  <span data-ttu-id="8e1c9-121">Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-121">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>
  ```powershell
  Restart-AzVM -InputObject $VM -Name $Name 

  Restart-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-122">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-122">After</span></span>

  ```powershell
  Restart-AzVM -InputObject $VM

  Restart-AzVM -ResourceId $Id
  ```

- <span data-ttu-id="8e1c9-123">Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Start-AzVM`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-123">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Start-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-124">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-124">Before</span></span>

  <span data-ttu-id="8e1c9-125">Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-125">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Start-AzVM -InputObject $VM -Name $Name 

  Start-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-126">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-126">After</span></span>

  ```powershell
  Start-AzVM -InputObject $VM

  Start-AzVM -ResourceId $Id
  ```

- <span data-ttu-id="8e1c9-127">Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Stop-AzVM`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-127">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Stop-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-128">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-128">Before</span></span>

  <span data-ttu-id="8e1c9-129">Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-129">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Stop-AzVM -InputObject $VM -Name $Name 

  Stop-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-130">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-130">After</span></span>

  ```powershell
  Stop-AzVM -InputObject $VM

  Stop-AzVM -ResourceId $Id
  ```

- <span data-ttu-id="8e1c9-131">Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Remove-AzVM`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-131">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Remove-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-132">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-132">Before</span></span>

  <span data-ttu-id="8e1c9-133">Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-133">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Remove-AzVM -InputObject $VM -Name $Name

  Remove-AzVM -ResourceId $Id -Name $Name 
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-134">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-134">After</span></span>

  ```powershell
  Remove-AzVM -InputObject $VM 

  Remove-AzVM -ResourceId $Id 
  ```

- <span data-ttu-id="8e1c9-135">Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Set-AzVM`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-135">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Set-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-136">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-136">Before</span></span>

  <span data-ttu-id="8e1c9-137">Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-137">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Set-AzVM -InputObject $VM -Name $Name ...

  Set-AzVM -ResourceId $Id -Name $Name ...
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-138">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-138">After</span></span>

  ```powershell
  Set-AzVM -InputObject $VM ...

  Set-AzVM -ResourceId $Id ...
  ```

- <span data-ttu-id="8e1c9-139">Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Save-AzVMImage`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-139">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Save-AzVMImage`</span></span> 
  
  #### <a name="before"></a><span data-ttu-id="8e1c9-140">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-140">Before</span></span>
  <span data-ttu-id="8e1c9-141">Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-141">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>
  ```powershell
  Save-AzVMImage -InputObject $VM -Name $Name ...

  Save-AzVMImage -ResourceId $Id -Name $Name ...
  ```
  #### <a name="after"></a><span data-ttu-id="8e1c9-142">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-142">After</span></span>
  ```powershell
  Save-AzVMImage -InputObject $VM ...

  Save-AzVMImage -ResourceId $Id ...
  ```

- <span data-ttu-id="8e1c9-143">Foi adicionada a propriedade ProtectionPolicy para encapsular a propriedade `ProtectFromScaleIn` em `PSVirtualMachineScaleSetVM`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-143">Added ProtectionPolicy property to encapsulate `ProtectFromScaleIn` property in `PSVirtualMachineScaleSetVM`</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-144">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-144">Before</span></span>

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectFromScaleIn = $true
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-145">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-145">After</span></span>

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  ```

- <span data-ttu-id="8e1c9-146">Foi adicionada a propriedade ```EncryptionSettingsCollection``` para delimitar a propriedade `EncryptionSettings` em `PSDisk`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-146">Added ```EncryptionSettingsCollection``` Property to enclose `EncryptionSettings` property in `PSDisk`</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-147">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-147">Before</span></span>

  ```powershell
  $disk = New-AzDisk ... | Set-AzDiskDiskEncrytionKey ...
  $disk.EncryptionSettings

  $disk = New-AzDisk ... | Set-AzDiskKeyEncrytionKey ...
  $disk.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateDiskEncryptionKey ...
  $update.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateKeyEncryptionKey ...
  $update.EncryptionSettings
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-148">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-148">After</span></span>

  ```powershell
  $disk = New-AzDisk ... | Set-AzDiskDiskEncrytionKey ...
  $disk.EncryptionSettingsCollection.EncryptionSettings

  $disk = New-AzDisk ... | Set-AzDiskKeyEncrytionKey ...
  $disk.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateDiskEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateKeyEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings
  ```

- <span data-ttu-id="8e1c9-149">Foi adicionada a propriedade ```EncryptionSettingsCollection``` para delimitar a propriedade `EncryptionSettings` em `PSSnapshot`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-149">Added ```EncryptionSettingsCollection``` Property to enclose `EncryptionSettings` property in `PSSnapshot`</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-150">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-150">Before</span></span>

  ```powershell
  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotDiskEncryptionKey ...
  $snap.EncryptionSettings

  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotKeyEncryptionKey ...
  $snap.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateDiskEncryptionKey ...
  $update.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateKeyEncryptionKey ...
  $update.EncryptionSettings
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-151">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-151">After</span></span>

  ```powershell
  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotDiskEncryptionKey ...
  $snap.EncryptionSettingsCollection.EncryptionSettings

  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotKeyEncryptionKey ...
  $snap.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateDiskEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateKeyEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings
  ```

- <span data-ttu-id="8e1c9-152">Foi removida a propriedade `VirtualMachineProfile` de `PSVirtualMachineScaleSet`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-152">Removed `VirtualMachineProfile` property from `PSVirtualMachineScaleSet`</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-153">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-153">Before</span></span>

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.VirtualMachineProfile.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-154">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-154">After</span></span>

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

- <span data-ttu-id="8e1c9-155">O cmdlet `Set-AzVMBootDiagnostic` removeu o alias para `Set-AzVMBootDiagnostics`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-155">Cmdlet `Set-AzVMBootDiagnostic` removed alias to `Set-AzVMBootDiagnostics`</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-156">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-156">Before</span></span>

  <span data-ttu-id="8e1c9-157">Utilização de alias preterido</span><span class="sxs-lookup"><span data-stu-id="8e1c9-157">Using deprecated alias</span></span>

  ```powershell
  Set-AzVMBootDiagnostics
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-158">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-158">After</span></span>

  ```powershell
  Set-AzVMBootDIagnostic
  ```

- <span data-ttu-id="8e1c9-159">O cmdlet `Export-AzLogAnalyticThrottledRequest` removeu o alias para `Export-AzLogAnalyticThrottledRequests`</span><span class="sxs-lookup"><span data-stu-id="8e1c9-159">Cmdlet `Export-AzLogAnalyticThrottledRequest` removed alias to `Export-AzLogAnalyticThrottledRequests`</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-160">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-160">Before</span></span>

  <span data-ttu-id="8e1c9-161">Utilização de alias preterido</span><span class="sxs-lookup"><span data-stu-id="8e1c9-161">Using deprectaed alias</span></span>

  ```powershell
  Export-AzLogAnalyticThrottledRequests
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-162">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-162">After</span></span>

  ```powershell
  Export-AzLogAnalyticThrottledRequest
  ```

### <a name="azhdinsight"></a><span data-ttu-id="8e1c9-163">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8e1c9-163">Az.HDInsight</span></span>

- <span data-ttu-id="8e1c9-164">Foram removidos os cmdlets `Grant-AzHDInsightHttpServicesAccess` e `Revoke-AzHDInsightHttpServicesAccess`.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-164">Removed the `Grant-AzHDInsightHttpServicesAccess` and `Revoke-AzHDInsightHttpServicesAccess` cmdlets.</span></span> <span data-ttu-id="8e1c9-165">Já não são necessários porque o acesso HTTP está sempre ativado em todos os clusters do HDInsight.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-165">These are no longer necessary because HTTP access is always enabled on all HDInsight clusters.</span></span>
- <span data-ttu-id="8e1c9-166">Foi adicionado um novo cmdlet `Set-AzHDInsightGatewayCredential`.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-166">Added a new `Set-AzHDInsightGatewayCredential`  cmdlet.</span></span> <span data-ttu-id="8e1c9-167">Utilize este cmdlet para alterar o nome de utilizador e a palavra-passe HTTP do gateway (substitui `Grant-AzHDInsightHttpServicesAccess`).</span><span class="sxs-lookup"><span data-stu-id="8e1c9-167">Use this cmdlet to change the gateway HTTP username and password (replaces `Grant-AzHDInsightHttpServicesAccess`).</span></span>
- <span data-ttu-id="8e1c9-168">Foi atualizado o cmdlet `Get-AzHDInsightJobOutput` para suportar acesso granular baseado em funções à chave de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-168">Updated the `Get-AzHDInsightJobOutput` cmdlet to support granular role-based access to the storage key.</span></span>
    - <span data-ttu-id="8e1c9-169">Os utilizadores com as funções Operador de Clusters, Contribuidor ou Proprietário do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-169">Users with HDInsight Cluster Operator, Contributor, or Owner roles will not be affected.</span></span>
    - <span data-ttu-id="8e1c9-170">Os utilizadores apenas com a função Leitor terão de especificar o parâmetro `DefaultStorageAccountKey` explicitamente.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-170">Users with only the Reader role will need to specify `DefaultStorageAccountKey` parameter explicitly.</span></span>

<span data-ttu-id="8e1c9-171">Para obter mais informações sobre estas alterações ao acesso baseado em funções, veja [aka.ms/hdi-config-update](https://aka.ms/hdi-config-update)</span><span class="sxs-lookup"><span data-stu-id="8e1c9-171">For more information about these role-based access changes, see [aka.ms/hdi-config-update](https://aka.ms/hdi-config-update)</span></span>

  #### <a name="before"></a><span data-ttu-id="8e1c9-172">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-172">Before</span></span>

  ```powershell
  Grant-AzHDInsightHttpServicesAccess -ClusterName $cluster -HttpCredential $credential
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-173">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-173">After</span></span>

  ```powershell
  Set-AzHDInsightGatewayCredential -ClusterName $cluster -HttpCredential $credential
  ```

###  <a name="users-with-only-reader-role-for-cmdlet-get-azhdinsightjoboutput"></a><span data-ttu-id="8e1c9-174">Utilizadores apenas com a função Leitor para o cmdlet Get-AzHDInsightJobOutput</span><span class="sxs-lookup"><span data-stu-id="8e1c9-174">Users with only Reader role for cmdlet Get-AzHDInsightJobOutput</span></span>

  ####  <a name="before"></a><span data-ttu-id="8e1c9-175">Antes</span><span class="sxs-lookup"><span data-stu-id="8e1c9-175">Before</span></span>

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId
  ```

  #### <a name="after"></a><span data-ttu-id="8e1c9-176">Depois</span><span class="sxs-lookup"><span data-stu-id="8e1c9-176">After</span></span>

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId -DefaultStorageAccountKey $storageAccountKey
  ```

### <a name="azstorage"></a><span data-ttu-id="8e1c9-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8e1c9-177">Az.Storage</span></span>

- <span data-ttu-id="8e1c9-178">Os espaços de nomes para os tipos devolvidos dos cmdlets Blob, Fila e Ficheiro foram alterados de `Microsoft.WindowsAzure.Storage` para `Microsoft.Azure.Storage`.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-178">Namespaces for types returned from Blob, Queue, and File cmdlets have changed their namespace from `Microsoft.WindowsAzure.Storage` to `Microsoft.Azure.Storage`.</span></span>  <span data-ttu-id="8e1c9-179">Embora não seja tecnicamente uma alteração interruptiva, de acordo com a respetiva política, podem ser necessárias algumas alterações ao código que utiliza os métodos do SDK .NET de Armazenamento para interagir com os objetos devolvidos por estes cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-179">While this is not technically a breaking change according to the breaking change policy, it may require some changes in code that uses the methods from the Storage .Net SDK to interact with the objects returned from these cmdlets.</span></span>

  #### <a name="example-1--add-a-message-to-a-queue-change-cloudqueuemessage-object-namespace"></a><span data-ttu-id="8e1c9-180">Exemplo 1:  Adicionar uma mensagem a uma Fila (alterar o espaço de nomes do objeto CloudQueueMessage)</span><span class="sxs-lookup"><span data-stu-id="8e1c9-180">Example 1:  Add a message to a Queue (change CloudQueueMessage object namespace)</span></span>

  <span data-ttu-id="8e1c9-181">Antes:</span><span class="sxs-lookup"><span data-stu-id="8e1c9-181">Before:</span></span> 

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.WindowsAzure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)" -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  <span data-ttu-id="8e1c9-182">Depois:</span><span class="sxs-lookup"><span data-stu-id="8e1c9-182">After:</span></span>

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.Azure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)"  -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  #### <a name="example-2--fetch-blobfile-attributes-with-accesscondition-change-accesscondition-object-namespace"></a><span data-ttu-id="8e1c9-183">Exemplo 2:  Obter os atributos de Blob/Ficheiro com AccessCondition (alterar o espaço de nomes do objeto AccessCondition)</span><span class="sxs-lookup"><span data-stu-id="8e1c9-183">Example 2:  Fetch Blob/File Attributes with AccessCondition (change AccessCondition object namespace)</span></span>

  <span data-ttu-id="8e1c9-184">Antes:</span><span class="sxs-lookup"><span data-stu-id="8e1c9-184">Before:</span></span> 

  ```powershell
  $accessCondition= New-Object Microsoft.WindowsAzure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

  <span data-ttu-id="8e1c9-185">Depois:</span><span class="sxs-lookup"><span data-stu-id="8e1c9-185">After:</span></span>

  ```powershell
  $accessCondition= New-Object Microsoft.Azure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

- <span data-ttu-id="8e1c9-186">Embora não seja tecnicamente uma alteração interruptiva, irá reparar nas diferenças de saída na propriedade Sku.Name das Contas de Armazenamento devolvidas a partir das alterações de `New/Get/Set-AzStorageAccount`.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-186">While not technically a breaking change, you will notice output differences in the Sku.Name property of Storage Accounts returned from  `New/Get/Set-AzStorageAccount` changes are as follows.</span></span> <span data-ttu-id="8e1c9-187">(Após a alteração, o SkuName de entrada e saída estão alinhados.)</span><span class="sxs-lookup"><span data-stu-id="8e1c9-187">(After the change, output and input SkuName are aligned.)</span></span>
  - <span data-ttu-id="8e1c9-188">"StandardLRS" -> "Standard_LRS";</span><span class="sxs-lookup"><span data-stu-id="8e1c9-188">"StandardLRS" -> "Standard_LRS";</span></span>
  - <span data-ttu-id="8e1c9-189">"StandardGRS" -> "Standard_GRS";</span><span class="sxs-lookup"><span data-stu-id="8e1c9-189">"StandardGRS" -> "Standard_GRS";</span></span>
  - <span data-ttu-id="8e1c9-190">"StandardRAGRS" -> "Standard_RAGRS";</span><span class="sxs-lookup"><span data-stu-id="8e1c9-190">"StandardRAGRS" -> "Standard_RAGRS";</span></span>
  - <span data-ttu-id="8e1c9-191">"StandardZRS" -> "Standard_ZRS";</span><span class="sxs-lookup"><span data-stu-id="8e1c9-191">"StandardZRS" -> "Standard_ZRS";</span></span>
  - <span data-ttu-id="8e1c9-192">"PremiumLRS" -> "Premium_LRS";</span><span class="sxs-lookup"><span data-stu-id="8e1c9-192">"PremiumLRS" -> "Premium_LRS";</span></span>

- <span data-ttu-id="8e1c9-193">Foi alterado o comportamento de serviço padrão ao criar uma conta de armazenamento sem especificar uma Variante.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-193">The default service behavior when creating a storage account withous specifying a Kind has changed.</span></span>  <span data-ttu-id="8e1c9-194">Nas versões anteriores, quando foi criada uma conta de armazenamento sem qualquer atributo `Kind` especificado, foi utilizada a Variante da conta de armazenamento de `Storage` na nova versão `StorageV2`, sendo o valor predefinido `Kind`.</span><span class="sxs-lookup"><span data-stu-id="8e1c9-194">In previous versions, when a storage account was created with no `Kind` specified, the Storage account Kind of `Storage` was used, in the new version `StorageV2` is the default `Kind` value.</span></span> <span data-ttu-id="8e1c9-195">Se precisar de criar uma conta de armazenamento V1 com a Variante "Armazenamento", adicione o parâmetro "-Kind Storage"</span><span class="sxs-lookup"><span data-stu-id="8e1c9-195">If you need to create a V1 Storage account with Kind 'Storage', add parameter '-Kind Storage'</span></span>

  #### <a name="example--create-a-storage-account-default-kind-change"></a><span data-ttu-id="8e1c9-196">Exemplo: Criar uma conta de armazenamento (alterar a Variante predefinida)</span><span class="sxs-lookup"><span data-stu-id="8e1c9-196">Example : Create a storage Account (Default Kind change)</span></span>  

  <span data-ttu-id="8e1c9-197">Antes:</span><span class="sxs-lookup"><span data-stu-id="8e1c9-197">Before:</span></span>

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName     Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------     ----      ---------- ------------          ----------------- ----------------------
  accountname        groupname         westus   StandardLRS Storage   Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```

  <span data-ttu-id="8e1c9-198">Depois:</span><span class="sxs-lookup"><span data-stu-id="8e1c9-198">After:</span></span>

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName      Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------      ----      ----------  ------------          ----------------- ----------------------
  accountname        groupname         westus   Standard_LRS StorageV2 Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```