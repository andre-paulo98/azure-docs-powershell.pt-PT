---
title: Todas as alterações do AzureRM para o Azure PowerShell Az 1.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 1.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2019
ms.openlocfilehash: 1d99f04525a33f03f859bfb4abe263b12ca6add9
ms.sourcegitcommit: 492e21ce65bd5782c65171ff93522c6366818060
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "66814385"
---
# <a name="breaking-changes-for-az-100"></a>Alterações interruptivas do Az 1.0.0

Este documento fornece informações detalhadas sobre as alterações entre o AzureRM 6.x e o novo módulo do Az, versão 1.x e posterior. O índice irá guiá-lo através de um caminho de migração completo, incluindo alterações específicas do módulo que podem afetar os scripts.

Para obter orientação geral sobre como começar uma migração do AzureRM para o Az, veja [Iniciar a migração do AzureRM para o Az](migrate-from-azurerm-to-az.md).

> [!IMPORTANT]
> Também têm sido feitas alterações interruptivas entre o Az 1.0.0 e o Az 2.0.0. Depois de seguir este guia para atualizar do AzureRM para o Az, veja as [alterações interruptivas do Az 2.0.0](migrate-az-2.0.0.md) para saber se tem de fazer alterações adicionais.

## <a name="table-of-contents"></a>Índice

