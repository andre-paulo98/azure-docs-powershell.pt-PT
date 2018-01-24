# <a name="breaking-changes-for-microsoft-azure-powershell-400"></a>Alterações recentes ao Microsoft Azure PowerShell 4.0.0

Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell. Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço. Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.

## <a name="table-of-contents"></a>Índice

- [Alterações recentes aos cmdlets de Computação](#breaking-changes-to-compute-cmdlets)
- [Alterações recentes aos cmdlets de EventHub](#breaking-changes-to-eventhub-cmdlets)
- [Alterações recentes aos cmdlets de Insights](#breaking-changes-to-insights-cmdlets)
- [Alterações recentes aos cmdlets de Rede](#breaking-changes-to-network-cmdlets)
- [Alterações recentes aos cmdlets de ServiceBus](#breaking-changes-to-servicebus-cmdlets)
- [Alterações recentes aos cmdlets de SQL](#breaking-changes-to-sql-cmdlets)
- [Alterações recentes aos cmdlets de Armazenamento](#breaking-changes-to-storage-cmdlets)
- [Alterações recentes aos cmdlets de Perfil](#breaking-changes-to-profile-cmdlets)
## <a name="breaking-changes-to-compute-cmdlets"></a>Alterações recentes aos cmdlets de Computação

Os seguintes tipos de saída foram afetados nesta versão:

### <a name="psvirtualmachine"></a>PSVirtualMachine
- As propriedades de nível superior `DataDiskNames` e `NetworkInterfaceIDs` do objeto `PSVirtualMachine` foram removidas do tipo de saída. Estas propriedades têm estado sempre disponíveis nas propriedades `StorageProfile` e `NetworkProfile` do objeto `PSVirtualMachine` e esta é a forma como terão de ser acedidas daqui em diante.
- Esta alteração afeta os seguintes cmdlets:
    - `Add-AzureRmVMDataDisk`
    - `Add-AzureRmVMNetworkInterface`
    - `Get-AzureRmVM`
    - `Remove-AzureRmVMDataDisk`
    - `Remove-AzureRmVMNetworkInterface`
    - `Set-AzureRmVMDataDisk`

```powershell
# Old
$vm.DataDiskNames
$vm.NetworkInterfaceIDs

# New
$vm.StorageProfile.DataDisks | Select -Property Name
$vm.NetworkProfile.NetworkInterfaces | Select -Property Id
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a>Alterações recentes aos cmdlets de EventHub

Os seguintes cmdlets foram afetados nesta versão:

### <a name="get-azurermeventhubnamespace"></a>Get-AzureRmEventHubNamespace
- A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`

### <a name="new-azurermeventhubnamespace"></a>New-AzureRmEventHubNamespace
- A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`

## <a name="breaking-changes-to-insights-cmdlets"></a>Alterações recentes aos cmdlets de Insights

Os seguintes cmdlets foram afetados nesta versão:
    
### <a name="get-azurermusage"></a>Get-AzureRmUsage
- Este cmdlet foi preterido.

### <a name="remove-azurermalertrule"></a>Remove-AzureRmAlertRule
- A saída deste cmdlet foi alterada de uma lista com um único objeto para um objeto único; este objeto inclui o requestId e o código de estado.
    
```powershell
# Old  
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name chiricutin
if ($s1 -ne $null)
{
    $r = $s1(0).RequestId
    $s = $s1(0).StatusCode
}

# New
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name chiricutin
$r = $s1.RequestId
$s = $s1.StatusCode
```
    
### <a name="add-azurermlogalertrule"></a>Add-AzureRmLogAlertRule
- Este cmdlet foi preterido.
    
### <a name="get-azurermalertrule"></a>Get-AzureRmAlertRule
- Cada elemento da saída (uma lista de objetos) deste cmdlet foi simplificado, ou seja, em vez de devolver objetos com a estrutura `{ Id, Location, Name, Tags, Properties }`, devolverá objetos com a estrutura `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, o que corresponde a todos os atributos de um Recurso do Azure juntamente com todos os atributos de um AlertRuleResource no nível superior.
    
```powershell
# Old
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -fore red "Error updating alert rule"
      
    Write-Host $rules(0).Id
    Write-Host $rules(0).Properties.IsEnabled
    Write-Host $rules(0).Properties.Condition
}

# New
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -fore red "Error updating alert rule"
 
    Write-Host $rules(0).Id
      
    # Properties will remain for a while
    Write-Host $rules(0).Properties.IsEnabled
      
    # But the properties will be at the top level too. Later Properties will be removed
    Write-Host $rules(0).IsEnabled
    Write-Host $rules(0).Condition
}
```
    
### <a name="get-azurermautoscalesetting"></a>Get-AzureRmAutoscaleSetting
- O campo `AutoscaleSettingResourceName` foi preterido porque tem sempre o mesmo valor que o campo `Name`.

```powershell
# Old  
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
if ($s1.AutoscaleSettingResourceName -ne $s1.Name)
{
    Write-Host "There is something wrong with the name"
}

# New
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
    
# There won't be a AutoscaleSettingResourceName
Write-Host $s1.Name
```
    
### <a name="remove-azurermlogprofile"></a>Remove-AzureRmLogProfile
- A saída deste cmdlet irá ser alterada de `Boolean` para um objeto que contém `RequestId` e `StatusCode`

```powershell
# Old  
$s1 = Remove-AzureRmLogProfile -Name myLogProfile
if ($s1 -eq $true)
{
    Write-Host "Removed"
}
else
{
    Write-Host "Failed"
}

# New
$s1 = Remove-AzureRmLogProfile -Name myLogProfile
$r = $s1.RequestId
$s = $s1.StatusCode
```
    
### <a name="add-azurermlogprofile"></a>Add-AzureRmLogProfile
- A saída deste cmdlet irá ser alterada de um objeto que inclui o requestId, o código de estado e o recurso atualizado ou recém-criado
    
```powershell
# Old  
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.ServiceBusRuleId

# New
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.RequestId
$s = $s1.StatusCode
$a = $s1.NewResource.ServiceBusRuleId
    
```
    
### <a name="set-azurermdiagnosticsettings"></a>Set-AzureRmDiagnosticSettings
- O nome do comando irá ser mudado para `Update-AzureRmDiagnsoticSettings`

```powershell
# Old
Set-AzureRmDiagnosticSettings

# New
Update-AzureRmDiagnosticSettings
```

## <a name="breaking-changes-to-network-cmdlets"></a>Alterações recentes aos cmdlets de Rede

Os seguintes cmdlets foram afetados nesta versão:

### <a name="new-azurermvirtualnetworkgatewayconnection"></a>New-AzureRmVirtualNetworkGatewayConnection
- O parâmetro `EnableBgp` foi alterado de modo a precisar de `boolean` em vez de `string`

```powershell
# Old
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp "true"

# New
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp $true
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a>Alterações recentes aos cmdlets de ServiceBus

Os seguintes cmdlets foram afetados nesta versão:

### <a name="get-azurermservicebusnamespace"></a>Get-AzureRmServiceBusNamespace
- A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`

### <a name="new-azurermservicebusnamespace"></a>New-AzureRmServiceBusNamespace

- A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`

## <a name="breaking-changes-to-sql-cmdlets"></a>Alterações recentes aos cmdlets de SQL

Os seguintes cmdlets foram afetados nesta versão:

### <a name="new-azurermsqldatabasefailovergroup"></a>New-AzureRmSqlDatabaseFailoverGroup
- O parâmetro `Tag` foi removido
- O nome do parâmetro `GracePeriodWithDataLossHour` foi mudado para `GracePeriodWithDataLossHours`

```powershell
# Old
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="set-azurermsqldatabasefailovergroup"></a>Set-AzureRmSqlDatabaseFailoverGroup
- O parâmetro `Tag` foi removido
- O nome do parâmetro `GracePeriodWithDataLossHour` foi mudado para `GracePeriodWithDataLossHours`

```powershell
# Old
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="add-azurermsqldatabasetofailovergroup"></a>Add-AzureRmSqlDatabaseToFailoverGroup
- O parâmetro `Tag` foi removido

```powershell
# Old
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

###  <a name="remove-azurermsqldatabasefromfailovergroup"></a>Remove-AzureRmSqlDatabaseFromFailoverGroup
- O parâmetro `Tag` foi removido

```powershell
# Old
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

### <a name="remove-azurermsqldatabasefailovergroup"></a>Remove-AzureRmSqlDatabaseFailoverGroup
- O parâmetro `PartnerResourceGroupName` foi removido
- O parâmetro `PartnerServerName` foi removido

```powershell
# Old
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -PartnerResourceGroupName rg

# New
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg
```

### <a name="set-azurermsqldatabasethreatdetectionpolicy"></a>Set-AzureRmSqlDatabaseThreatDetectionPolicy
- O valor `Usage_Anomaly` já não é válido para o parâmetro `ExcludedDetectionType`

### <a name="set-azurermsqlserverthreatdetectionpolicy"></a>Set-AzureRmSqlServerThreatDetectionPolicy
- O valor `Usage_Anomaly` já não é válido para o parâmetro `ExcludedDetectionType`

## <a name="breaking-changes-to-storage-cmdlets"></a>Alterações recentes aos cmdlets de Armazenamento

As seguintes propriedades de tipo de saída foram afetadas nesta versão:

### <a name="azurestorageblobicloudblobserviceclient"></a>AzureStorageBlob.ICloudBlob.ServiceClient
- As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- Esta alteração afeta os seguintes cmdlets:
    - `Get-AzureStorageBlob`
    - `Get-AzureStorageBlobContent`
    - `Get-AzureStorageBlobCopyState`
    - `Set-AzureStorageBlobContent`
    - `Start-AzureStorageBlobCopy`
    - `Stop-AzureStorageBlobCopy`
    
### <a name="azurestoragecontainercloudblobcontainerserviceclient"></a>AzureStorageContainer.CloudBlobContainer.ServiceClient
- As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- Esta alteração afeta os seguintes cmdlets:
    - `Get-AzureStorageContainer`
    - `New-AzureStorageContainer`
    - `Set-AzureStorageContainerAcl`
    
### <a name="azurestoragequeuecloudqueueserviceclient"></a>AzureStorageQueue.CloudQueue.ServiceClient
- As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):
    - `LocationMode`
    - `MaximumExecutionTime`
    - `RetryPolicy`
    - `ServerTimeout`
- Esta alteração afeta os seguintes cmdlets:
    - `Get-AzureStorageQueue`
    - `New-AzureStorageQueue`
    
### <a name="azurestoragetablecloudtableserviceclient"></a>AzureStorageTable.CloudTable.ServiceClient
- As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):
    - `LocationMode`
    - `MaximumExecutionTime`
    - `PayloadFormat`
    - `RetryPolicy`
    - `ServerTimeout`
- Esta alteração afeta os seguintes cmdlets:
    - `Get-AzureStorageTable`
    - `New-AzureStorageTable`
    
```powershell
# Old
$LocationMode = (Get-AzureStorageBlob -Container $containername)[0].ICloudBlob.ServiceClient.LocationMode       
$ParallelOperationThreadCount = (Get-AzureStorageContainer -Container $containername).CloudBlobContainer.ServiceClient.ParallelOperationThreadCount
$PayloadFormat = (Get-AzureStorageTable -Name $tablename).CloudTable.ServiceClient.PayloadFormat
$RetryPolicy = (Get-AzureStorageQueue -Name $queuename).CloudQueue.ServiceClient.RetryPolicy

# New
$LocationMode = (Get-AzureStorageBlob -Container $containername)[0].ICloudBlob.ServiceClient.DefaultRequestOptions.LocationMode     
$ParallelOperationThreadCount = (Get-AzureStorageContainer -Container $containername).CloudBlobContainer.ServiceClient.DefaultRequestOptions.ParallelOperationThreadCount
$PayloadFormat = (Get-AzureStorageTable -Name $tablename).CloudTable.ServiceClient.DefaultRequestOptions.PayloadFormat
$RetryPolicy = (Get-AzureStorageQueue -Name $queuename).CloudQueue.ServiceClient.DefaultRequestOptions.RetryPolicy
```

## <a name="breaking-changes-to-profile-cmdlets"></a>Alterações recentes aos cmdlets de Perfil

Os cmdlets e tipos de saída de cmdlet que se seguem foram alterados nesta versão.

### <a name="add-azurermaccount-breaking-changes"></a>Alterações recentes a Add-AzureRmAccount

- O parâmetro ```EnvironmentName``` foi removido e substituído por ```Environment``` e, agora, ```Environment``` precisa de uma cadeia e não de um objeto ```AzureEnvironment```

```powershell
# Old
Add-AzureRmAccount -EnvironmentName AzureChinaCloud

# New
Add-AzureRmAccount -Environment AzureChinaCloud
```

### <a name="select-azurermprofile-was-renamed-to-import-azurermcontext"></a>O nome de Select-AzureRmProfile foi mudado para Import-AzureRmContext

O nome de ```Select-AzureRmProfile``` foi mudado para ```Import-AzureRmContext```

```powershell
# Old
Select-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Import-AzureRmContext -Path c:\mydir\myprofile.json
```

### <a name="save-azurermprofile-was-renamed-to-save-azurermcontext"></a>O nome de Save-AzureRmProfile foi mudado para Save-AzureRmContext

O nome de ```Save-AzureRmProfile``` foi mudado para ```Save-AzureRmContext```

```powershell
# Old
Save-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Save-AzureRmContext -Path c:\mydir\myprofile.json
```
### <a name="breaking-changes-to-output-psazurecontext-type"></a>Alterações recentes à saída do Tipo PSAzureContext

- A propriedade ```TokenCache``` foi alterada para um tipo que implementa ```IAzureTokenCache``` em vez de um ```byte[]```

```powershell
# Old
$bytes = (Get-AzureRmContext).TokenCache
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache
$bytes = (Add-AzureRmAccount).Context.TokenCache

# New
$bytes = (Get-AzureRmContext).TokenCache.CacheData
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache.CacheData
$bytes = (Add-AzureRmAccount).Context.TokenCache.CacheData
```

### <a name="breaking-changes-to-the-output-psazureaccount-type"></a>Alterações recentes à saída do Tipo PSAzureAccount

- A propriedade ```AccountType``` foi alterada para ```Type```

```powershell
# Old
$type = (Get-AzureRmContext).Account.AccountType
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.AccountType
$type = (Add-AzureRmAccount).Context.Account.AccountType

# New 
$type = (Get-AzureRmContext).Account.Type
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.Type
$type = (Add-AzureRmAccount).Context.Account.Type
```

### <a name="breaking-changes-to-the-output-psazuresubscription-type"></a>Alterações recentes à saída do Tipo PSAzureSubscription
- A propriedade ```SubscriptionId``` foi alterada para ```Id```

```powershell
# Old
$id =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).SubscriptionId
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.SubscriptionId
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionId
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionId

# New
$id =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).Id
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.Id
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Id
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Id
```

- A propriedade ```SubscriptionName``` foi alterada para ```Name```

```powershell
# Old
$name =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).SubscriptionName
$name =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.SubscriptionName
$name =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionName
$name =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionName

# New
$name =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).Name
$name =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.Name
$name =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Name
$name =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Name
```

### <a name="breaking-changes-to-the-output-psazuretenant-type"></a>Alterações recentes à saída do Tipo PSAzureTenant

- A propriedade ```TenantId``` foi alterada para ```Id```

```powershell
# Old
$id =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).TenantId
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Tenant.TenantId
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.TenantId
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.TenantId

# New
$id =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Id
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Tenant.Id
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.Id
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.Id
```

- A propriedade ```Domain``` foi alterada para ```Directory```

```powershell
# Old
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Domain

# New
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Directory
```
