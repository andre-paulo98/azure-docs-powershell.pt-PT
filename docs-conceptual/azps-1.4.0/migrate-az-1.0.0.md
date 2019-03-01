---
title: Alterações interruptivas do Microsoft Azure PowerShell Az 1.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 1.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/14/2018
ms.openlocfilehash: be3e19dc4b689adbc63b933dd9f3454122d5344a
ms.sourcegitcommit: 5630030c5cfa9828c3c024b69de59248263ef17f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/26/2019
ms.locfileid: "56837372"
---
# <a name="migration-guide-for-az-100"></a>Guia de migração para o Az 1.0.0

Este documento descreve as alterações realizadas entre as versões de 6.x do AzureRM e a versão do Az 1.0.0.

## <a name="table-of-contents"></a>Índice
- [Alterações interruptivas gerais](#general-breaking-changes)
  - [Alterações do Prefixo de Nomes de Cmdlet](#cmdlet-noun-prefix-changes)
  - [Alterações de Nomes de Módulos](#module-name-changes)
  - [Módulos removidos](#removed-modules)
  - [Windows PowerShell 5.1 e .NET 4.7.2](#windows-powershell-51-and-net-472)
  - [Remoção temporária do Início de sessão do utilizador através de PSCredential](#temporary-removal-of-user-login-using-pscredential)
  - [Início de sessão com o Código de Dispositivo Predefinido em vez da linha de comandos do Browser](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [Alterações interruptivas do módulo](#module-breaking-changes)
  - [Az.ApiManagement (anteriormente AzureRM.ApiManagement)](#azapimanagement-previously-azurermapimanagement)
  - [Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)](#azcognitiveservices-previously-azurermcognitiveservices)
  - [Az.Compute (anteriormente AzureRM.Compute)](#azcompute-previously-azurermcompute)
  - [Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)](#azdatalakestore-previously-azurermdatalakestore)
  - [Az.KeyVault (anteriormente AzureRM.KeyVault)](#azkeyvault-previously-azurermkeyvault)
  - [Az.Media (anteriormente AzureRM.Media)](#azmedia-previously-azurermmedia)
  - [Az.Monitor (anteriormente AzureRM.Insights)](#azmonitor-previously-azurerminsights)
  - [Az.Network (anteriormente AzureRM.Network)](#aznetwork-previously-azurermnetwork)
  - [Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)](#azoperationalinsights-previously-azurermoperationalinsights)
  - [Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [Az.Resources (anteriormente AzureRM.Resources)](#azresources-previously-azurermresources)
  - [Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)](#azservicefabric-previously-azurermservicefabric)
  - [Az.Sql (anteriormente AzureRM.Sql)](#azsql-previously-azurermsql)
  - [Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)](#azstorage-previously-azurestorage-and-azurermstorage)
  - [Az.Websites (anteriormente AzureRM.Websites)](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a>Alterações interruptivas gerais
### <a name="cmdlet-noun-prefix-changes"></a>Alterações do Prefixo de Nomes de Cmdlet
No AzureRM, os cmdlets utilizavam "AzureRM" ou "Azure" como prefixo de nome.  O Az simplifica e normaliza os nomes de cmdlet, para que todos os cmdlets utilizem "Az" como prefixo de nomes de cmdlet. Por exemplo:
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

Foi alterado para
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

Para simplificar a transição para estes novos nomes de cmdlet, o Az apresenta dois novos cmdlets: ```Enable-AzureRmAlias``` e ```Disable-AzureRmAlias```.  ```Enable-AzureRmAlias``` cria aliases a partir dos nomes de cmdlet mais antigos no AzureRM e transforma-os em nomes de cmdlet do Az mais recentes.  O cmdlet permite criar aliases na sessão atual, ou em todas as sessões, ao alterar o seu perfil de utilizador ou de computador. 

Por exemplo, o seguinte script no AzureRM:
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Pode ser executado com alterações mínimas com ```Enable-AzureRmAlias```:
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

A utilização de ```Enable-AzureRmAlias -Scope CurrentUser``` permite empregar os aliases em todas as sessões do Powershell que forem abertas, para que, após a execução deste cmdlet, não seja necessário alterar um script deste tipo:
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Para obter detalhes completos sobre a utilização de cmdlets do alias, execute ```Get-Help -Online Enable-AzureRmAlias``` a partir da linha de comandos do Powershell.

```Disable-AzureRmAlias``` remove os aliases de cmdlet do AzureRM criados por ```Enable-AzureRmAlias```.  Para obter detalhes completos, execute ```Get-Help -Online Disable-AzureRmAlias``` a partir da linha de comandos do Powershell.

### <a name="module-name-changes"></a>Alterações de Nomes de Módulos
- Os nomes de módulos foram alterados de `AzureRM.*` para `Az.*`, exceto para os seguintes módulos:
```
AzureRM.Profile                       -> Az.Accounts
Azure.AnalysisServices                -> Az.AnalysisServices
AzureRM.Consumption                   -> Az.Billing
AzureRM.UsageAggregates               -> Az.Billing
AzureRM.DataFactories                 -> Az.DataFactory
AzureRM.DataFactoryV2                 -> Az.DataFactory
AzureRM.MachineLearningCompute        -> Az.MachineLearning
AzureRM.Insights                      -> Az.Monitor
AzureRM.RecoveryServices.Backup       -> Az.RecoveryServices
AzureRM.RecoveryServices.SiteRecovery -> Az.RecoveryServices
AzureRM.Tags                          -> Az.Resources
Azure.Storage                         -> Az.Storage
```

As alterações realizadas ao nível dos nomes de módulos significam que qualquer script que utilizar ```#Requires``` ou ```Import-Module``` para carregar módulos específicos terá de ser alterado de modo a utilizar o novo módulo.

#### <a name="migrating-requires-statements"></a>Migrar Declarações #Requires
Os scripts que utilizam #Requires para declarar uma dependência nos módulos do AzureRM devem ser atualizados de modo a utilizarem os novos nomes de módulos
```powershell
#Requires -Module AzureRM.Compute
```

Devem ser alterados para
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a>Migrar Declarações Import-Module
Os scripts que utilizam ```Import-Module``` para carregar módulos do AzureRM têm de ser atualizados de modo a refletirem os novos nomes de módulos.
```powershell
Import-Module -Name AzureRM.Compute
```

Devem ser alterados para
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a>Migrar Invocações de Cmdlets Completamente Qualificados
Os scripts que utilizam invocações de cmdlets qualificados por módulo, como
```powershell
AzureRM.Compute\Get-AzureRmVM
```

Devem ser alterados de modo a utilizarem os novos nomes de módulos e cmdlets
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a>Migrar Dependências de Manifestos de Módulos
Os módulos que expressam dependências nos módulos do AzureRM através de um ficheiro (.psd1) de manifesto de módulo terão de atualizar os nomes de módulos na respetiva secção "RequiredModules"

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

Devem ser alterados para

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a>Módulos removidos
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

As ferramentas para estes serviços já não são suportadas ativamente.  Os clientes são incentivados a mudar para serviços alternativos assim que for possível.

### <a name="windows-powershell-51-and-net-472"></a>Windows PowerShell 5.1 e .NET 4.7.2
- Para utilizar o Az com o Windows PowerShell 5.1, tem de instalar o .NET 4.7.2. No entanto, para utilizar o Az com o PowerShell Core não é preciso o .NET 4.7.2. 

### <a name="temporary-removal-of-user-login-using-pscredential"></a>Remoção temporária do Início de sessão do utilizador através de PSCredential
- Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a remover temporariamente o início de sessão do utilizador através de PSCredential. Esta capacidade será introduzida novamente na versão de 15/01/2019 para o Windows PowerShell 5.1. Este assunto é abordado em detalhe [neste debate sobre o problema](https://github.com/Azure/azure-powershell/issues/7430).

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a>Início de sessão com o Código de Dispositivo Predefinido em vez da linha de comandos do Browser
- Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a utilizar o início de sessão de dispositivo como o fluxo de início de sessão predefinido durante o início de sessão interativo. O início de sessão baseado no browser será introduzido novamente para o Windows PowerShell 5.1 como a predefinição na versão de 15/01/2019. Nessa altura, os utilizadores poderão escolher o início de sessão de dispositivo através de um parâmetro de mudança (Switch).

## <a name="module-breaking-changes"></a>Alterações interruptivas do módulo

### <a name="azapimanagement-previously-azurermapimanagement"></a>Az.ApiManagement (anteriormente AzureRM.ApiManagement)
- Os cmdlets que se seguem vão ser removidos:
  - New-AzureRmApiManagementHostnameConfiguration
  - Set-AzureRmApiManagementHostnames
  - Update-AzureRmApiManagementDeployment
  - Import-AzureRmApiManagementHostnameCertificate
  - Em alternativa, utilize o cmdlet **Set-AzApiManagement** para definir estas propriedades
- As propriedades que se seguem foram removidas
  - As propriedades `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` e `ScmHostnameConfiguration` do tipo `PsApiManagementHostnameConfiguration` foram removidas de `PsApiManagementContext`. Em vez disso, utilize `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` e `ScmCustomHostnameConfiguration` do tipo `PsApiManagementCustomHostNameConfiguration`.
  - A propriedade `StaticIPs` foi removida de PsApiManagementContext. A propriedade foi dividida em `PublicIPAddresses` e `PrivateIPAddresses`.
  - A propriedade necessária `Location` foi removida do cmdlet New-AzureApiManagementVirtualNetwork.

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a>Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)
- O parâmetro `InvoiceName` foi removido do cmdlet `Get-AzConsumptionUsageDetail`.  Os scripts terão de utilizar outros parâmetros de identidade para a faturação.

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a>Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)
- O conjunto de parâmetros `GetSkusWithAccountParamSetName` foi removido do cmdlet `Get-AzCognitiveServicesAccountSkus`.  Tem de obter os Skus através do Tipo de Conta e da Localização, em vez de utilizar ResourceGroupName e o Nome da Conta.

### <a name="azcompute-previously-azurermcompute"></a>Az.Compute (anteriormente AzureRM.Compute)
- Os `IdentityIds` foram removidos da propriedade `Identity` nos objetos `PSVirtualMachine` e `PSVirtualMachineScaleSet`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.
- O tipo de propriedade `InstanceView` do objeto `PSVirtualMachineScaleSetVM` foi alterado de `VirtualMachineInstanceView` para `VirtualMachineScaleSetVMInstanceView`
- As propriedades `AutoOSUpgradePolicy` e `AutomaticOSUpgrade` foram removidas da propriedade `UpgradePolicy`
- O tipo de propriedade `Sku` no objeto `PSSnapshotUpdate` foi alterado de `DiskSku` para `SnapshotSku`
- `VmScaleSetVMParameterSet` foi removido do cmdlet `Add-AzVMDataDisk`. Já não pode adicionar um disco de dados individualmente a uma VM de conjunto de dimensionamento (ScaleSet).

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a>Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)
- O parâmetro `GatewayName` tornou-se obrigatório no cmdlet `New-AzDataFactoryEncryptValue`
- O cmdlet `New-AzDataFactoryGatewayKey` foi removido
- O parâmetro `LinkedServiceName` foi removido do cmdlet `Get-AzDataFactoryV2ActivityRun`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a>Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)
- Os cmdlets preteridos que se seguem foram removidos: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret` e `Set-AzDataLakeAnalyticsCatalogSecret`

### <a name="azdatalakestore-previously-azurermdatalakestore"></a>Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)
- O tipo do parâmetro `Encoding` foi alterado de `FileSystemCmdletProviderEncoding` para `System.Text.Encoding` nos cmdlets que se seguem. Esta alteração remove os valores de codificação `String` e `Oem`. Todos os outros valores de codificação anteriores permanecem.
  - New-AzureRmDataLakeStoreItem
  - Add-AzureRmDataLakeStoreItemContent
  - Get-AzureRmDataLakeStoreItemContent
- O alias de propriedade preterido `Tags` foi removido dos cmdlets `New-AzDataLakeStoreAccount` e `Set-AzDataLakeStoreAccount`

  Os scripts que utilizam
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  Devem ser alterados para
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- As propriedades preteridas ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier``` e ```FirewallAllowAzureIps``` foram removidas do objeto ```PSDataLakeStoreAccountBasic```.  Qualquer script que utilize ```PSDatalakeStoreAccount``` devolvido a partir de ```Get-AzDataLakeStoreAccount``` não deve fazer referência a essas propriedades.

### <a name="azkeyvault-previously-azurermkeyvault"></a>Az.KeyVault (anteriormente AzureRM.KeyVault)
- A propriedade `PurgeDisabled` foi removida dos objetos `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` e `PSKeyVaultSecretAttributes`. Os scripts devem deixar de fazer referência à propriedade ```PurgeDisabled``` para tomar decisões de processamento.

### <a name="azmedia-previously-azurermmedia"></a>Az.Media (anteriormente AzureRM.Media)
- O alias de propriedade preterido `Tags` foi removido do cmdlet `New-AzMediaService`. Os scripts que utilizam
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  Devem ser alterados para
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a>Az.Monitor (anteriormente AzureRM.Insights)
- Os nomes de parâmetros no plural `Categories` e `Timegrains` foram removidos em prol de nomes de parâmetros no singular do cmdlet `Set-AzDiagnosticSetting`. Os scripts que utilizam
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  Devem ser alterados para
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a>Az.Network (anteriormente AzureRM.Network)
- O parâmetro preterido `ResourceId` foi removido do cmdlet `Get-AzServiceEndpointPolicyDefinition`
- A propriedade preterida `EnableVmProtection` foi removida do objeto `PSVirtualNetwork`
- O cmdlet preterido `Set-AzVirtualNetworkGatewayVpnClientConfig` foi removido
  
Os scripts devem deixar de tomar decisões de processamento com base nos valores destes campos.

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a>Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)
- O conjunto de parâmetros predefinido para `Get-AzOperationalInsightsDataSource` foi removido e `ByWorkspaceNameByKind` passou a ser o conjunto de parâmetros predefinido

  Os scripts que listavam origens de dados com
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  Devem ser alterados para especificar um tipo (Kind)
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a>Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)
- O parâmetro `Encryption` foi removido do cmdlet `New/Set-AzRecoveryServicesAsrPolicy`
- Agora, o parâmetro `TargetStorageAccountName` é obrigatório para os restauros de discos geridos no cmdlet `Restore-AzRecoveryServicesBackupItem`
- Os parâmetros `StorageAccountName` e `StorageAccountResourceGroupName` foram removidos no cmdlet `Restore-AzRecoveryServicesBackupItem`
- O parâmetro `Name` foi removido no cmdlet `Get-AzRecoveryServicesBackupContainer`

### <a name="azresources-previously-azurermresources"></a>Az.Resources (anteriormente AzureRM.Resources)
- O parâmetro `Sku` foi removido do cmdlet `New/Set-AzPolicyAssignment`
- O parâmetro `Password` foi removido dos cmdlets `New-AzADServicePrincipal` e `New-AzADSpCredential`. As palavras-passe são geradas automaticamente e o scripts que forneciam a palavra-passe:
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  Devem ser alterados de modo a obterem a palavra-passe a partir da saída:
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a>Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)
- Foram alterados os seguintes tipos de retorno de cmdlet:
  - A propriedade `SerivceTypeHealthPolicies` do tipo `ApplicationHealthPolicy` foi removida.
  - A propriedade `ApplicationHealthPolicies` do tipo `ClusterUpgradeDeltaHealthPolicy` foi removida.
  - A propriedade `OverrideUserUpgradePolicy` do tipo `ClusterUpgradePolicy` foi removida.
  - Estas alterações afetam os seguintes cmdlets:
    - Add-AzServiceFabricClientCertificate
    - Add-AzServiceFabricClusterCertificate
    - Add-AzServiceFabricNode
    - Add-AzServiceFabricNodeType
    - Get-AzServiceFabricCluster
    - Remove-AzServiceFabricClientCertificate
    - Remove-AzServiceFabricClusterCertificate
    - Remove-AzServiceFabricNode
    - Remove-AzServiceFabricNodeType
    - Remove-AzServiceFabricSetting
    - Set-AzServiceFabricSetting
    - Set-AzServiceFabricUpgradeType
    - Update-AzServiceFabricDurability
    - Update-AzServiceFabricReliability

### <a name="azsql-previously-azurermsql"></a>Az.Sql (anteriormente AzureRM.Sql)
- Os parâmetros `State` e `ResourceId` foram removidos do cmdlet `Set-AzSqlDatabaseBackupLongTermRetentionPolicy`
- Foram removidos os seguintes cmdlets preteridos: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing` e `Remove-AzSqlServerAuditing`
- O parâmetro preterido `Current` foi removido do cmdlet `Get-AzSqlDatabaseBackupLongTermRetentionPolicy`
- O parâmetro preterido `DatabaseName` foi removido do cmdlet `Get-AzSqlServerServiceObjective`
- O parâmetro preterido `PrivilegedLogin` foi removido do cmdlet `Set-AzSqlDatabaseDataMaskingPolicy`

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a>Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)
- Para suportar a criação de um contexto de armazenamento de Oauth com apenas o nome da conta de armazenamento, o conjunto de parâmetros predefinido foi alterado para `OAuthParameterSet`
  - Exemplo: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`
- O parâmetro `Location` tornou-se obrigatório no cmdlet `Get-AzStorageUsage`
- Os métodos da API de Armazenamento utilizam agora o Padrão Assíncrono Baseado em Tarefas (TAP), em vez de chamadas síncronas à API.
#### <a name="1-blob-snapshot"></a>1. Instantâneo do Blob
##### <a name="before"></a>Antes:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a>Depois:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a>2. Instantâneo da Partilha
##### <a name="before"></a>Antes:
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a>Depois:
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a>3. Anular a eliminação de um blob de eliminação de forma recuperável
##### <a name="before"></a>Antes:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a>Depois:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a>4. Definir Camada de Blob
##### <a name="before"></a>Antes:
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a>Depois:
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a>Az.Websites (anteriormente AzureRM.Websites)
- As propriedades preteridas foram removidas dos objetos `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` e `PSSite`