- [Alterações interruptivas gerais](#general-breaking-changes)
  - [Alterações dos prefixo de nomes de cmdlets](#cmdlet-noun-prefix-changes)
  - [Alterações de Nomes de Módulos](#module-name-changes)
  - [Módulos removidos](#removed-modules)
  - [Windows PowerShell 5.1 e .NET 4.7.2](#windows-powershell-51-and-net-472)
  - [Remoção temporária do início de sessão do utilizador através de PSCredential](#temporary-removal-of-user-login-using-pscredential)
  - [Início de sessão com o código de dispositivo predefinido em vez da linha de comandos do browser](#default-device-code-login-instead-of-web-browser-prompt)
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

Esta secção fornece detalhes sobre as alterações interruptivas gerais que fazem parte do novo design do módulo do Az.

### <a name="cmdlet-noun-prefix-changes"></a>Alterações do Prefixo de Nomes de Cmdlet

No módulo do AzureRM, os cmdlets utilizavam `AzureRM` ou `Azure` como prefixo de nome.  O Az simplifica e normaliza os nomes de cmdlets, para que todos os cmdlets utilizem "Az" como prefixo de nome de cmdlet. Por exemplo:

```azurepowershell-interactive
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

Foi alterado para:

```azurepowershell-interactive
Get-AzVM
Get-AzKeyVaultSecret
```

Para simplificar a transição para estes novos nomes de cmdlets, o Az apresenta dois novos cmdlets, [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) e [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).  `Enable-AzureRmAlias` cria aliases para os nomes de cmdlets mais antigos no AzureRM que os mapeia para os nomes de cmdlets do Az mais recentes. A utilização do argumento `-Scope` com `Enable-AzureRmAlias` permite-lhe escolher onde os aliases estão ativados.

Por exemplo, o seguinte script no AzureRM:

```azurepowershell-interactive
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Pode ser executado com alterações mínimas com `Enable-AzureRmAlias`:

```azurepowershell-interactive
#Requires -Modules Az.Storage
Enable-AzureRmAlias -Scope Process
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

A utilização de `Enable-AzureRmAlias -Scope CurrentUser` permite atualizar os aliases em todas as sessões do PowerShell que forem abertas, para que, após a execução deste cmdlet, não seja necessário alterar um script deste tipo:

```azurepowershell-interactive
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Para obter detalhes completos sobre a utilização de cmdlets de aliases,veja a [referência Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias).

Quando estiver pronto para desativar aliases, `Disable-AzureRmAlias` remove os aliases criados. Para obter detalhes completos, veja a [referência Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).

> [!IMPORTANT]
> Quando desativar aliases, certifique-se de que estão desativados para _todos_ os âmbitos que tiveram aliases ativados.

### <a name="module-name-changes"></a>Alterações de Nomes de Módulos

Os nomes de módulos foram alterados de `AzureRM.*` para `Az.*`, exceto para os seguintes módulos:

| Módulo do AzureRM | Módulo do Az |
|----------------|-----------|
| Azure.Storage | Az.Storage |
| Azure.AnalysisServices | Az.AnalysisServices |
| AzureRM.Profile | Az.Accounts |
| AzureRM.Insights | Az.Monitor |
| AzureRM.DataFactories | Az.DataFactory |
| AzureRM.DataFactoryV2 | Az.DataFactory |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices |
| AzureRM.Tags | Az.Resources |
| AzureRM.MachineLearningCompute | Az.MachineLearning |
| AzureRM.UsageAggregates | Az.Billing |
| AzureRM.Consumption | Az.Billing |

As alterações realizadas ao nível dos nomes de módulos significam que qualquer script que utilizar `#Requires` ou `Import-Module` para carregar módulos específicos terá de ser alterado de modo a utilizar o novo módulo. Para os módulos em que o sufixo de cmdlet não foi alterado, embora o nome do módulo tenha sido alterado, o sufixo que indica o espaço da operação _não foi alterado_.

#### <a name="migrating-requires-and-import-module-statements"></a>Migrar Declarações #Requires e Import-Module

Os scripts que utilizam `#Requires` ou `Import-Module` para declarar uma dependência nos módulos do AzureRM devem ser atualizados de modo a utilizarem os novos nomes de módulos. Por exemplo:

```azurepowershell-interactive
#Requires -Module AzureRM.Compute
```

Deve ser alterado para:

```azurepowershell-interactive
#Requires -Module Az.Compute
```

Para `Import-Module`:

```azurepowershell-interactive
Import-Module -Name AzureRM.Compute
```

Deve ser alterado para:

```azurepowershell-interactive
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a>Migrar Invocações de Cmdlets Completamente Qualificados

Os scripts que utilizam invocações de cmdlets qualificados por módulo, como:

```azurepowershell-interactive
AzureRM.Compute\Get-AzureRmVM
```

Têm de ser alterados de modo a utilizarem os novos nomes de módulos e cmdlets:

```azurepowershell-interactive
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a>Migrar dependências de manifestos de módulos

Os módulos que expressam dependências nos módulos do AzureRM através de um ficheiro (.psd1) de manifesto de módulo terão de atualizar os nomes de módulos na respetiva secção `RequiredModules`:

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

Tem de ser alterado para:

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a>Módulos removidos

Os módulos seguintes foram removidos:

- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

As ferramentas para estes serviços já não são suportadas ativamente.  Os clientes são incentivados a mudar para serviços alternativos assim que for possível.

### <a name="windows-powershell-51-and-net-472"></a>Windows PowerShell 5.1 e .NET 4.7.2

Para utilizar o Az com o PowerShell 5.1 para Windows, tem de instalar o .NET Framework 4.7.2. A utilização do PowerShell Core 6.x ou posterior não requer o .NET Framework.

### <a name="temporary-removal-of-user-login-using-pscredential"></a>Remoção temporária do Início de sessão do utilizador através de PSCredential

Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a remover temporariamente o início de sessão do utilizador através de PSCredential. Esta capacidade será introduzida novamente na versão de 15/01/2019 para o PowerShell 5.1 para Windows. Este assunto é abordado em detalhe [neste debate sobre o problema no GitHub](https://github.com/Azure/azure-powershell/issues/7430).

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a>Início de sessão com o código de dispositivo predefinido em vez da linha de comandos do browser

Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a utilizar o início de sessão de dispositivo como o fluxo de início de sessão predefinido durante o início de sessão interativo. O início de sessão baseado no browser será introduzido novamente para o PowerShell 5.1 para Windows como a predefinição na versão de 15/01/2019. Nessa altura, os utilizadores poderão escolher o início de sessão de dispositivo através de um parâmetro de mudança (Switch).

## <a name="module-breaking-changes"></a>Alterações interruptivas do módulo

Esta secção fornece detalhes sobre alterações interruptivas específicas para cmdlets e módulos individuais.

### <a name="azapimanagement-previously-azurermapimanagement"></a>Az.ApiManagement (anteriormente AzureRM.ApiManagement)

- Foram removidos os seguintes cmdlets:
  - New-AzureRmApiManagementHostnameConfiguration
  - Set-AzureRmApiManagementHostnames
  - Update-AzureRmApiManagementDeployment
  - Import-AzureRmApiManagementHostnameCertificate
  - Em alternativa, utilize o cmdlet **Set-AzApiManagement** para definir estas propriedades
- Foram removidas as seguintes propriedades:
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
  ```azurepowershell-interactive
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  Devem ser alterados para
  ```azurepowershell-interactive
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- As propriedades preteridas `Identity`, `EncryptionState`, `EncryptionProvisioningState`, `EncryptionConfig`, `FirewallState`, `FirewallRules`, `VirtualNetworkRules`, `TrustedIdProviderState`, `TrustedIdProviders`, `DefaultGroup`, `NewTier`, `CurrentTier` e `FirewallAllowAzureIps` foram removidas do objeto `PSDataLakeStoreAccountBasic`.  Qualquer script que utilize `PSDatalakeStoreAccount` devolvido a partir de `Get-AzDataLakeStoreAccount` não deve fazer referência a essas propriedades.

### <a name="azkeyvault-previously-azurermkeyvault"></a>Az.KeyVault (anteriormente AzureRM.KeyVault)

- A propriedade `PurgeDisabled` foi removida dos objetos `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` e `PSKeyVaultSecretAttributes`. Os scripts devem deixar de fazer referência à propriedade ```PurgeDisabled``` para tomar decisões de processamento.

### <a name="azmedia-previously-azurermmedia"></a>Az.Media (anteriormente AzureRM.Media)

- O alias de propriedade preterido `Tags` foi removido do cmdlet `New-AzMediaService`. Os scripts que utilizam
  ```azurepowershell-interactive
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  Devem ser alterados para
  ```azurepowershell-interactive
  New-AzMediaService -Tag @{TagName="TagValue"}
  ```

### <a name="azmonitor-previously-azurerminsights"></a>Az.Monitor (anteriormente AzureRM.Insights)

- Os nomes de parâmetros no plural `Categories` e `Timegrains` foram removidos em prol de nomes de parâmetros no singular do cmdlet `Set-AzDiagnosticSetting`. Os scripts que utilizam
  ```azurepowershell-interactive
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  Devem ser alterados para
  ```azurepowershell-interactive
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
  ```azurepowershell-interactive
  Get-AzureRmOperationalInsightsDataSource
  ```

  Devem ser alterados para especificar um tipo (Kind)
  ```azurepowershell-interactive
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

  ```azurepowershell-interactive
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  Devem ser alterados de modo a obterem a palavra-passe a partir da saída:

  ```azurepowershell-interactive
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a>Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)

- Foram alterados os seguintes tipos de retorno de cmdlet:
  - A propriedade `ServiceTypeHealthPolicies` do tipo `ApplicationHealthPolicy` foi removida.
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
- Os métodos da API de Armazenamento utilizam agora o Padrão Assíncrono Baseado em Tarefas (TAP), em vez de chamadas síncronas à API. Os exemplos seguintes demonstram os novos comandos assíncronos:

#### <a name="blob-snapshot"></a>Instantâneo do Blob

AzureRM:

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

Az:

```azurepowershell-interactive
$b = Get-AzStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="share-snapshot"></a>Instantâneo da Partilha

AzureRM:

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```

Az:

```azurepowershell-interactive
$Share = Get-AzStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="undelete-soft-deleted-blob"></a>Anular eliminação do blob eliminado de forma recuperável

AzureRM:

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```

Az:

```azurepowershell-interactive
$b = Get-AzStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="set-blob-tier"></a>Definir Camada de Blob

AzureRM:

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

Az:

```azurepowershell-interactive
$blockBlob = Get-AzStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a>Az.Websites (anteriormente AzureRM.Websites)

- As propriedades preteridas foram removidas dos objetos `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` e `PSSite`
