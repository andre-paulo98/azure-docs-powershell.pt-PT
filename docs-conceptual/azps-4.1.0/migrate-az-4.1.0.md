---
ms.openlocfilehash: 636fd0432d421f74fa74f3275abbc31ec5dc0b5c
ms.sourcegitcommit: 31f4facf815c2e25dc44e2fde0e1d2bd690bfc54
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/20/2020
ms.locfileid: "83688531"
---
# <a name="migration-guide-for-az-410"></a><span data-ttu-id="2b3b9-101">Guia de Migração para o Az 4.1.0</span><span class="sxs-lookup"><span data-stu-id="2b3b9-101">Migration Guide for Az 4.1.0</span></span>

<span data-ttu-id="2b3b9-102">Este documento descreve as alterações realizadas entre as versões 3.0.0 e 4.1.0 do Az.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-102">This document describes the changes between the 3.0.0 and 4.1.0 versions of Az.</span></span>

- [<span data-ttu-id="2b3b9-103">Guia de migração para o Az 4.1.0</span><span class="sxs-lookup"><span data-stu-id="2b3b9-103">Migration Guide for Az 4.1.0</span></span>](#migration-guide-for-az-410)
  - [<span data-ttu-id="2b3b9-104">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b3b9-104">Az.ApiManagement</span></span>](#azapimanagement)
    - [`Add-AzApiManagementRegion`](#add-azapimanagementregion)
    - [`New-AzApiManagement`](#new-azapimanagement)
    - [`Set-AzApiManagement`](#set-azapimanagement)
    - [`Get-AzApiManagementProperty`](#get-azapimanagementproperty)
    - [`New-AzApiManagementProperty`](#new-azapimanagementproperty)
    - [`Remove-AzApiManagementProperty`](#remove-azapimanagementproperty)
    - [`Set-AzApiManagementProperty`](#set-azapimanagementproperty)
  - [<span data-ttu-id="2b3b9-105">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b3b9-105">Az.Batch</span></span>](#azbatch)
    - [<span data-ttu-id="2b3b9-106">`Get-AzBatchApplication`, `New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-106">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>](#get-azbatchapplication-new-azbatchapplication)
    - [<span data-ttu-id="2b3b9-107">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-107">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>](#get-azbatchcomputenode-new-azbatchpool)
    - [<span data-ttu-id="2b3b9-108">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-108">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>](#get-azbatchapplicationpackage-new-azbatchapplicationpackage)
  - [<span data-ttu-id="2b3b9-109">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b3b9-109">Az.Compute</span></span>](#azcompute)
    - [`Remove-AzVmssDiagnosticsExtension`](#remove-azvmssdiagnosticsextension)
    - [`Get-AzVMImage`](#get-azvmimage)
    - [`New-AzVMConfig`](#new-azvmconfig)
    - [`Update-AzVM`](#update-azvm)
    - [`New-AzProximityPlacementGroup`](#new-azproximityplacementgroup)
    - [`Remove-AzProximityPlacementGroup`](#remove-azproximityplacementgroup)
    - [`Get-AzProximityPlacementGroup`](#get-azproximityplacementgroup)
    - [`Add-AzVmssAdditionalUnattendContent`](#add-azvmssadditionalunattendcontent)
    - [`Add-AzVmssDataDisk`](#add-azvmssdatadisk)
    - [`Add-AzVmssExtension`](#add-azvmssextension)
    - [`Add-AzVmssNetworkInterfaceConfiguration`](#add-azvmssnetworkinterfaceconfiguration)
    - [`Add-AzVmssSecret`](#add-azvmsssecret)
    - [`Add-AzVmssSshPublicKey`](#add-azvmsssshpublickey)
    - [`Add-AzVmssWinRMListener`](#add-azvmsswinrmlistener)
    - [`New-AzVmssConfig`](#new-azvmssconfig)
    - [`Remove-AzVmssDataDisk`](#remove-azvmssdatadisk)
    - [`Remove-AzVmssExtension`](#remove-azvmssextension)
    - [`Remove-AzVmssNetworkInterfaceConfiguration`](#remove-azvmssnetworkinterfaceconfiguration)
    - [`Set-AzVmssBootDiagnostic`](#set-azvmssbootdiagnostic)
    - [`Set-AzVmssOsProfile`](#set-azvmssosprofile)
    - [`Set-AzVmssRollingUpgradePolicy`](#set-azvmssrollingupgradepolicy)
    - [`Set-AzVmssStorageProfile`](#set-azvmssstorageprofile)
    - [`New-AzVmss`](#new-azvmss)
    - [`Repair-AzVmssServiceFabricUpdateDomain`](#repair-azvmssservicefabricupdatedomain)
    - [`Get-AzVmss`](#get-azvmss)
    - [`Set-AzVmssOrchestrationServiceState`](#set-azvmssorchestrationservicestate)
    - [`Update-AzVmss`](#update-azvmss)
    - [`Add-AzVmssDiagnosticsExtension`](#add-azvmssdiagnosticsextension)
    - [`Disable-AzVmssDiskEncryption`](#disable-azvmssdiskencryption)
  - [<span data-ttu-id="2b3b9-110">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b3b9-110">Az.KeyVault</span></span>](#azkeyvault)
    - [`New-AzKeyVaultCertificateOrganizationDetail`](#new-azkeyvaultcertificateorganizationdetail)
    - [`New-AzKeyVaultCertificateAdministratorDetail`](#new-azkeyvaultcertificateadministratordetail)
    - [`New-AzKeyVault`](#new-azkeyvault)
  - [<span data-ttu-id="2b3b9-111">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b3b9-111">Az.Monitor</span></span>](#azmonitor)
    - [`Add-AzLogProfile`](#add-azlogprofile)
    - [`Get-AzLogProfile`](#get-azlogprofile)
    - [`New-AzMetricAlertRuleV2Criteria`](#new-azmetricalertrulev2criteria)
  - [<span data-ttu-id="2b3b9-112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b3b9-112">Az.Network</span></span>](#aznetwork)
    - [`Get-AzNetworkWatcherConnectionMonitor`](#get-aznetworkwatcherconnectionmonitor)
    - [`New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`](#new-aznetworkwatcherconnectionmonitortestconfigurationobject)
  - [<span data-ttu-id="2b3b9-113">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b3b9-113">Az.OperationalInsights</span></span>](#azoperationalinsights)
    - [`Get-AzOperationalInsightsDataSource`](#get-azoperationalinsightsdatasource)
    - [`New-AzOperationalInsightsApplicationInsightsDataSource`](#new-azoperationalinsightsapplicationinsightsdatasource)
    - [`New-AzOperationalInsightsAzureActivityLogDataSource`](#new-azoperationalinsightsazureactivitylogdatasource)
    - [`New-AzOperationalInsightsCustomLogDataSource`](#new-azoperationalinsightscustomlogdatasource)
    - [`New-AzOperationalInsightsLinuxPerformanceObjectDataSource`](#new-azoperationalinsightslinuxperformanceobjectdatasource)
    - [`New-AzOperationalInsightsLinuxSyslogDataSource`](#new-azoperationalinsightslinuxsyslogdatasource)
    - [`New-AzOperationalInsightsWindowsEventDataSource`](#new-azoperationalinsightswindowseventdatasource)
    - [`New-AzOperationalInsightsWindowsPerformanceCounterDataSource`](#new-azoperationalinsightswindowsperformancecounterdatasource)
    - [`Remove-AzOperationalInsightsDataSource`](#remove-azoperationalinsightsdatasource)
    - [`Disable-AzOperationalInsightsIISLogCollection`](#disable-azoperationalinsightsiislogcollection)
    - [`Disable-AzOperationalInsightsLinuxCustomLogCollection`](#disable-azoperationalinsightslinuxcustomlogcollection)
    - [`Disable-AzOperationalInsightsLinuxPerformanceCollection`](#disable-azoperationalinsightslinuxperformancecollection)
    - [`Disable-AzOperationalInsightsLinuxSyslogCollection`](#disable-azoperationalinsightslinuxsyslogcollection)
    - [`Enable-AzOperationalInsightsIISLogCollection`](#enable-azoperationalinsightsiislogcollection)
    - [`Enable-AzOperationalInsightsLinuxCustomLogCollection`](#enable-azoperationalinsightslinuxcustomlogcollection)
    - [`Enable-AzOperationalInsightsLinuxPerformanceCollection`](#enable-azoperationalinsightslinuxperformancecollection)
    - [`Enable-AzOperationalInsightsLinuxSyslogCollection`](#enable-azoperationalinsightslinuxsyslogcollection)
    - [`Get-AzOperationalInsightsSavedSearch`](#get-azoperationalinsightssavedsearch)
    - [`Get-AzOperationalInsightsSavedSearchResult`](#get-azoperationalinsightssavedsearchresult)
    - [`Get-AzOperationalInsightsSearchResult`](#get-azoperationalinsightssearchresult)
    - [`Get-AzOperationalInsightsStorageInsight`](#get-azoperationalinsightsstorageinsight)
    - [`New-AzOperationalInsightsStorageInsight`](#new-azoperationalinsightsstorageinsight)
    - [`Remove-AzOperationalInsightsStorageInsight`](#remove-azoperationalinsightsstorageinsight)
    - [`Set-AzOperationalInsightsStorageInsight`](#set-azoperationalinsightsstorageinsight)
    - [`Get-AzOperationalInsightsLinkTarget`](#get-azoperationalinsightslinktarget)
    - [`Get-AzOperationalInsightsWorkspace`](#get-azoperationalinsightsworkspace)
    - [`New-AzOperationalInsightsWorkspace`](#new-azoperationalinsightsworkspace)
    - [`Set-AzOperationalInsightsWorkspace`](#set-azoperationalinsightsworkspace)
    - [`Invoke-AzOperationalInsightsQuery`](#invoke-azoperationalinsightsquery)
  - [<span data-ttu-id="2b3b9-114">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b3b9-114">Az.Resources</span></span>](#azresources)
    - [`Get-AzDeploymentScript`](#get-azdeploymentscript)
    - [`Get-AzDeploymentScriptLog`](#get-azdeploymentscriptlog)
    - [`Save-AzDeploymentScriptLog`](#save-azdeploymentscriptlog)
    - [`Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`](#get-azresourcelock-new-azresourcelock-remove-azresourcelock-set-azresourcelock)
    - [`Get-AzPolicyAlias`](#get-azpolicyalias)
    - [`New-AzPolicyAssignment`](#new-azpolicyassignment)
    - [`Remove-AzDeploymentScript`](#remove-azdeploymentscript)
  - [<span data-ttu-id="2b3b9-115">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b3b9-115">Az.Storage</span></span>](#azstorage)
    - [<span data-ttu-id="2b3b9-116">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-116">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>](#update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset)
    - [<span data-ttu-id="2b3b9-117">`New-AzStorageTable`, `Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-117">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>](#new-azstoragetable-get-azstoragetable)
    - [<span data-ttu-id="2b3b9-118">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-118">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>](#get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy)
    - [<span data-ttu-id="2b3b9-119">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-119">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>](#get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory)
    - [<span data-ttu-id="2b3b9-120">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-120">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>](#get-azstorageshare-new-azstorageshare-remove-azstorageshare)
    - [`Set-AzStorageShareQuota`](#set-azstoragesharequota)
    - [`Remove-AzStorageDirectory`](#remove-azstoragedirectory)

## <a name="azapimanagement"></a><span data-ttu-id="2b3b9-121">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b3b9-121">Az.ApiManagement</span></span>

### `Add-AzApiManagementRegion`

<span data-ttu-id="2b3b9-122">O tipo de propriedade `Type` do tipo `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` foi alterado de `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` para `System.String`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-122">The type of property `Type` of type `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` has changed from `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` to `System.String`.</span></span>

### `New-AzApiManagement`

- <span data-ttu-id="2b3b9-123">O cmdlet `New-AzApiManagement` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-123">The cmdlet `New-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-124">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `New-AzApiManagement` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-124">The parameter set `__AllParameterSets` for cmdlet `New-AzApiManagement` has been removed.</span></span>

### `Set-AzApiManagement`

- <span data-ttu-id="2b3b9-125">O cmdlet `Set-AzApiManagement` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-125">The cmdlet `Set-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-126">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `Set-AzApiManagement` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-126">The parameter set `__AllParameterSets` for cmdlet `Set-AzApiManagement` has been removed.</span></span>

### `Get-AzApiManagementProperty`

<span data-ttu-id="2b3b9-127">O cmdlet `Get-AzApiManagementProperty` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-127">The cmdlet `Get-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

### `New-AzApiManagementProperty`

<span data-ttu-id="2b3b9-128">O cmdlet `New-AzApiManagementProperty` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-128">The cmdlet `New-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Remove-AzApiManagementProperty`

<span data-ttu-id="2b3b9-129">O cmdlet `Remove-AzApiManagementProperty` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-129">The cmdlet `Remove-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Set-AzApiManagementProperty`

<span data-ttu-id="2b3b9-130">O cmdlet `Set-AzApiManagementProperty` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-130">The cmdlet `Set-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

## <a name="azbatch"></a><span data-ttu-id="2b3b9-131">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b3b9-131">Az.Batch</span></span>

### <a name="get-azbatchapplication-new-azbatchapplication"></a><span data-ttu-id="2b3b9-132">`Get-AzBatchApplication`, `New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-132">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>

<span data-ttu-id="2b3b9-133">A propriedade `ApplicationPackages` do tipo `Microsoft.Azure.Commands.Batch.Models.PSApplication` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-133">The property `ApplicationPackages` of type `Microsoft.Azure.Commands.Batch.Models.PSApplication` has been removed.</span></span>

### <a name="get-azbatchcomputenode-new-azbatchpool"></a><span data-ttu-id="2b3b9-134">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-134">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>

<span data-ttu-id="2b3b9-135">A propriedade `PublicIPs` do tipo `Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-135">The property `PublicIPs` of type `Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` has been removed</span></span>

### <a name="get-azbatchapplicationpackage-new-azbatchapplicationpackage"></a><span data-ttu-id="2b3b9-136">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-136">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>

<span data-ttu-id="2b3b9-137">O tipo de propriedade `StorageUrlExpiry` do tipo `Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` foi alterado de `System.DateTime` para `System.DateTime?`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-137">The type of property `StorageUrlExpiry` of type `Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` has changed from `System.DateTime` to `System.DateTime?`.</span></span>

## <a name="azcompute"></a><span data-ttu-id="2b3b9-138">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b3b9-138">Az.Compute</span></span>

### `Remove-AzVmssDiagnosticsExtension`

<span data-ttu-id="2b3b9-139">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-139">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVMImage`

- <span data-ttu-id="2b3b9-140">O cmdlet `Get-AzVMImage` já não suporta o parâmetro `FilterExpression` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-140">The cmdlet `Get-AzVMImage` no longer supports the parameter `FilterExpression` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-141">O conjunto de parâmetros `ListVMImage` para o cmdlet `Get-AzVMImage` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-141">The parameter set `ListVMImage` for cmdlet `Get-AzVMImage` has been removed.</span></span>

### `New-AzVMConfig`

- <span data-ttu-id="2b3b9-142">O cmdlet `New-AzVMConfig` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-142">The cmdlet `New-AzVMConfig` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-143">O conjunto de parâmetros `AssignIdentityParameterSet` para o cmdlet `New-AzVMConfig` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-143">The parameter set `AssignIdentityParameterSet` for cmdlet `New-AzVMConfig` has been removed.</span></span>

### `Update-AzVM`

- <span data-ttu-id="2b3b9-144">O cmdlet `Update-AzVM` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-144">The cmdlet `Update-AzVM` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-145">O conjunto de parâmetros `AssignIdentityParameterSet` para o cmdlet `Update-AzVM` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-145">The parameter set `AssignIdentityParameterSet` for cmdlet `Update-AzVM` has been removed.</span></span>

### `New-AzProximityPlacementGroup`

- <span data-ttu-id="2b3b9-146">O tipo genérico da propriedade `VirtualMachines`, `VirtualMachineScaleSets` e `AvailabilitySets` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-146">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="2b3b9-147">As propriedades `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus` e `AvailabilitySetsColocationStatus` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-147">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-148">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-148">Before</span></span>

```powershell
PS C:\> New-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName -Location $location -Tag @{key1 = 'val1'} | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : Standard
VirtualMachinesColocationStatus         : {}
VirtualMachineScaleSetsColocationStatus : {}
AvailabilitySetsColocationStatus        : {}
ColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

#### <a name="after"></a><span data-ttu-id="2b3b9-149">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-149">After</span></span>

```powershell
PS C:\> New-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName -Location $location -Tag @{key1 = 'val1'} | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : StandardColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

### `Remove-AzProximityPlacementGroup`

- <span data-ttu-id="2b3b9-150">O tipo genérico da propriedade `VirtualMachines`, `VirtualMachineScaleSets` e `AvailabilitySets` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-150">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="2b3b9-151">As propriedades `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus` e `AvailabilitySetsColocationStatus` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-151">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-152">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-152">Before</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Remove-AzProximityPlacementGroup | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : Standard
VirtualMachinesColocationStatus         : {}
VirtualMachineScaleSetsColocationStatus : {}
AvailabilitySetsColocationStatus        : {}
ColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

#### <a name="after"></a><span data-ttu-id="2b3b9-153">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-153">After</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Remove-AzProximityPlacementGroup | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : StandardColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

### `Get-AzProximityPlacementGroup`

- <span data-ttu-id="2b3b9-154">O tipo genérico da propriedade `VirtualMachines`, `VirtualMachineScaleSets` e `AvailabilitySets` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-154">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="2b3b9-155">As propriedades `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus` e `AvailabilitySetsColocationStatus` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-155">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-156">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-156">Before</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : Standard
VirtualMachinesColocationStatus         : {}
VirtualMachineScaleSetsColocationStatus : {}
AvailabilitySetsColocationStatus        : {}
ColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

#### <a name="after"></a><span data-ttu-id="2b3b9-157">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-157">After</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : StandardColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

### `Add-AzVmssAdditionalUnattendContent`

<span data-ttu-id="2b3b9-158">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-158">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssDataDisk`

<span data-ttu-id="2b3b9-159">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-159">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssExtension`

<span data-ttu-id="2b3b9-160">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-160">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="2b3b9-161">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-161">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSecret`

<span data-ttu-id="2b3b9-162">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-162">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSshPublicKey`

<span data-ttu-id="2b3b9-163">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-163">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssWinRMListener`

<span data-ttu-id="2b3b9-164">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-164">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmssConfig`

- <span data-ttu-id="2b3b9-165">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-165">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="2b3b9-166">Já não suporta o parâmetro `AutomaticRepairMaxInstanceRepairsPercent` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-166">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-167">Já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-167">No longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-168">O conjunto de parâmetros `__AllParameterSets` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-168">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="2b3b9-169">O conjunto de parâmetros `ExplicitIdentityParameterSet` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-169">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>
- <span data-ttu-id="2b3b9-170">O conjunto de parâmetros `AssignIdentityParameterSet` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-170">The parameter set `AssignIdentityParameterSet` has been removed.</span></span>

### `Remove-AzVmssDataDisk`

<span data-ttu-id="2b3b9-171">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-171">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssExtension`

<span data-ttu-id="2b3b9-172">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-172">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="2b3b9-173">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-173">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssBootDiagnostic`

<span data-ttu-id="2b3b9-174">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-174">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOsProfile`

<span data-ttu-id="2b3b9-175">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-175">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssRollingUpgradePolicy`

<span data-ttu-id="2b3b9-176">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-176">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssStorageProfile`

<span data-ttu-id="2b3b9-177">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-177">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmss`

<span data-ttu-id="2b3b9-178">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-178">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Repair-AzVmssServiceFabricUpdateDomain`

<span data-ttu-id="2b3b9-179">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-179">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVmss`

<span data-ttu-id="2b3b9-180">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-180">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOrchestrationServiceState`

<span data-ttu-id="2b3b9-181">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-181">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Update-AzVmss`

- <span data-ttu-id="2b3b9-182">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-182">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="2b3b9-183">Já não suporta o parâmetro `AutomaticRepairMaxInstanceRepairsPercent` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-183">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-184">O conjunto de parâmetros `__AllParameterSets` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-184">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="2b3b9-185">O conjunto de parâmetros `ExplicitIdentityParameterSet` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-185">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>

### `Add-AzVmssDiagnosticsExtension`

<span data-ttu-id="2b3b9-186">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-186">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Disable-AzVmssDiskEncryption`

<span data-ttu-id="2b3b9-187">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-187">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

## <a name="azkeyvault"></a><span data-ttu-id="2b3b9-188">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b3b9-188">Az.KeyVault</span></span>

### `New-AzKeyVaultCertificateOrganizationDetail`

<span data-ttu-id="2b3b9-189">O alias `New-AzKeyVaultCertificateOrganizationDetails` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-189">The alias `New-AzKeyVaultCertificateOrganizationDetails` is removed.</span></span> <span data-ttu-id="2b3b9-190">Utilize `New-AzKeyVaultCertificateOrganizationDetail`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-190">Please use `New-AzKeyVaultCertificateOrganizationDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-191">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-191">Before</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetails -AdministratorDetails $AdminDetails
```

#### <a name="after"></a><span data-ttu-id="2b3b9-192">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-192">After</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetail -AdministratorDetails $AdminDetails
```

### `New-AzKeyVaultCertificateAdministratorDetail`

<span data-ttu-id="2b3b9-193">O alias `New-AzKeyVaultCertificateAdministratorDetails` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-193">The alias `New-AzKeyVaultCertificateAdministratorDetails` is removed.</span></span> <span data-ttu-id="2b3b9-194">Utilize `New-AzKeyVaultCertificateAdministratorDetail`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-194">Please use `New-AzKeyVaultCertificateAdministratorDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-195">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-195">Before</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetails -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

#### <a name="after"></a><span data-ttu-id="2b3b9-196">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-196">After</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetail -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

### `New-AzKeyVault`

<span data-ttu-id="2b3b9-197">`-EnableSoftDelete` é removido, uma vez que a eliminação recuperável está ativada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-197">`-EnableSoftDelete` is removed, as soft delete is enabled by default.</span></span> <span data-ttu-id="2b3b9-198">Se não pretender este comportamento, utilize `-DisableSoftDelete`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-198">Please use `-DisableSoftDelete` if you do not want this behavior.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-199">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-199">Before</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US' -EnableSoftDelete
```

#### <a name="after"></a><span data-ttu-id="2b3b9-200">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-200">After</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US'
```

## <a name="azmonitor"></a><span data-ttu-id="2b3b9-201">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b3b9-201">Az.Monitor</span></span>

### `Add-AzLogProfile`

<span data-ttu-id="2b3b9-202">O tipo de propriedade `RetentionPolicy` do tipo `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` foi alterado de `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` para `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-202">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `Get-AzLogProfile`

<span data-ttu-id="2b3b9-203">O tipo de propriedade `RetentionPolicy` do tipo `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` foi alterado de `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` para `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-203">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `New-AzMetricAlertRuleV2Criteria`

<span data-ttu-id="2b3b9-204">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `New-AzMetricAlertRuleV2Criteria` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-204">The parameter set `__AllParameterSets` for cmdlet `New-AzMetricAlertRuleV2Criteria` has been removed.</span></span>

## <a name="aznetwork"></a><span data-ttu-id="2b3b9-205">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b3b9-205">Az.Network</span></span>

### `Get-AzNetworkWatcherConnectionMonitor`

<span data-ttu-id="2b3b9-206">O tipo genérico da propriedade `RoundTripTimeMs` foi alterado de `System.Nullable1[System.Int32]` para `System.Nullable1[System.Double]`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-206">The generic type for property `RoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

### `New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`

<span data-ttu-id="2b3b9-207">O tipo genérico do parâmetro `SuccessThresholdRoundTripTimeMs` foi alterado de `System.Nullable1[System.Int32]` para `System.Nullable1[System.Double]`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-207">The generic type for parameter `SuccessThresholdRoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

## <a name="azoperationalinsights"></a><span data-ttu-id="2b3b9-208">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b3b9-208">Az.OperationalInsights</span></span>

### `Get-AzOperationalInsightsDataSource`

<span data-ttu-id="2b3b9-209">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-209">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsApplicationInsightsDataSource`

<span data-ttu-id="2b3b9-210">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-210">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsAzureActivityLogDataSource`

<span data-ttu-id="2b3b9-211">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-211">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsCustomLogDataSource`

<span data-ttu-id="2b3b9-212">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-212">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxPerformanceObjectDataSource`

<span data-ttu-id="2b3b9-213">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-213">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxSyslogDataSource`

<span data-ttu-id="2b3b9-214">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-214">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsEventDataSource`

<span data-ttu-id="2b3b9-215">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-215">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsPerformanceCounterDataSource`

<span data-ttu-id="2b3b9-216">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-216">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsDataSource`

<span data-ttu-id="2b3b9-217">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-217">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="2b3b9-218">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-218">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="2b3b9-219">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-219">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="2b3b9-220">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-220">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="2b3b9-221">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-221">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="2b3b9-222">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-222">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="2b3b9-223">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-223">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="2b3b9-224">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-224">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="2b3b9-225">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-225">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearch`

<span data-ttu-id="2b3b9-226">A propriedade `Metadata` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-226">The property `Metadata` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearchResult`

<span data-ttu-id="2b3b9-227">O cmdlet `Get-AzOperationalInsightsSavedSearchResult` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-227">The cmdlet `Get-AzOperationalInsightsSavedSearchResult` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Get-AzOperationalInsightsSearchResult`

<span data-ttu-id="2b3b9-228">O cmdlet `Get-AzOperationalInsightsSearchResult` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-228">The cmdlet `Get-AzOperationalInsightsSearchResult` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Get-AzOperationalInsightsStorageInsight`

<span data-ttu-id="2b3b9-229">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-229">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsStorageInsight`

<span data-ttu-id="2b3b9-230">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-230">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsStorageInsight`

<span data-ttu-id="2b3b9-231">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-231">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsStorageInsight`

<span data-ttu-id="2b3b9-232">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-232">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsLinkTarget`

<span data-ttu-id="2b3b9-233">O cmdlet `Get-AzOperationalInsightsLinkTarget` foi removido e não foi encontrado qualquer alias para o nome de cmdlet original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-233">The cmdlet `Get-AzOperationalInsightsLinkTarget` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Get-AzOperationalInsightsWorkspace`

<span data-ttu-id="2b3b9-234">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-234">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWorkspace`

- <span data-ttu-id="2b3b9-235">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-235">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>
- <span data-ttu-id="2b3b9-236">O cmdlet `New-AzOperationalInsightsWorkspace` já não suporta o parâmetro `CustomerId` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-236">The cmdlet `New-AzOperationalInsightsWorkspace` no longer supports the parameter `CustomerId` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="2b3b9-237">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `New-AzOperationalInsightsWorkspace` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-237">The parameter set `__AllParameterSets` for cmdlet `New-AzOperationalInsightsWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsWorkspace`

<span data-ttu-id="2b3b9-238">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-238">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Invoke-AzOperationalInsightsQuery`

<span data-ttu-id="2b3b9-239">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-239">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

## <a name="azresources"></a><span data-ttu-id="2b3b9-240">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b3b9-240">Az.Resources</span></span>

### `Get-AzDeploymentScript`

<span data-ttu-id="2b3b9-241">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-241">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzDeploymentScriptLog`

<span data-ttu-id="2b3b9-242">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-242">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Save-AzDeploymentScriptLog`

<span data-ttu-id="2b3b9-243">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-243">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`

<span data-ttu-id="2b3b9-244">O parâmetro `TenantLevel` foi removido.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-244">Parameter `TenantLevel` has been removed.</span></span>

### `Get-AzPolicyAlias`

<span data-ttu-id="2b3b9-245">O tipo genérico da propriedade `Aliases` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-245">The generic type for property `Aliases` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]`.</span></span>

### `New-AzPolicyAssignment`

- <span data-ttu-id="2b3b9-246">O cmdlet `New-AzPolicyAssignment` já não suporta o tipo `System.Management.Automation.PSObject` para o parâmetro `PolicyDefinition`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-246">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicyDefinition`.</span></span>
- <span data-ttu-id="2b3b9-247">O cmdlet `New-AzPolicyAssignment` já não suporta o tipo `System.Management.Automation.PSObject` para o parâmetro `PolicySetDefinition`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-247">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicySetDefinition`.</span></span>

### `Remove-AzDeploymentScript`

<span data-ttu-id="2b3b9-248">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-248">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

## <a name="azstorage"></a><span data-ttu-id="2b3b9-249">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b3b9-249">Az.Storage</span></span>

### <a name="update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset"></a><span data-ttu-id="2b3b9-250">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-250">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>

<span data-ttu-id="2b3b9-251">O valor de NetWorkRule DefaultAction foi alterado de: Permitir = 1, Recusar = 0, para: Permitir = 0, Recusar = 1.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-251">Changed NetWorkRule DefaultAction value from: Allow = 1, Deny = 0, to: Allow = 0, Deny = 1.</span></span>

### <a name="new-azstoragetable-get-azstoragetable"></a><span data-ttu-id="2b3b9-252">`New-AzStorageTable`, `Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-252">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>

<span data-ttu-id="2b3b9-253">Foram removidas duas propriedades ao objeto de saída AzureStorageTable.CloudTable.ServiceClient: ConnectionPolicy, ConsistencyLevel.</span><span class="sxs-lookup"><span data-stu-id="2b3b9-253">Output object AzureStorageTable.CloudTable.ServiceClient have 2 properties removed: ConnectionPolicy, ConsistencyLevel.</span></span>

### <a name="get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy"></a><span data-ttu-id="2b3b9-254">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-254">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>

<span data-ttu-id="2b3b9-255">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada "CloudFile" da saída nova</span><span class="sxs-lookup"><span data-stu-id="2b3b9-255">Change output type from CloudFile to AzureStorageFile, the original output will become child property "CloudFile" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-256">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-256">Before</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file
```

#### <a name="after"></a><span data-ttu-id="2b3b9-257">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-257">After</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file.CloudFile
```

### <a name="get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory"></a><span data-ttu-id="2b3b9-258">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-258">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>

<span data-ttu-id="2b3b9-259">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada "CloudFileDirectory" da saída nova</span><span class="sxs-lookup"><span data-stu-id="2b3b9-259">Change output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become child property "CloudFileDirectory" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-260">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-260">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="2b3b9-261">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-261">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```

### <a name="get-azstorageshare-new-azstorageshare-remove-azstorageshare"></a><span data-ttu-id="2b3b9-262">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="2b3b9-262">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>

<span data-ttu-id="2b3b9-263">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada "CloudFileShare" da saída nova</span><span class="sxs-lookup"><span data-stu-id="2b3b9-263">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become child property "CloudFileShare" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-264">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-264">Before</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share
```

#### <a name="after"></a><span data-ttu-id="2b3b9-265">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-265">After</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share.CloudFileShare
```

### `Set-AzStorageShareQuota`

<span data-ttu-id="2b3b9-266">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na subpropriedade subordinada "CloudFileShare.Properties" da saída nova</span><span class="sxs-lookup"><span data-stu-id="2b3b9-266">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become sub child property ""CloudFileShare.Properties"" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-267">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-267">Before</span></span>

```powershell
PS C:\> $shareProperties = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $shareProperties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

#### <a name="after"></a><span data-ttu-id="2b3b9-268">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-268">After</span></span>

```powershell
PS C:\> $share = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $share

   File End Point: https://weiors1.file.core.windows.net/

Name     QuotaGiB LastModified                IsSnapshot SnapshotTime
----     -------- ------------                ---------- ------------
weitest1 100      5/11/2020 3:03:30 PM +00:00 False

PS C:\> $share.CloudFileShare.Properties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

### `Remove-AzStorageDirectory`

<span data-ttu-id="2b3b9-269">Ao remover subdiretórios de ficheiros com objeto de diretório principal e -Path, já não é possível introduzir -Path a partir do pipeline com correspondência de tipo (cadeia).</span><span class="sxs-lookup"><span data-stu-id="2b3b9-269">When removing sub File Directories with parent Directory object and -Path, Can't input -Path from pipeline with type (string) match anymore.</span></span>

#### <a name="before"></a><span data-ttu-id="2b3b9-270">Antes</span><span class="sxs-lookup"><span data-stu-id="2b3b9-270">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> @('dir1', 'dir2') | Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="2b3b9-271">Depois</span><span class="sxs-lookup"><span data-stu-id="2b3b9-271">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> $paths = @(
    [PSCustomObject]@{  Path = 'dir1 }
    [PSCustomObject]@{ Path = 'dir2' }
)

PS C:\> $paths | Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```
