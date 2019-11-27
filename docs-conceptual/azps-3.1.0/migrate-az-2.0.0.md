---
title: Guia de migração para o Az 2.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/24/2019
ms.openlocfilehash: 5f15d1a4f1e8416d7214aceb78494867fe4aad52
ms.sourcegitcommit: 45e1823aa1a792840aa4829831b5f67a9d5d24a0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/26/2019
ms.locfileid: "74537180"
---
# <a name="migration-guide-for-az-200"></a>Guia de migração para o Az 2.0.0

Este documento descreve as alterações realizadas entre as versões 1.0.0 e 2.0.0 do Az 

## <a name="table-of-contents"></a>Índice
- [Alterações interruptivas do módulo](#module-breaking-changes)
  - [Az.Compute](#azcompute)
  - [Az.HDInsight](#azhdinsight)
  - [Az.Storage](#azstorage)

## <a name="module-breaking-changes"></a>Alterações interruptivas do módulo

### <a name="azcompute"></a>Az.Compute

- Foi removido o parâmetro `Managed` dos cmdlets `New-AzAvailabilitySet` e `Update-AzAvailabilitySet` em favor da utilização de ```Sku = Aligned```

  #### <a name="before"></a>Antes

  ```powershell
  Update-AzAvailabilitySet -Managed
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Update-AzAvailabilitySet -Sku Aligned
  ```
- Para consistência, foi removido o parâmetro `Image` dos parâmetros "ByName" e "ByResourceId" definidos em `Update-AzImage` 
  
  #### <a name="before"></a>Antes

  Tenha em atenção que o código abaixo funciona, mas o parâmetro ImageName transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Image $Image -Tag $tags

  Update-AzImage -ResourceId $Id -Image $Image -Tag $tags
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Tag $tags

  Update-AzImage -ResourceId $Id -Tag $tags
  ```

- Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Restart-AzVM`
  
  #### <a name="before"></a>Antes

  Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.
  ```powershell
  Restart-AzVM -InputObject $VM -Name $Name 

  Restart-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Restart-AzVM -InputObject $VM

  Restart-AzVM -ResourceId $Id
  ```

- Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Start-AzVM`
  
  #### <a name="before"></a>Antes

  Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.

  ```powershell
  Start-AzVM -InputObject $VM -Name $Name 

  Start-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Start-AzVM -InputObject $VM

  Start-AzVM -ResourceId $Id
  ```

- Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Stop-AzVM`
  
  #### <a name="before"></a>Antes

  Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.

  ```powershell
  Stop-AzVM -InputObject $VM -Name $Name 

  Stop-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Stop-AzVM -InputObject $VM

  Stop-AzVM -ResourceId $Id
  ```

- Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Remove-AzVM`
  
  #### <a name="before"></a>Antes

  Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.

  ```powershell
  Remove-AzVM -InputObject $VM -Name $Name

  Remove-AzVM -ResourceId $Id -Name $Name 
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Remove-AzVM -InputObject $VM 

  Remove-AzVM -ResourceId $Id 
  ```

- Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Set-AzVM`
  
  #### <a name="before"></a>Antes

  Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.

  ```powershell
  Set-AzVM -InputObject $VM -Name $Name ...

  Set-AzVM -ResourceId $Id -Name $Name ...
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Set-AzVM -InputObject $VM ...

  Set-AzVM -ResourceId $Id ...
  ```

- Para consistência, foi removido o parâmetro `Name` dos parâmetros "ByObject" e "ByResourceId" definidos em `Save-AzVMImage` 
  
  #### <a name="before"></a>Antes
  Tenha em atenção que o código abaixo funciona, mas o parâmetro Name transmitido não é utilizado, pelo que a remoção deste parâmetro não tem qualquer impacto funcional.
  ```powershell
  Save-AzVMImage -InputObject $VM -Name $Name ...

  Save-AzVMImage -ResourceId $Id -Name $Name ...
  ```
  #### <a name="after"></a>Depois
  ```powershell
  Save-AzVMImage -InputObject $VM ...

  Save-AzVMImage -ResourceId $Id ...
  ```

- Foi adicionada a propriedade ProtectionPolicy para encapsular a propriedade `ProtectFromScaleIn` em `PSVirtualMachineScaleSetVM`

  #### <a name="before"></a>Antes

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectFromScaleIn = $true
  ```

  #### <a name="after"></a>Depois

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  ```

- Foi adicionada a propriedade ```EncryptionSettingsCollection``` para delimitar a propriedade `EncryptionSettings` em `PSDisk`

  #### <a name="before"></a>Antes

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

  #### <a name="after"></a>Depois

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

- Foi adicionada a propriedade ```EncryptionSettingsCollection``` para delimitar a propriedade `EncryptionSettings` em `PSSnapshot`

  #### <a name="before"></a>Antes

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

  #### <a name="after"></a>Depois

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

- Foi removida a propriedade `VirtualMachineProfile` de `PSVirtualMachineScaleSet`

  #### <a name="before"></a>Antes

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.VirtualMachineProfile.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

  #### <a name="after"></a>Depois

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

- O cmdlet `Set-AzVMBootDiagnostic` removeu o alias para `Set-AzVMBootDiagnostics`

  #### <a name="before"></a>Antes

  Utilização de alias preterido

  ```powershell
  Set-AzVMBootDiagnostics
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Set-AzVMBootDIagnostic
  ```

- O cmdlet `Export-AzLogAnalyticThrottledRequest` removeu o alias para `Export-AzLogAnalyticThrottledRequests`

  #### <a name="before"></a>Antes

  Utilização de alias preterido

  ```powershell
  Export-AzLogAnalyticThrottledRequests
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Export-AzLogAnalyticThrottledRequest
  ```

### <a name="azhdinsight"></a>Az.HDInsight

- Foram removidos os cmdlets `Grant-AzHDInsightHttpServicesAccess` e `Revoke-AzHDInsightHttpServicesAccess`. Já não são necessários porque o acesso HTTP está sempre ativado em todos os clusters do HDInsight.
- Foi adicionado um novo cmdlet `Set-AzHDInsightGatewayCredential`. Utilize este cmdlet para alterar o nome de utilizador e a palavra-passe HTTP do gateway (substitui `Grant-AzHDInsightHttpServicesAccess`).
- Foi atualizado o cmdlet `Get-AzHDInsightJobOutput` para suportar acesso granular baseado em funções à chave de armazenamento.
    - Os utilizadores com as funções Operador de Clusters, Contribuidor ou Proprietário do HDInsight não serão afetados.
    - Os utilizadores apenas com a função Leitor terão de especificar o parâmetro `DefaultStorageAccountKey` explicitamente.

Para obter mais informações sobre estas alterações ao acesso baseado em funções, veja [aka.ms/hdi-config-update](http://aka.ms/hdi-config-update)

  #### <a name="before"></a>Antes

  ```powershell
  Grant-AzHDInsightHttpServicesAccess -ClusterName $cluster -HttpCredential $credential
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Set-AzHDInsightGatewayCredential -ClusterName $cluster -HttpCredential $credential
  ```

###  <a name="users-with-only-reader-role-for-cmdlet-get-azhdinsightjoboutput"></a>Utilizadores apenas com a função Leitor para o cmdlet Get-AzHDInsightJobOutput

  ####  <a name="before"></a>Antes

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId
  ```

  #### <a name="after"></a>Depois

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId -DefaultStorageAccountKey $storageAccountKey
  ```

### <a name="azstorage"></a>Az.Storage

- Os espaços de nomes para os tipos devolvidos dos cmdlets Blob, Fila e Ficheiro foram alterados de `Microsoft.WindowsAzure.Storage` para `Microsoft.Azure.Storage`.  Embora não seja tecnicamente uma alteração interruptiva, de acordo com a respetiva política, podem ser necessárias algumas alterações ao código que utiliza os métodos do SDK .NET de Armazenamento para interagir com os objetos devolvidos por estes cmdlets.

  #### <a name="example-1--add-a-message-to-a-queue-change-cloudqueuemessage-object-namespace"></a>Exemplo 1:  Adicionar uma mensagem a uma Fila (alterar o espaço de nomes do objeto CloudQueueMessage)

  Antes: 

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.WindowsAzure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)" -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  Depois:

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.Azure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)"  -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  #### <a name="example-2--fetch-blobfile-attributes-with-accesscondition-change-accesscondition-object-namespace"></a>Exemplo 2:  Obter os atributos de Blob/Ficheiro com AccessCondition (alterar o espaço de nomes do objeto AccessCondition)

  Antes: 

  ```powershell
  $accessCondition= New-Object Microsoft.WindowsAzure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

  Depois:

  ```powershell
  $accessCondition= New-Object Microsoft.Azure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

- Embora não seja tecnicamente uma alteração interruptiva, irá reparar nas diferenças de saída na propriedade Sku.Name das Contas de Armazenamento devolvidas a partir das alterações de `New/Get/Set-AzStorageAccount`. (Após a alteração, o SkuName de entrada e saída estão alinhados.)
  - "StandardLRS" -> "Standard_LRS";
  - "StandardGRS" -> "Standard_GRS";
  - "StandardRAGRS" -> "Standard_RAGRS";
  - "StandardZRS" -> "Standard_ZRS";
  - "PremiumLRS" -> "Premium_LRS";

- Foi alterado o comportamento de serviço padrão ao criar uma conta de armazenamento sem especificar uma Variante.  Nas versões anteriores, quando foi criada uma conta de armazenamento sem qualquer atributo `Kind` especificado, foi utilizada a Variante da conta de armazenamento de `Storage` na nova versão `StorageV2`, sendo o valor predefinido `Kind`. Se precisar de criar uma conta de armazenamento V1 com a Variante "Armazenamento", adicione o parâmetro "-Kind Storage"

  #### <a name="example--create-a-storage-account-default-kind-change"></a>Exemplo: Criar uma conta de armazenamento (alterar a Variante predefinida)  

  Antes:

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName     Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------     ----      ---------- ------------          ----------------- ----------------------
  accountname        groupname         westus   StandardLRS Storage   Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```

  Depois:

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName      Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------      ----      ----------  ------------          ----------------- ----------------------
  accountname        groupname         westus   Standard_LRS StorageV2 Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```
