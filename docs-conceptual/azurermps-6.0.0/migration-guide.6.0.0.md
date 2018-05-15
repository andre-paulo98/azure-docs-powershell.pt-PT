---
title: Alterações recentes ao Microsoft Azure PowerShell 6.0.0
description: Este guia de migração contém uma lista de alterações de interrupção realizadas no Azure PowerShell no lançamento da versão 6.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: dc88ba8a2359e92cb3aa9c3e891463e70143ddb4
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2018
---
# <a name="breaking-changes-for-microsoft-azure-powershell-600"></a>Alterações recentes ao Microsoft Azure PowerShell 6.0.0

Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell. Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço. Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.

## <a name="table-of-contents"></a>Índice

- [Alterações interruptivas gerais](#general-breaking-changes)
    - [Versão mínima do PowerShell necessária bumped para 5.0](#minimum-powershell-version-required-bumped-to-50)
    - [Gravação automática do contexto ativada por predefinição](#context-autosaved-enabled-by-default)
    - [Remoção de alias de Etiquetas](#removal-of-tags-alias)
- [Alterações interruptivas aos cmdlets AzureRM.Compute](#breaking-changes-to-azurermcompute-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.DataLakeStore](#breaking-changes-to-azurermdatalakestore-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.Dns](#breaking-changes-to-azurermdns-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.Insights](#breaking-changes-to-azurerminsights-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.KeyVault](#breaking-changes-to-azurermkeyvault-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.Network](#breaking-changes-to-azurermnetwork-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.RedisCache](#breaking-changes-to-azurermrediscache-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.Resources](#breaking-changes-to-azurermresources-cmdlets)
- [Alterações interruptivas aos cmdlets AzureRM.Storage](#breaking-changes-to-azurermstorage-cmdlets)
- [Módulos removidos](#removed-modules)
    - [`AzureRM.ServerManagement`](#azurermservermanagement)
    - [`AzureRM.SiteRecovery`](#azurermsiterecovery)

## <a name="general-breaking-changes"></a>Alterações interruptivas gerais

### <a name="minimum-powershell-version-required-bumped-to-50"></a>Versão mínima do PowerShell necessária bumped para 5.0

Anteriormente, o Azure PowerShell precisava de, _pelo menos_, a versão 3.0 do PowerShell para executar qualquer cmdlet. Daqui para a frente, este requisito será acionado para a versão 5.0 do PowerShell. Para obter informações sobre a atualização para o PowerShell 5.0, veja [esta tabela](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).

### <a name="context-autosave-enabled-by-default"></a>Gravação automática do contexto ativada por predefinição

A gravação automática do contexto é o armazenamento de informações de início de sessão do Azure que podem ser utilizadas entre sessões do PowerShell novas e diferentes. Para obter mais informações sobre a gravação automática do contexto, veja [este documento](https://docs.microsoft.com/en-us/powershell/azure/context-persistence).

Anteriormente a gravação automática do contexto estava desativada por predefinição, o que significa que as informações de início de sessão do Azure do utilizador não foram armazenadas entre sessões até executarem o cmdlet `Enable-AzureRmContextAutosave` para ativar a persistência de contexto. Daqui para a frente, a gravação automática do contexto será ativada por predefinição, o que significa que os utilizadores _sem definições guardadas da gravação automática do contexto_ terão os respetivos contextos armazenados quando iniciarem sessão pela próxima vez. Os utilizadores podem optar ativamente por não participar desta funcionalidade através do cmdlet `Disable-AzureRmContextAutosave`.

_Nota_: os utilizadores que anteriormente desativaram a gravação automática do contexto ou os utilizadores com gravação automática do contexto ativado e contextos existentes não serão afetados por esta alteração

### <a name="removal-of-tags-alias"></a>Remoção de alias de Etiquetas

O alias `Tags` para o parâmetro `Tag` foi removido entre vários cmdlets. Segue-se uma lista de módulos (e os cmdlets correspondentes) afetados por este problema:

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

## <a name="breaking-changes-to-azurermcompute-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.Compute

**Diversos**
- A propriedade de nome de sku aninhada nos tipos `PSDisk` e `PSSnapshot` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

```powershell
$disk = Get-AzureRmDisk -ResourceGroupName "MyResourceGroup" -DiskName "MyDiskName"
$disk.Sku.Name       # This will now return Standard_LRS or Premium_LRS

$snapshot = Get-AzureRmSnapshot -ResourceGroupName "MyResourceGroup" -SnapshotName "MySnapshotName"
$snapshot.Sku.Name   # This will now return Standard_LRS or Premium_LRS
```

- A propriedade do tipo de conta de armazenamento aninhada nos tipos `PSVirtualMachine``PSVirtualMachineScaleSet` e `PSImage` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

```powershell
$vm = Get-AzureRmVM -ResourceGroupName "MyResourceGroup" -Name "MyVM"
$vm.StorageProfile.DataDisks[0].ManagedDisk.StorageAccountType   # This will now return Standard_LRS or Premium_LRS
```

**Add-AzureRmImageDataDisk**
- Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Add-AzureRmVMDataDisk**
- Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Add-AzureRmVmssDataDisk**
- Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**New-AzureRmAvailabilitySet**
- O parâmetro `Managed` foi removido em favor de `Sku`

```powershell
# Old
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Managed

# New
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Sku "Aligned"
```

**New-AzureRmDiskConfig**
- Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**New-AzureRmDiskUpdateConfig**
- Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**New-AzureRmSnapshotConfig**
- Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**New-AzureRmSnapshotUpdateConfig**
- Os valores aceites para o parâmetro `SkuName` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Set-AzureRmImageOsDisk**
- Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Set-AzureRmVMAEMExtension**
- O parâmetro `DisableWAD` foi removido
    -  O Diagnóstico do Azure do Windows está desativado por predefinição

**Set-AzureRmVMDataDisk**
- Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Set-AzureRmVMOSDisk**
- Os valores aceites para o parâmetro `StorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Set-AzureRmVmssStorageProfile**
- Os valores aceites para o parâmetro `ManagedDisk` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

**Update-AzureRmVmss**
- Os valores aceites para o parâmetro `ManagedDiskStorageAccountType` mudaram de `StandardLRS` e `PremiumLRS` para `Standard_LRS` e `Premium_LRS`, respetivamente

## <a name="breaking-changes-to-azurermdatalakestore-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.DataLakeStore

**Export-AzureRmDataLakeStoreItem**
- Os parâmetros `PerFileThreadCount` e `ConcurrentFileCount` foram removidos. Utilize o parâmetro `Concurrency` daqui para a frente

```powershell
# Old
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -Concurrency 160
```

**Import-AzureRmDataLakeStoreItem**
- Os parâmetros `PerFileThreadCount` e `ConcurrentFileCount` foram removidos. Utilize o parâmetro `Concurrency` daqui para a frente

```powershell
# Old
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -Concurrency 160
```

**Remove-AzureRmDataLakeStoreItem**
- O parâmetro `Clean` foi removido

```powershell
# Old
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse -Clean

# New
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse
```

## <a name="breaking-changes-to-azurermdns-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.Dns

**New-AzureRmDnsRecordSet**
- O parâmetro `Force` foi removido

**Remove-AzureRmDnsRecordSet**
- O parâmetro `Force` foi removido

**Remove-AzureRmDnsZone**
- O parâmetro `Force` foi removido

## <a name="breaking-changes-to-azurerminsights-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.Insights

**Add-AzureRmAutoscaleSetting**
- Os aliases de parâmetro `AutoscaleProfiles` e `Notifications` foram removidos

**Add-AzureRmLogProfile**
- Os aliases de parâmetro `Categories` e `Locations` foram removidos

**Add-AzureRmMetricAlertRule**
- Os aliases de parâmetro `Actions` foram removidos

**Add-AzureRmWebtestAlertRule**
- Os aliases de parâmetro `Actions` foram removidos

**Get-AzureRmLog**
- Os aliases de parâmetro `MaxRecords` e `MaxEvents` foram removidos

**Get-AzureRmMetricDefinition**
- Os aliases de parâmetro `MetricNames` foram removidos

**New-AzureRmAlertRuleEmail**
- Os aliases de parâmetro `CustomEmails` e `SendToServiceOwners` foram removidos

**New-AzureRmAlertRuleWebhook**
- Os aliases de parâmetro `Properties` foram removidos

**New-AzureRmAutoscaleNotification**
- Os aliases de parâmetro `CustomEmails`, `SendEmailToSubscriptionCoAdministrators` e `Webhooks` foram removidos

**New-AzureRmAutoscaleProfile**
- Os aliases de parâmetro `Rules`, `ScheduleDays` , `ScheduleHours` e `ScheduleMinutes`foram removidos

**New-AzureRmAutoscaleWebhook**
- Os aliases de parâmetro `Properties` foram removidos

## <a name="breaking-changes-to-azurermkeyvault-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.KeyVault

**Add-AzureKeyVaultCertificate**
- O parâmetro `Certificate` tornou-se obrigatório.

**Set-AzureKeyVaultManagedStorageSasDefinition**
- O cmdlet já não aceita parâmetros individuais que compõem o token de acesso; em vez disso, o cmdlet substitui parâmetros de token explícitos, como `Service` ou `Permissions`, com um parâmetro `TemplateUri` genérico correspondente a um token de acesso de exemplo definido noutro local (possivelmente através de cmdlets do PowerShell de Armazenamento ou composto manualmente de acordo com a documentação de Armazenamento.) O cmdlet mantém o parâmetro `ValidityPeriod`.

Para obter mais informações sobre a composição de tokens de acesso partilhado para o Armazenamento do Azure, veja as páginas de documentação, respetivamente:
- [Construir um Serviço SAS] (https://docs.microsoft.com/en-us/rest/api/storageservices/Constructing-a-Service-SAS)
- [Construir uma Conta SAS] (https://docs.microsoft.com/en-us/rest/api/storageservices/constructing-an-account-sas)

```powershell
# Old
$sas = Set-AzureKeyVaultManagedStorageSasDefinition -VaultName myVault -Name myKey -Service Blob -Permissions 'rcw' -ValidityPeriod 180d

# New
$sctx=New-AzureStorageContext -StorageAccountName $sa.StorageAccountName -Protocol Https -StorageAccountKey Key1
$start=[System.DateTime]::Now.AddDays(-1)
$end=[System.DateTime]::Now.AddMonths(1)
$at=New-AzureStorageAccountSasToken -Service blob -ResourceType Service,Container,Object -Permission "racwdlup" -Protocol HttpsOnly -StartTime $start -ExpiryTime $end -Context $sctx
$sas=Set-AzureKeyVaultManagedStorageSasDefinition -AccountName $sa.StorageAccountName -VaultName $kv.VaultName -Name accountsas -TemplateUri $at -SasType 'account' -ValidityPeriod ([System.Timespan]::FromDays(30))
```

**Set-AzureKeyVaultCertificateIssuer**
- O parâmetro `IssuerProvider` tornou-se obrigatório.

**Undo-AzureKeyVaultCertificateRemoval**
- O resultado deste cmdlet foi alterado de `CertificateBundle` para `PSKeyVaultCertificate`.

**Undo-AzureRmKeyVaultRemoval**
- `ResourceGroupName` foi removido do conjunto de parâmetros `InputObject` e, em vez disso, é obtido a partir da propriedade `InputObject` do parâmetro `ResourceId`.

**Set-AzureRmKeyVaultAccessPolicy**
- A permissão `all` foi removida de `PermissionsToKeys`, `PermissionsToSecrets` e `PermissionsToCertificates`.

**Geral**
- A propriedade `ValueFromPipelineByPropertyName` foi removida de todos os cmdlets onde a tubagem por `InputObject` foi ativada.  Os cmdlets afetados são:
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

- `ConfirmImpact` níveis foram removidos de todos os cmdlets.  Os cmdlets afetados são:
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

- O `IKeyVaultDataServiceClient` foi atualizado para todas as operações de Certificado devolverem PSTypes em vez de tipos de SDK. Isto inclui:
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

## <a name="breaking-changes-to-azurermnetwork-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.Network


**Add-AzureRmApplicationGatewayBackendHttpSettings**
- O parâmetro `ProbeEnabled` foi removido

**Add-AzureRmVirtualNetworkPeering**
- Os aliases de parâmetro `AlloowGatewayTransit` foram removidos

**New-AzureRmApplicationGatewayBackendHttpSettings**
- O parâmetro `ProbeEnabled` foi removido

**Set-AzureRmApplicationGatewayBackendHttpSettings**
- O parâmetro `ProbeEnabled` foi removido

## <a name="breaking-changes-to-azurermrediscache-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.RedisCache

**New-AzureRmRedisCache**
- Os parâmetros `Subnet` e `VirtualNetwork` foram removidos em favor de `SubnetId`
- O parâmetro `RedisVersion` foi removido
- O parâmetro `MaxMemoryPolicy` foi removido em favor de `RedisConfiguration`

```powershell
# Old
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -MaxMemoryPolicy "allkeys-lru"

# New
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

**Set-AzureRmRedisCache**
- O parâmetro `MaxMemoryPolicy` foi removido em favor de `RedisConfiguration`

```powershell
# Old
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -MaxMemoryPolicy "allkeys-lru"

# New
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

## <a name="breaking-changes-to-azurermresources-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.Resources

**Find-AzureRmResource**
- Este cmdlet foi removido e a funcionalidade foi movida para `Get-AzureRmResource`

```powershell
# Old
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupNameContains "ResourceGroup"
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceNameContains "test"

# New
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupName "*ResourceGroup*"
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -Name "*test*"
```

**Find-AzureRmResourceGroup**
- Este cmdlet foi removido e a funcionalidade foi movida para `Get-AzureRmResourceGroup`

```powershell
# Old
Find-AzureRmResourceGroup
Find-AzureRmResourceGroup -Tag @{ "testtag" = $null }
Find-AzureRmResourceGroup -Tag @{ "testtag" = "testval" }

# New
Get-AzureRmResourceGroup
Get-AzureRmResourceGroup -Tag @{ "testtag" = $null }
Get-AzureRmResourceGroup -Tag @{ "testtag" = "testval" }
```

**Get-AzureRmRoleDefinition**
- O parâmetro `AtScopeAndBelow` foi removido.

```powershell

# Old
Get-AzureRmRoleDefinition [other required parameters] -AtScopeAndBelow

# New
Get-AzureRmRoleDefinition [other required parameters]
```

## <a name="breaking-changes-to-azurermstorage-cmdlets"></a>Alterações interruptivas aos cmdlets AzureRM.Storage

**New-AzureRmStorageAccount**
- O parâmetro `EnableEncryptionService` foi removido

**Set-AzureRmStorageAccount**
- Os parâmetros `EnableEncryptionService` e `DisableEncryptionService` foram removidos

## <a name="removed-modules"></a>Módulos removidos

### `AzureRM.ServerManagement`

O serviço de Ferramentas de Gestão do Servidor foi [extinto no ano passado](https://blogs.technet.microsoft.com/servermanagement/2017/05/17/smt-preview-service-is-being-retired-on-june-30-2017/) e, consequentemente, o módulo correspondente para SMT, `AzureRM.ServerManagement`, foi removido do `AzureRM` e deixará de ser enviado daqui para a frente.

### `AzureRM.SiteRecovery`

O módulo `AzureRM.SiteRecovery` está a ser substituído por `AzureRM.RecoveryServices.SiteRecovery`, que é um superconjunto funcional do módulo `AzureRM.SiteRecovery` e inclui um novo conjunto de cmdlets equivalentes. Pode encontrar a lista completa de mapeamentos dos cmdlets antigos para os novos abaixo:

| Cmdlet preterido                                        | Cmdlet equivalente                                                | Aliases                                  |
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