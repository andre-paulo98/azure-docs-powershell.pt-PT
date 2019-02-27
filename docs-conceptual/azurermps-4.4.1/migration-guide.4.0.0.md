---
title: Alterações recentes ao Microsoft Azure PowerShell 4.0.0
description: Este guia de migração contém uma lista de alterações recentes realizadas no Azure PowerShell no lançamento da versão 4.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: 379bbc788e530598f51e893a2bad71f09b059193
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153443"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-400"></a><span data-ttu-id="80a00-103">Alterações recentes ao Microsoft Azure PowerShell 4.0.0</span><span class="sxs-lookup"><span data-stu-id="80a00-103">Breaking changes for Microsoft Azure PowerShell 4.0.0</span></span>

<span data-ttu-id="80a00-104">Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="80a00-104">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="80a00-105">Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço.</span><span class="sxs-lookup"><span data-stu-id="80a00-105">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="80a00-106">Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.</span><span class="sxs-lookup"><span data-stu-id="80a00-106">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="80a00-107">Índice</span><span class="sxs-lookup"><span data-stu-id="80a00-107">Table of Contents</span></span>

- [<span data-ttu-id="80a00-108">Alterações recentes aos cmdlets de Computação</span><span class="sxs-lookup"><span data-stu-id="80a00-108">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="80a00-109">Alterações recentes aos cmdlets de EventHub</span><span class="sxs-lookup"><span data-stu-id="80a00-109">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="80a00-110">Alterações recentes aos cmdlets de Insights</span><span class="sxs-lookup"><span data-stu-id="80a00-110">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="80a00-111">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="80a00-111">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="80a00-112">Alterações recentes aos cmdlets de ServiceBus</span><span class="sxs-lookup"><span data-stu-id="80a00-112">Breaking changes to ServiceBus cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)
- [<span data-ttu-id="80a00-113">Alterações recentes aos cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="80a00-113">Breaking changes to Sql cmdlets</span></span>](#breaking-changes-to-sql-cmdlets)
- [<span data-ttu-id="80a00-114">Alterações recentes aos cmdlets de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="80a00-114">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
- [<span data-ttu-id="80a00-115">Alterações recentes aos cmdlets de Perfil</span><span class="sxs-lookup"><span data-stu-id="80a00-115">Breaking Changes to Profile Cmdlets</span></span>](#breaking-changes-to-profile-cmdlets)
  ## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="80a00-116">Alterações recentes aos cmdlets de Computação</span><span class="sxs-lookup"><span data-stu-id="80a00-116">Breaking changes to Compute cmdlets</span></span>

<span data-ttu-id="80a00-117">Os seguintes tipos de saída foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-117">The following output types were affected this release:</span></span>

### <a name="psvirtualmachine"></a><span data-ttu-id="80a00-118">PSVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="80a00-118">PSVirtualMachine</span></span>
- <span data-ttu-id="80a00-119">As propriedades de nível superior `DataDiskNames` e `NetworkInterfaceIDs` do objeto `PSVirtualMachine` foram removidas do tipo de saída.</span><span class="sxs-lookup"><span data-stu-id="80a00-119">Top level properties `DataDiskNames` and `NetworkInterfaceIDs` of nthe `PSVirtualMachine` object have been removed from the output type.</span></span> <span data-ttu-id="80a00-120">Estas propriedades têm estado sempre disponíveis nas propriedades `StorageProfile` e `NetworkProfile` do objeto `PSVirtualMachine` e esta é a forma como terão de ser acedidas daqui em diante.</span><span class="sxs-lookup"><span data-stu-id="80a00-120">These properties have always been available in the `StorageProfile` and `NetworkProfile` properties of the `PSVirtualMachine` object and will be the way they will need to be accessed going forward.</span></span>
- <span data-ttu-id="80a00-121">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="80a00-121">This change affects the following cmdlets:</span></span>
    - `Add-AzureRmVMDataDisk`
    - `Add-AzureRmVMNetworkInterface`
    - `Get-AzureRmVM`
    - `Remove-AzureRmVMDataDisk`
    - `Remove-AzureRmVMNetworkInterface`
    - `Set-AzureRmVMDataDisk`

```powershell-interactive
# Old
$vm.DataDiskNames
$vm.NetworkInterfaceIDs

# New
$vm.StorageProfile.DataDisks | Select -Property Name
$vm.NetworkProfile.NetworkInterfaces | Select -Property Id
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="80a00-122">Alterações recentes aos cmdlets de EventHub</span><span class="sxs-lookup"><span data-stu-id="80a00-122">Breaking changes to EventHub cmdlets</span></span>

<span data-ttu-id="80a00-123">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-123">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="80a00-124">Get-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="80a00-124">Get-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="80a00-125">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="80a00-125">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="80a00-126">New-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="80a00-126">New-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="80a00-127">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="80a00-127">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="80a00-128">Alterações recentes aos cmdlets de Insights</span><span class="sxs-lookup"><span data-stu-id="80a00-128">Breaking changes to Insights cmdlets</span></span>

<span data-ttu-id="80a00-129">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-129">The following cmdlets were affected this release:</span></span>
    
### <a name="get-azurermusage"></a><span data-ttu-id="80a00-130">Get-AzureRmUsage</span><span class="sxs-lookup"><span data-stu-id="80a00-130">Get-AzureRmUsage</span></span>
- <span data-ttu-id="80a00-131">Este cmdlet foi preterido.</span><span class="sxs-lookup"><span data-stu-id="80a00-131">This cmdlet has been deprecated.</span></span>

### <a name="remove-azurermalertrule"></a><span data-ttu-id="80a00-132">Remove-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="80a00-132">Remove-AzureRmAlertRule</span></span>
- <span data-ttu-id="80a00-133">A saída deste cmdlet foi alterada de uma lista com um único objeto para um objeto único; este objeto inclui o requestId e o código de estado.</span><span class="sxs-lookup"><span data-stu-id="80a00-133">The output of this cmdlet has changed from a list with a single object to a single object; this object includes the requestId, and status code.</span></span>
    
```powershell-interactive
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
    
### <a name="add-azurermlogalertrule"></a><span data-ttu-id="80a00-134">Add-AzureRmLogAlertRule</span><span class="sxs-lookup"><span data-stu-id="80a00-134">Add-AzureRmLogAlertRule</span></span>
- <span data-ttu-id="80a00-135">Este cmdlet foi preterido.</span><span class="sxs-lookup"><span data-stu-id="80a00-135">This cmdlet has been deprecated.</span></span>
    
### <a name="get-azurermalertrule"></a><span data-ttu-id="80a00-136">Get-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="80a00-136">Get-AzureRmAlertRule</span></span>
- <span data-ttu-id="80a00-137">Cada elemento da saída (uma lista de objetos) deste cmdlet foi simplificado, ou seja, em vez de devolver objetos com a estrutura `{ Id, Location, Name, Tags, Properties }`, devolverá objetos com a estrutura `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, o que corresponde a todos os atributos de um Recurso do Azure juntamente com todos os atributos de um AlertRuleResource no nível superior.</span><span class="sxs-lookup"><span data-stu-id="80a00-137">Each element of the the output (a list of objects) of this cmdlet is flattened, i.e. instead of returning objects with the structure `{ Id, Location, Name, Tags, Properties }` it will return objects with the structure `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, which is all of the attributes of an Azure Resource plus all of the attributes of an AlertRuleResource at the top level.</span></span>
    
```powershell-interactive
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
    
### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="80a00-138">Get-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="80a00-138">Get-AzureRmAutoscaleSetting</span></span>
- <span data-ttu-id="80a00-139">O campo `AutoscaleSettingResourceName` foi preterido porque tem sempre o mesmo valor que o campo `Name`.</span><span class="sxs-lookup"><span data-stu-id="80a00-139">The `AutoscaleSettingResourceName` field is deprecated since it always has the same value as the `Name` field.</span></span>

```powershell-interactive
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
    
### <a name="remove-azurermlogprofile"></a><span data-ttu-id="80a00-140">Remove-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="80a00-140">Remove-AzureRmLogProfile</span></span>
- <span data-ttu-id="80a00-141">A saída deste cmdlet irá ser alterada de `Boolean` para um objeto que contém `RequestId` e `StatusCode`</span><span class="sxs-lookup"><span data-stu-id="80a00-141">The output of this cmdlet will change from `Boolean` to and object containing `RequestId` and `StatusCode`</span></span>

```powershell-interactive
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
    
### <a name="add-azurermlogprofile"></a><span data-ttu-id="80a00-142">Add-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="80a00-142">Add-AzureRmLogProfile</span></span>
- <span data-ttu-id="80a00-143">A saída deste cmdlet irá ser alterada de um objeto que inclui o requestId, o código de estado e o recurso atualizado ou recém-criado</span><span class="sxs-lookup"><span data-stu-id="80a00-143">The output of this cmdlet will change from an object that includes the requestId, status code, and the updated or newly created resource</span></span>
    
```powershell-interactive
# Old  
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.ServiceBusRuleId

# New
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.RequestId
$s = $s1.StatusCode
$a = $s1.NewResource.ServiceBusRuleId
    
```
    
### <a name="set-azurermdiagnosticsettings"></a><span data-ttu-id="80a00-144">Set-AzureRmDiagnosticSettings</span><span class="sxs-lookup"><span data-stu-id="80a00-144">Set-AzureRmDiagnosticSettings</span></span>
- <span data-ttu-id="80a00-145">O nome do comando irá ser mudado para `Update-AzureRmDiagnsoticSettings`</span><span class="sxs-lookup"><span data-stu-id="80a00-145">The command is going to be renamed to `Update-AzureRmDiagnsoticSettings`</span></span>

```powershell-interactive
# Old
Set-AzureRmDiagnosticSettings

# New
Update-AzureRmDiagnosticSettings
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="80a00-146">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="80a00-146">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="80a00-147">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-147">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermvirtualnetworkgatewayconnection"></a><span data-ttu-id="80a00-148">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="80a00-148">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="80a00-149">O parâmetro `EnableBgp` foi alterado de modo a precisar de `boolean` em vez de `string`</span><span class="sxs-lookup"><span data-stu-id="80a00-149">`EnableBgp` parameter has been changed to take a `boolean` instead of a `string`</span></span>

```powershell-interactive
# Old
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp "true"

# New
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp $true
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="80a00-150">Alterações recentes aos cmdlets de ServiceBus</span><span class="sxs-lookup"><span data-stu-id="80a00-150">Breaking changes to ServiceBus cmdlets</span></span>

<span data-ttu-id="80a00-151">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-151">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermservicebusnamespace"></a><span data-ttu-id="80a00-152">Get-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="80a00-152">Get-AzureRmServiceBusNamespace</span></span>
- <span data-ttu-id="80a00-153">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="80a00-153">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermservicebusnamespace"></a><span data-ttu-id="80a00-154">New-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="80a00-154">New-AzureRmServiceBusNamespace</span></span>

- <span data-ttu-id="80a00-155">A propriedade `ResourceGroupName` foi removida do tipo de saída `NamespaceAttributes`</span><span class="sxs-lookup"><span data-stu-id="80a00-155">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-sql-cmdlets"></a><span data-ttu-id="80a00-156">Alterações recentes aos cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="80a00-156">Breaking changes to Sql cmdlets</span></span>

<span data-ttu-id="80a00-157">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-157">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermsqldatabasefailovergroup"></a><span data-ttu-id="80a00-158">New-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="80a00-158">New-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="80a00-159">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="80a00-159">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="80a00-160">O nome do parâmetro `GracePeriodWithDataLossHour` foi mudado para `GracePeriodWithDataLossHours`</span><span class="sxs-lookup"><span data-stu-id="80a00-160">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell-interactive
# Old
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="set-azurermsqldatabasefailovergroup"></a><span data-ttu-id="80a00-161">Set-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="80a00-161">Set-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="80a00-162">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="80a00-162">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="80a00-163">O nome do parâmetro `GracePeriodWithDataLossHour` foi mudado para `GracePeriodWithDataLossHours`</span><span class="sxs-lookup"><span data-stu-id="80a00-163">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell-interactive
# Old
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="add-azurermsqldatabasetofailovergroup"></a><span data-ttu-id="80a00-164">Add-AzureRmSqlDatabaseToFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="80a00-164">Add-AzureRmSqlDatabaseToFailoverGroup</span></span>
- <span data-ttu-id="80a00-165">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="80a00-165">`Tag` parameter has been removed</span></span>

```powershell-interactive
# Old
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

###  <a name="remove-azurermsqldatabasefromfailovergroup"></a><span data-ttu-id="80a00-166">Remove-AzureRmSqlDatabaseFromFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="80a00-166">Remove-AzureRmSqlDatabaseFromFailoverGroup</span></span>
- <span data-ttu-id="80a00-167">O parâmetro `Tag` foi removido</span><span class="sxs-lookup"><span data-stu-id="80a00-167">`Tag` parameter has been removed</span></span>

```powershell-interactive
# Old
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

### <a name="remove-azurermsqldatabasefailovergroup"></a><span data-ttu-id="80a00-168">Remove-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="80a00-168">Remove-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="80a00-169">O parâmetro `PartnerResourceGroupName` foi removido</span><span class="sxs-lookup"><span data-stu-id="80a00-169">`PartnerResourceGroupName` parameter has been removed</span></span>
- <span data-ttu-id="80a00-170">O parâmetro `PartnerServerName` foi removido</span><span class="sxs-lookup"><span data-stu-id="80a00-170">`PartnerServerName` parameter has been removed</span></span>

```powershell-interactive
# Old
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -PartnerResourceGroupName rg

# New
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg
```

### <a name="set-azurermsqldatabasethreatdetectionpolicy"></a><span data-ttu-id="80a00-171">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="80a00-171">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span></span>
- <span data-ttu-id="80a00-172">O valor `Usage_Anomaly` já não é válido para o parâmetro `ExcludedDetectionType`</span><span class="sxs-lookup"><span data-stu-id="80a00-172">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

### <a name="set-azurermsqlserverthreatdetectionpolicy"></a><span data-ttu-id="80a00-173">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="80a00-173">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
- <span data-ttu-id="80a00-174">O valor `Usage_Anomaly` já não é válido para o parâmetro `ExcludedDetectionType`</span><span class="sxs-lookup"><span data-stu-id="80a00-174">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="80a00-175">Alterações recentes aos cmdlets de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="80a00-175">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="80a00-176">As seguintes propriedades de tipo de saída foram afetadas nesta versão:</span><span class="sxs-lookup"><span data-stu-id="80a00-176">The following output type properties were affected this release:</span></span>

### <a name="azurestorageblobicloudblobserviceclient"></a><span data-ttu-id="80a00-177">AzureStorageBlob.ICloudBlob.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="80a00-177">AzureStorageBlob.ICloudBlob.ServiceClient</span></span>
- <span data-ttu-id="80a00-178">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="80a00-178">The following properties were removed from this type (_note_: they can still be found in `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="80a00-179">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="80a00-179">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageBlob`
    - `Get-AzureStorageBlobContent`
    - `Get-AzureStorageBlobCopyState`
    - `Set-AzureStorageBlobContent`
    - `Start-AzureStorageBlobCopy`
    - `Stop-AzureStorageBlobCopy`
    
### <a name="azurestoragecontainercloudblobcontainerserviceclient"></a><span data-ttu-id="80a00-180">AzureStorageContainer.CloudBlobContainer.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="80a00-180">AzureStorageContainer.CloudBlobContainer.ServiceClient</span></span>
- <span data-ttu-id="80a00-181">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="80a00-181">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="80a00-182">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="80a00-182">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageContainer`
    - `New-AzureStorageContainer`
    - `Set-AzureStorageContainerAcl`
    
### <a name="azurestoragequeuecloudqueueserviceclient"></a><span data-ttu-id="80a00-183">AzureStorageQueue.CloudQueue.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="80a00-183">AzureStorageQueue.CloudQueue.ServiceClient</span></span>
- <span data-ttu-id="80a00-184">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="80a00-184">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="80a00-185">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="80a00-185">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageQueue`
    - `New-AzureStorageQueue`
    
### <a name="azurestoragetablecloudtableserviceclient"></a><span data-ttu-id="80a00-186">AzureStorageTable.CloudTable.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="80a00-186">AzureStorageTable.CloudTable.ServiceClient</span></span>
- <span data-ttu-id="80a00-187">As seguintes propriedades foram removidas deste tipo (_nota_: ainda podem ser encontradas na propriedade `DefaultRequestOptions`):</span><span class="sxs-lookup"><span data-stu-id="80a00-187">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `PayloadFormat`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="80a00-188">Esta alteração afeta os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="80a00-188">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageTable`
    - `New-AzureStorageTable`
    
```powershell-interactive
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

## <a name="breaking-changes-to-profile-cmdlets"></a><span data-ttu-id="80a00-189">Alterações recentes aos cmdlets de Perfil</span><span class="sxs-lookup"><span data-stu-id="80a00-189">Breaking Changes to Profile Cmdlets</span></span>

<span data-ttu-id="80a00-190">Os cmdlets e tipos de saída de cmdlet que se seguem foram alterados nesta versão.</span><span class="sxs-lookup"><span data-stu-id="80a00-190">The following cmdlets and cmdlet output types were changed in this release.</span></span>

### <a name="add-azurermaccount-breaking-changes"></a><span data-ttu-id="80a00-191">Alterações recentes a Add-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="80a00-191">Add-AzureRmAccount breaking changes</span></span>

- <span data-ttu-id="80a00-192">O parâmetro ```EnvironmentName``` foi removido e substituído por ```Environment``` e, agora, ```Environment``` precisa de uma cadeia e não de um objeto ```AzureEnvironment```</span><span class="sxs-lookup"><span data-stu-id="80a00-192">```EnvironmentName``` parameter has been removed and replaced with ```Environment```, the ```Environment``` now takes a string and not an ```AzureEnvironment``` object</span></span>

```powershell-interactive
# Old
Add-AzureRmAccount -EnvironmentName AzureChinaCloud

# New
Add-AzureRmAccount -Environment AzureChinaCloud
```

### <a name="select-azurermprofile-was-renamed-to-import-azurermcontext"></a><span data-ttu-id="80a00-193">O nome de Select-AzureRmProfile foi mudado para Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="80a00-193">Select-AzureRmProfile was renamed to Import-AzureRmContext</span></span>

<span data-ttu-id="80a00-194">O nome de ```Select-AzureRmProfile``` foi mudado para ```Import-AzureRmContext```</span><span class="sxs-lookup"><span data-stu-id="80a00-194">```Select-AzureRmProfile``` was renamed to ```Import-AzureRmContext```</span></span>

```powershell-interactive
# Old
Select-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Import-AzureRmContext -Path c:\mydir\myprofile.json
```

### <a name="save-azurermprofile-was-renamed-to-save-azurermcontext"></a><span data-ttu-id="80a00-195">O nome de Save-AzureRmProfile foi mudado para Save-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="80a00-195">Save-AzureRmProfile was renamed to Save-AzureRmContext</span></span>

<span data-ttu-id="80a00-196">O nome de ```Save-AzureRmProfile``` foi mudado para ```Save-AzureRmContext```</span><span class="sxs-lookup"><span data-stu-id="80a00-196">```Save-AzureRmProfile``` was renamed to ```Save-AzureRmContext```</span></span>

```powershell-interactive
# Old
Save-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Save-AzureRmContext -Path c:\mydir\myprofile.json
```
### <a name="breaking-changes-to-output-psazurecontext-type"></a><span data-ttu-id="80a00-197">Alterações recentes à saída do Tipo PSAzureContext</span><span class="sxs-lookup"><span data-stu-id="80a00-197">Breaking Changes to output PSAzureContext Type</span></span>

- <span data-ttu-id="80a00-198">A propriedade ```TokenCache``` foi alterada para um tipo que implementa ```IAzureTokenCache``` em vez de um ```byte[]```</span><span class="sxs-lookup"><span data-stu-id="80a00-198">The ```TokenCache``` property changed to a type that implements ```IAzureTokenCache``` instead of a ```byte[]```</span></span>

```powershell-interactive
# Old
$bytes = (Get-AzureRmContext).TokenCache
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache
$bytes = (Add-AzureRmAccount).Context.TokenCache

# New
$bytes = (Get-AzureRmContext).TokenCache.CacheData
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache.CacheData
$bytes = (Add-AzureRmAccount).Context.TokenCache.CacheData
```

### <a name="breaking-changes-to-the-output-psazureaccount-type"></a><span data-ttu-id="80a00-199">Alterações recentes à saída do Tipo PSAzureAccount</span><span class="sxs-lookup"><span data-stu-id="80a00-199">Breaking Changes to the output PSAzureAccount Type</span></span>

- <span data-ttu-id="80a00-200">A propriedade ```AccountType``` foi alterada para ```Type```</span><span class="sxs-lookup"><span data-stu-id="80a00-200">The ```AccountType``` property was changed to ```Type```</span></span>

```powershell-interactive
# Old
$type = (Get-AzureRmContext).Account.AccountType
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.AccountType
$type = (Add-AzureRmAccount).Context.Account.AccountType

# New 
$type = (Get-AzureRmContext).Account.Type
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.Type
$type = (Add-AzureRmAccount).Context.Account.Type
```

### <a name="breaking-changes-to-the-output-psazuresubscription-type"></a><span data-ttu-id="80a00-201">Alterações recentes à saída do Tipo PSAzureSubscription</span><span class="sxs-lookup"><span data-stu-id="80a00-201">Breaking Changes to the output PSAzureSubscription Type</span></span>
- <span data-ttu-id="80a00-202">A propriedade ```SubscriptionId``` foi alterada para ```Id```</span><span class="sxs-lookup"><span data-stu-id="80a00-202">The ```SubscriptionId``` property was changed to ```Id```</span></span>

```powershell-interactive
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

- <span data-ttu-id="80a00-203">A propriedade ```SubscriptionName``` foi alterada para ```Name```</span><span class="sxs-lookup"><span data-stu-id="80a00-203">The ```SubscriptionName``` property was changed to ```Name```</span></span>

```powershell-interactive
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

### <a name="breaking-changes-to-the-output-psazuretenant-type"></a><span data-ttu-id="80a00-204">Alterações recentes à saída do Tipo PSAzureTenant</span><span class="sxs-lookup"><span data-stu-id="80a00-204">Breaking Changes to the output PSAzureTenant Type</span></span>

- <span data-ttu-id="80a00-205">A propriedade ```TenantId``` foi alterada para ```Id```</span><span class="sxs-lookup"><span data-stu-id="80a00-205">The ```TenantId``` property was changed to ```Id```</span></span>

```powershell-interactive
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

- <span data-ttu-id="80a00-206">A propriedade ```Domain``` foi alterada para ```Directory```</span><span class="sxs-lookup"><span data-stu-id="80a00-206">The ```Domain``` property was changed to ```Directory```</span></span>

```powershell-interactive
# Old
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Domain

# New
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Directory
```
