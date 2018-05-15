# <a name="breaking-changes-for-microsoft-azure-powershell-400"></a><span data-ttu-id="d64f3-101">Alterações recentes ao Microsoft Azure PowerShell 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d64f3-101">Breaking changes for Microsoft Azure PowerShell 4.0.0</span></span>

<span data-ttu-id="d64f3-102">Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d64f3-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="d64f3-103">Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço.</span><span class="sxs-lookup"><span data-stu-id="d64f3-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="d64f3-104">Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.</span><span class="sxs-lookup"><span data-stu-id="d64f3-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="d64f3-105">Índice</span><span class="sxs-lookup"><span data-stu-id="d64f3-105">Table of Contents</span></span>

- [<span data-ttu-id="d64f3-106">Alterações recentes aos cmdlets de Computação</span><span class="sxs-lookup"><span data-stu-id="d64f3-106">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="d64f3-107">Alterações recentes aos cmdlets de EventHub</span><span class="sxs-lookup"><span data-stu-id="d64f3-107">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="d64f3-108">Alterações recentes aos cmdlets de Insights</span><span class="sxs-lookup"><span data-stu-id="d64f3-108">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="d64f3-109">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="d64f3-109">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="d64f3-110">Alterações recentes aos cmdlets de ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d64f3-110">Breaking changes to ServiceBus cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)
- [<span data-ttu-id="d64f3-111">Alterações recentes aos cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="d64f3-111">Breaking changes to Sql cmdlets</span></span>](#breaking-changes-to-sql-cmdlets)
- [<span data-ttu-id="d64f3-112">Alterações recentes aos cmdlets de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d64f3-112">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
- [<span data-ttu-id="d64f3-113">Alterações recentes aos cmdlets de Perfil</span><span class="sxs-lookup"><span data-stu-id="d64f3-113">Breaking Changes to Profile Cmdlets</span></span>](#breaking-changes-to-profile-cmdlets)
## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="d64f3-114">Alterações recentes aos cmdlets de Computação</span><span class="sxs-lookup"><span data-stu-id="d64f3-114">Breaking changes to Compute cmdlets</span></span>

<span data-ttu-id="d64f3-115">Os seguintes tipos de saída foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-115">The following output types were affected this release:</span></span>

### <a name="psvirtualmachine"></a><span data-ttu-id="d64f3-116">PSVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="d64f3-116">PSVirtualMachine</span></span>
- <span data-ttu-id="d64f3-117">As propriedades de nível superior `DataDiskNames` e `NetworkInterfaceIDs` do objeto `PSVirtualMachine` foram removidas do tipo de saída.</span><span class="sxs-lookup"><span data-stu-id="d64f3-117">Top level properties `DataDiskNames` and `NetworkInterfaceIDs` of nthe `PSVirtualMachine` object have been removed from the output type.</span></span> <span data-ttu-id="d64f3-118">Estas propriedades têm estado sempre disponíveis nas propriedades `StorageProfile` e `NetworkProfile` do objeto `PSVirtualMachine` e esta é a forma como terão de ser acedidas daqui em diante.</span><span class="sxs-lookup"><span data-stu-id="d64f3-118">These properties have always been available in the `StorageProfile` and `NetworkProfile` properties of the `PSVirtualMachine` object and will be the way they will need to be accessed going forward.</span></span>
- <span data-ttu-id="d64f3-119">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d64f3-119">This change affects the following cmdlets:</span></span>
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

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="d64f3-120">Alterações recentes aos cmdlets de EventHub</span><span class="sxs-lookup"><span data-stu-id="d64f3-120">Breaking changes to EventHub cmdlets</span></span>

<span data-ttu-id="d64f3-121">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-121">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="d64f3-122">Get-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="d64f3-122">Get-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="d64f3-123">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="d64f3-123">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="d64f3-124">New-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="d64f3-124">New-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="d64f3-125">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="d64f3-125">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="d64f3-126">Alterações recentes aos cmdlets de Insights</span><span class="sxs-lookup"><span data-stu-id="d64f3-126">Breaking changes to Insights cmdlets</span></span>

<span data-ttu-id="d64f3-127">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-127">The following cmdlets were affected this release:</span></span>
    
### <a name="get-azurermusage"></a><span data-ttu-id="d64f3-128">Get-AzureRmUsage</span><span class="sxs-lookup"><span data-stu-id="d64f3-128">Get-AzureRmUsage</span></span>
- <span data-ttu-id="d64f3-129">Este cmdlet foi preterido.</span><span class="sxs-lookup"><span data-stu-id="d64f3-129">This cmdlet has been deprecated.</span></span>

### <a name="remove-azurermalertrule"></a><span data-ttu-id="d64f3-130">Remove-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="d64f3-130">Remove-AzureRmAlertRule</span></span>
- <span data-ttu-id="d64f3-131">A saída deste cmdlet foi alterada de uma lista com um único objeto para um objeto único; este objeto inclui o requestId e o código de estado.</span><span class="sxs-lookup"><span data-stu-id="d64f3-131">The output of this cmdlet has changed from a list with a single object to a single object; this object includes the requestId, and status code.</span></span>
    
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
    
### <a name="add-azurermlogalertrule"></a><span data-ttu-id="d64f3-132">Add-AzureRmLogAlertRule</span><span class="sxs-lookup"><span data-stu-id="d64f3-132">Add-AzureRmLogAlertRule</span></span>
- <span data-ttu-id="d64f3-133">Este cmdlet foi preterido.</span><span class="sxs-lookup"><span data-stu-id="d64f3-133">This cmdlet has been deprecated.</span></span>
    
### <a name="get-azurermalertrule"></a><span data-ttu-id="d64f3-134">Get-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="d64f3-134">Get-AzureRmAlertRule</span></span>
- <span data-ttu-id="d64f3-135">Cada elemento da saída (uma lista de objetos) deste cmdlet foi simplificado, ou seja, em vez de devolver objetos com a estrutura `{ Id, Location, Name, Tags, Properties }`, devolverá objetos com a estrutura `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, o que corresponde a todos os atributos de um Recurso do Azure juntamente com todos os atributos de um AlertRuleResource no nível superior.</span><span class="sxs-lookup"><span data-stu-id="d64f3-135">Each element of the the output (a list of objects) of this cmdlet is flattened, i.e. instead of returning objects with the structure `{ Id, Location, Name, Tags, Properties }` it will return objects with the structure `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, which is all of the attributes of an Azure Resource plus all of the attributes of an AlertRuleResource at the top level.</span></span>
    
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
    
### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="d64f3-136">Get-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="d64f3-136">Get-AzureRmAutoscaleSetting</span></span>
- <span data-ttu-id="d64f3-137">O campo `AutoscaleSettingResourceName` foi preterido porque tem sempre o mesmo valor que o campo `Name`.</span><span class="sxs-lookup"><span data-stu-id="d64f3-137">The `AutoscaleSettingResourceName` field is deprecated since it always has the same value as the `Name` field.</span></span>

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
    
### <a name="remove-azurermlogprofile"></a><span data-ttu-id="d64f3-138">Remove-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="d64f3-138">Remove-AzureRmLogProfile</span></span>
- <span data-ttu-id="d64f3-139">A saída deste cmdlet irá ser alterada de `Boolean` para um objeto que contém `RequestId` e `StatusCode`</span><span class="sxs-lookup"><span data-stu-id="d64f3-139">The output of this cmdlet will change from `Boolean` to and object containing `RequestId` and `StatusCode`</span></span>

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
    
### <a name="add-azurermlogprofile"></a><span data-ttu-id="d64f3-140">Add-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="d64f3-140">Add-AzureRmLogProfile</span></span>
- <span data-ttu-id="d64f3-141">A saída deste cmdlet irá ser alterada de um objeto que inclui o requestId, o código de estado e o recurso atualizado ou recém-criado</span><span class="sxs-lookup"><span data-stu-id="d64f3-141">The output of this cmdlet will change from an object that includes the requestId, status code, and the updated or newly created resource</span></span>
    
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
    
### <a name="set-azurermdiagnosticsettings"></a><span data-ttu-id="d64f3-142">Set-AzureRmDiagnosticSettings</span><span class="sxs-lookup"><span data-stu-id="d64f3-142">Set-AzureRmDiagnosticSettings</span></span>
- <span data-ttu-id="d64f3-143">O nome do comando irá ser mudado para `Update-AzureRmDiagnsoticSettings`</span><span class="sxs-lookup"><span data-stu-id="d64f3-143">The command is going to be renamed to `Update-AzureRmDiagnsoticSettings`</span></span>

```powershell
# Old
Set-AzureRmDiagnosticSettings

# New
Update-AzureRmDiagnosticSettings
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="d64f3-144">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="d64f3-144">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="d64f3-145">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-145">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermvirtualnetworkgatewayconnection"></a><span data-ttu-id="d64f3-146">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="d64f3-146">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="d64f3-147">O parâmetro `EnableBgp` foi alterado de modo a precisar de `boolean` em vez de `string`</span><span class="sxs-lookup"><span data-stu-id="d64f3-147">`EnableBgp` parameter has been changed to take a `boolean` instead of a `string`</span></span>

```powershell
# Old
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp "true"

# New
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp $true
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="d64f3-148">Alterações recentes aos cmdlets de ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d64f3-148">Breaking changes to ServiceBus cmdlets</span></span>

<span data-ttu-id="d64f3-149">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-149">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermservicebusnamespace"></a><span data-ttu-id="d64f3-150">Get-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="d64f3-150">Get-AzureRmServiceBusNamespace</span></span>
- <span data-ttu-id="d64f3-151">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="d64f3-151">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermservicebusnamespace"></a><span data-ttu-id="d64f3-152">New-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="d64f3-152">New-AzureRmServiceBusNamespace</span></span>

- <span data-ttu-id="d64f3-153">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="d64f3-153">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-sql-cmdlets"></a><span data-ttu-id="d64f3-154">Alterações recentes aos cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="d64f3-154">Breaking changes to Sql cmdlets</span></span>

<span data-ttu-id="d64f3-155">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-155">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermsqldatabasefailovergroup"></a><span data-ttu-id="d64f3-156">New-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="d64f3-156">New-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="d64f3-157">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="d64f3-157">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="d64f3-158">O nome do parâmetro `GracePeriodWithDataLossHour` foi mudado para `GracePeriodWithDataLossHours`</span><span class="sxs-lookup"><span data-stu-id="d64f3-158">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell
# Old
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="set-azurermsqldatabasefailovergroup"></a><span data-ttu-id="d64f3-159">Set-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="d64f3-159">Set-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="d64f3-160">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="d64f3-160">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="d64f3-161">O nome do parâmetro `GracePeriodWithDataLossHour` foi mudado para `GracePeriodWithDataLossHours`</span><span class="sxs-lookup"><span data-stu-id="d64f3-161">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell
# Old
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="add-azurermsqldatabasetofailovergroup"></a><span data-ttu-id="d64f3-162">Add-AzureRmSqlDatabaseToFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="d64f3-162">Add-AzureRmSqlDatabaseToFailoverGroup</span></span>
- <span data-ttu-id="d64f3-163">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="d64f3-163">`Tag` parameter has been removed</span></span>

```powershell
# Old
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

###  <a name="remove-azurermsqldatabasefromfailovergroup"></a><span data-ttu-id="d64f3-164">Remove-AzureRmSqlDatabaseFromFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="d64f3-164">Remove-AzureRmSqlDatabaseFromFailoverGroup</span></span>
- <span data-ttu-id="d64f3-165">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="d64f3-165">`Tag` parameter has been removed</span></span>

```powershell
# Old
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

### <a name="remove-azurermsqldatabasefailovergroup"></a><span data-ttu-id="d64f3-166">Remove-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="d64f3-166">Remove-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="d64f3-167">O parâmetro `PartnerResourceGroupName` foi removido</span><span class="sxs-lookup"><span data-stu-id="d64f3-167">`PartnerResourceGroupName` parameter has been removed</span></span>
- <span data-ttu-id="d64f3-168">O parâmetro `PartnerServerName` foi removido</span><span class="sxs-lookup"><span data-stu-id="d64f3-168">`PartnerServerName` parameter has been removed</span></span>

```powershell
# Old
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -PartnerResourceGroupName rg

# New
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg
```

### <a name="set-azurermsqldatabasethreatdetectionpolicy"></a><span data-ttu-id="d64f3-169">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d64f3-169">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span></span>
- <span data-ttu-id="d64f3-170">O valor `Usage_Anomaly` já não é válido para o parâmetro `ExcludedDetectionType`</span><span class="sxs-lookup"><span data-stu-id="d64f3-170">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

### <a name="set-azurermsqlserverthreatdetectionpolicy"></a><span data-ttu-id="d64f3-171">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d64f3-171">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
- <span data-ttu-id="d64f3-172">O valor `Usage_Anomaly` já não é válido para o parâmetro `ExcludedDetectionType`</span><span class="sxs-lookup"><span data-stu-id="d64f3-172">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="d64f3-173">Alterações recentes aos cmdlets de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d64f3-173">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="d64f3-174">As seguintes propriedades de tipo de saída foram afetadas nesta versão:</span><span class="sxs-lookup"><span data-stu-id="d64f3-174">The following output type properties were affected this release:</span></span>

### <a name="azurestorageblobicloudblobserviceclient"></a><span data-ttu-id="d64f3-175">AzureStorageBlob.ICloudBlob.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="d64f3-175">AzureStorageBlob.ICloudBlob.ServiceClient</span></span>
- <span data-ttu-id="d64f3-176">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="d64f3-176">The following properties were removed from this type (_note_: they can still be found in `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="d64f3-177">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d64f3-177">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageBlob`
    - `Get-AzureStorageBlobContent`
    - `Get-AzureStorageBlobCopyState`
    - `Set-AzureStorageBlobContent`
    - `Start-AzureStorageBlobCopy`
    - `Stop-AzureStorageBlobCopy`
    
### <a name="azurestoragecontainercloudblobcontainerserviceclient"></a><span data-ttu-id="d64f3-178">AzureStorageContainer.CloudBlobContainer.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="d64f3-178">AzureStorageContainer.CloudBlobContainer.ServiceClient</span></span>
- <span data-ttu-id="d64f3-179">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="d64f3-179">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="d64f3-180">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d64f3-180">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageContainer`
    - `New-AzureStorageContainer`
    - `Set-AzureStorageContainerAcl`
    
### <a name="azurestoragequeuecloudqueueserviceclient"></a><span data-ttu-id="d64f3-181">AzureStorageQueue.CloudQueue.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="d64f3-181">AzureStorageQueue.CloudQueue.ServiceClient</span></span>
- <span data-ttu-id="d64f3-182">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="d64f3-182">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="d64f3-183">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d64f3-183">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageQueue`
    - `New-AzureStorageQueue`
    
### <a name="azurestoragetablecloudtableserviceclient"></a><span data-ttu-id="d64f3-184">AzureStorageTable.CloudTable.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="d64f3-184">AzureStorageTable.CloudTable.ServiceClient</span></span>
- <span data-ttu-id="d64f3-185">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="d64f3-185">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `PayloadFormat`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="d64f3-186">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d64f3-186">This change affects the following cmdlets:</span></span>
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

## <a name="breaking-changes-to-profile-cmdlets"></a><span data-ttu-id="d64f3-187">Alterações recentes aos cmdlets de Perfil</span><span class="sxs-lookup"><span data-stu-id="d64f3-187">Breaking Changes to Profile Cmdlets</span></span>

<span data-ttu-id="d64f3-188">Os cmdlets e tipos de saída de cmdlet que se seguem foram alterados nesta versão.</span><span class="sxs-lookup"><span data-stu-id="d64f3-188">The following cmdlets and cmdlet output types were changed in this release.</span></span>

### <a name="add-azurermaccount-breaking-changes"></a><span data-ttu-id="d64f3-189">Alterações recentes a Add-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="d64f3-189">Add-AzureRmAccount breaking changes</span></span>

- <span data-ttu-id="d64f3-190">O parâmetro ```EnvironmentName``` foi removido e substituído por ```Environment``` e, agora, ```Environment``` precisa de uma cadeia e não de um objeto ```AzureEnvironment```</span><span class="sxs-lookup"><span data-stu-id="d64f3-190">```EnvironmentName``` parameter has been removed and replaced with ```Environment```, the ```Environment``` now takes a string and not an ```AzureEnvironment``` object</span></span>

```powershell
# Old
Add-AzureRmAccount -EnvironmentName AzureChinaCloud

# New
Add-AzureRmAccount -Environment AzureChinaCloud
```

### <a name="select-azurermprofile-was-renamed-to-import-azurermcontext"></a><span data-ttu-id="d64f3-191">O nome de Select-AzureRmProfile foi mudado para Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="d64f3-191">Select-AzureRmProfile was renamed to Import-AzureRmContext</span></span>

<span data-ttu-id="d64f3-192">O nome de ```Select-AzureRmProfile``` foi mudado para ```Import-AzureRmContext```</span><span class="sxs-lookup"><span data-stu-id="d64f3-192">```Select-AzureRmProfile``` was renamed to ```Import-AzureRmContext```</span></span>

```powershell
# Old
Select-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Import-AzureRmContext -Path c:\mydir\myprofile.json
```

### <a name="save-azurermprofile-was-renamed-to-save-azurermcontext"></a><span data-ttu-id="d64f3-193">O nome de Save-AzureRmProfile foi mudado para Save-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="d64f3-193">Save-AzureRmProfile was renamed to Save-AzureRmContext</span></span>

<span data-ttu-id="d64f3-194">O nome de ```Save-AzureRmProfile``` foi mudado para ```Save-AzureRmContext```</span><span class="sxs-lookup"><span data-stu-id="d64f3-194">```Save-AzureRmProfile``` was renamed to ```Save-AzureRmContext```</span></span>

```powershell
# Old
Save-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Save-AzureRmContext -Path c:\mydir\myprofile.json
```
### <a name="breaking-changes-to-output-psazurecontext-type"></a><span data-ttu-id="d64f3-195">Alterações recentes à saída do Tipo PSAzureContext</span><span class="sxs-lookup"><span data-stu-id="d64f3-195">Breaking Changes to output PSAzureContext Type</span></span>

- <span data-ttu-id="d64f3-196">A propriedade ```TokenCache``` foi alterada para um tipo que implementa ```IAzureTokenCache``` em vez de um ```byte[]```</span><span class="sxs-lookup"><span data-stu-id="d64f3-196">The ```TokenCache``` property changed to a type that implements ```IAzureTokenCache``` instead of a ```byte[]```</span></span>

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

### <a name="breaking-changes-to-the-output-psazureaccount-type"></a><span data-ttu-id="d64f3-197">Alterações recentes à saída do Tipo PSAzureAccount</span><span class="sxs-lookup"><span data-stu-id="d64f3-197">Breaking Changes to the output PSAzureAccount Type</span></span>

- <span data-ttu-id="d64f3-198">A propriedade ```AccountType``` foi alterada para ```Type```</span><span class="sxs-lookup"><span data-stu-id="d64f3-198">The ```AccountType``` property was changed to ```Type```</span></span>

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

### <a name="breaking-changes-to-the-output-psazuresubscription-type"></a><span data-ttu-id="d64f3-199">Alterações recentes à saída do Tipo PSAzureSubscription</span><span class="sxs-lookup"><span data-stu-id="d64f3-199">Breaking Changes to the output PSAzureSubscription Type</span></span>
- <span data-ttu-id="d64f3-200">A propriedade ```SubscriptionId``` foi alterada para ```Id```</span><span class="sxs-lookup"><span data-stu-id="d64f3-200">The ```SubscriptionId``` property was changed to ```Id```</span></span>

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

- <span data-ttu-id="d64f3-201">A propriedade ```SubscriptionName``` foi alterada para ```Name```</span><span class="sxs-lookup"><span data-stu-id="d64f3-201">The ```SubscriptionName``` property was changed to ```Name```</span></span>

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

### <a name="breaking-changes-to-the-output-psazuretenant-type"></a><span data-ttu-id="d64f3-202">Alterações recentes à saída do Tipo PSAzureTenant</span><span class="sxs-lookup"><span data-stu-id="d64f3-202">Breaking Changes to the output PSAzureTenant Type</span></span>

- <span data-ttu-id="d64f3-203">A propriedade ```TenantId``` foi alterada para ```Id```</span><span class="sxs-lookup"><span data-stu-id="d64f3-203">The ```TenantId``` property was changed to ```Id```</span></span>

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

- <span data-ttu-id="d64f3-204">A propriedade ```Domain``` foi alterada para ```Directory```</span><span class="sxs-lookup"><span data-stu-id="d64f3-204">The ```Domain``` property was changed to ```Directory```</span></span>

```powershell
# Old
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Domain

# New
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Directory
```
