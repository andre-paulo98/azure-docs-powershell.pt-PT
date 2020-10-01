---
title: Guia de migração para o Az 4.1.0
description: Este guia de migração contém uma lista das alterações interruptivas feitas ao Azure PowerShell no lançamento da versão 4.1.0 do Az.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/23/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c64541beb5eb0d3db38932fb3915de865919641b
ms.sourcegitcommit: 5fcf17330d6f335561640a5ee3d98c59f7baab94
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/26/2020
ms.locfileid: "91381467"
---
# <a name="migration-guide-for-az-410"></a><span data-ttu-id="85fed-103">Guia de Migração para o Az 4.1.0</span><span class="sxs-lookup"><span data-stu-id="85fed-103">Migration Guide for Az 4.1.0</span></span>

<span data-ttu-id="85fed-104">Este documento descreve as alterações realizadas entre as versões 3.0.0 e 4.1.0 do Az.</span><span class="sxs-lookup"><span data-stu-id="85fed-104">This document describes the changes between the 3.0.0 and 4.1.0 versions of Az.</span></span>

- [<span data-ttu-id="85fed-105">Guia de migração para o Az 4.1.0</span><span class="sxs-lookup"><span data-stu-id="85fed-105">Migration Guide for Az 4.1.0</span></span>](#migration-guide-for-az-410)
  - [<span data-ttu-id="85fed-106">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="85fed-106">Az.ApiManagement</span></span>](#azapimanagement)
    - [`Add-AzApiManagementRegion`](#add-azapimanagementregion)
    - [`New-AzApiManagement`](#new-azapimanagement)
    - [`Set-AzApiManagement`](#set-azapimanagement)
    - [`Get-AzApiManagementProperty`](#get-azapimanagementproperty)
    - [`New-AzApiManagementProperty`](#new-azapimanagementproperty)
    - [`Remove-AzApiManagementProperty`](#remove-azapimanagementproperty)
    - [`Set-AzApiManagementProperty`](#set-azapimanagementproperty)
  - [<span data-ttu-id="85fed-107">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="85fed-107">Az.Batch</span></span>](#azbatch)
    - [<span data-ttu-id="85fed-108">`Get-AzBatchApplication`, `New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="85fed-108">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>](#get-azbatchapplication-new-azbatchapplication)
    - [<span data-ttu-id="85fed-109">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="85fed-109">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>](#get-azbatchcomputenode-new-azbatchpool)
    - [<span data-ttu-id="85fed-110">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="85fed-110">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>](#get-azbatchapplicationpackage-new-azbatchapplicationpackage)
  - [<span data-ttu-id="85fed-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="85fed-111">Az.Compute</span></span>](#azcompute)
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
  - [<span data-ttu-id="85fed-112">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="85fed-112">Az.KeyVault</span></span>](#azkeyvault)
    - [`New-AzKeyVaultCertificateOrganizationDetail`](#new-azkeyvaultcertificateorganizationdetail)
    - [`New-AzKeyVaultCertificateAdministratorDetail`](#new-azkeyvaultcertificateadministratordetail)
    - [`New-AzKeyVault`](#new-azkeyvault)
  - [<span data-ttu-id="85fed-113">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="85fed-113">Az.Monitor</span></span>](#azmonitor)
    - [`Add-AzLogProfile`](#add-azlogprofile)
    - [`Get-AzLogProfile`](#get-azlogprofile)
    - [`New-AzMetricAlertRuleV2Criteria`](#new-azmetricalertrulev2criteria)
  - [<span data-ttu-id="85fed-114">Az.Network</span><span class="sxs-lookup"><span data-stu-id="85fed-114">Az.Network</span></span>](#aznetwork)
    - [`Get-AzNetworkWatcherConnectionMonitor`](#get-aznetworkwatcherconnectionmonitor)
    - [`New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`](#new-aznetworkwatcherconnectionmonitortestconfigurationobject)
  - [<span data-ttu-id="85fed-115">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="85fed-115">Az.OperationalInsights</span></span>](#azoperationalinsights)
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
  - [<span data-ttu-id="85fed-116">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="85fed-116">Az.Resources</span></span>](#azresources)
    - [`Get-AzDeploymentScript`](#get-azdeploymentscript)
    - [`Get-AzDeploymentScriptLog`](#get-azdeploymentscriptlog)
    - [`Save-AzDeploymentScriptLog`](#save-azdeploymentscriptlog)
    - [`Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`](#get-azresourcelock-new-azresourcelock-remove-azresourcelock-set-azresourcelock)
    - [`Get-AzPolicyAlias`](#get-azpolicyalias)
    - [`New-AzPolicyAssignment`](#new-azpolicyassignment)
    - [`Remove-AzDeploymentScript`](#remove-azdeploymentscript)
  - [<span data-ttu-id="85fed-117">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="85fed-117">Az.Storage</span></span>](#azstorage)
    - [<span data-ttu-id="85fed-118">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="85fed-118">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>](#update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset)
    - [<span data-ttu-id="85fed-119">`New-AzStorageTable`, `Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="85fed-119">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>](#new-azstoragetable-get-azstoragetable)
    - [<span data-ttu-id="85fed-120">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="85fed-120">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>](#get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy)
    - [<span data-ttu-id="85fed-121">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="85fed-121">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>](#get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory)
    - [<span data-ttu-id="85fed-122">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="85fed-122">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>](#get-azstorageshare-new-azstorageshare-remove-azstorageshare)
    - [`Set-AzStorageShareQuota`](#set-azstoragesharequota)
    - [`Remove-AzStorageDirectory`](#remove-azstoragedirectory)

## <a name="azapimanagement"></a><span data-ttu-id="85fed-123">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="85fed-123">Az.ApiManagement</span></span>

### `Add-AzApiManagementRegion`

<span data-ttu-id="85fed-124">O tipo de propriedade `Type` do tipo `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` foi alterado de `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` para `System.String`.</span><span class="sxs-lookup"><span data-stu-id="85fed-124">The type of property `Type` of type `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` has changed from `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` to `System.String`.</span></span>

### `New-AzApiManagement`

- <span data-ttu-id="85fed-125">O cmdlet `New-AzApiManagement` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-125">The cmdlet `New-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-126">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `New-AzApiManagement` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-126">The parameter set `__AllParameterSets` for cmdlet `New-AzApiManagement` has been removed.</span></span>

### `Set-AzApiManagement`

- <span data-ttu-id="85fed-127">O cmdlet `Set-AzApiManagement` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-127">The cmdlet `Set-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-128">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `Set-AzApiManagement` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-128">The parameter set `__AllParameterSets` for cmdlet `Set-AzApiManagement` has been removed.</span></span>

### `Get-AzApiManagementProperty`

<span data-ttu-id="85fed-129">O cmdlet `Get-AzApiManagementProperty` foi substituído por `Get-AzApiManagementNamedValue`.</span><span class="sxs-lookup"><span data-stu-id="85fed-129">The cmdlet `Get-AzApiManagementProperty` has been replaced by `Get-AzApiManagementNamedValue`.</span></span>

### `New-AzApiManagementProperty`

<span data-ttu-id="85fed-130">O cmdlet `New-AzApiManagementProperty` foi substituído por `New-AzApiManagementNamedValue`.</span><span class="sxs-lookup"><span data-stu-id="85fed-130">The cmdlet `New-AzApiManagementProperty` has been replaced by `New-AzApiManagementNamedValue`.</span></span>

### `Remove-AzApiManagementProperty`

<span data-ttu-id="85fed-131">O cmdlet `Remove-AzApiManagementProperty` foi substituído por `Remove-AzApiManagementNamedValue`.</span><span class="sxs-lookup"><span data-stu-id="85fed-131">The cmdlet `Remove-AzApiManagementProperty` has been replaced by `Remove-AzApiManagementNamedValue`.</span></span>

### `Set-AzApiManagementProperty`

<span data-ttu-id="85fed-132">O cmdlet `Set-AzApiManagementProperty` foi substituído por `Set-AzApiManagementNamedValue`.</span><span class="sxs-lookup"><span data-stu-id="85fed-132">The cmdlet `Set-AzApiManagementProperty` has been replaced by `Set-AzApiManagementNamedValue`.</span></span>

## <a name="azbatch"></a><span data-ttu-id="85fed-133">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="85fed-133">Az.Batch</span></span>

### <a name="get-azbatchapplication-new-azbatchapplication"></a><span data-ttu-id="85fed-134">`Get-AzBatchApplication`, `New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="85fed-134">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>

<span data-ttu-id="85fed-135">A propriedade `ApplicationPackages` do tipo `Microsoft.Azure.Commands.Batch.Models.PSApplication` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-135">The property `ApplicationPackages` of type `Microsoft.Azure.Commands.Batch.Models.PSApplication` has been removed.</span></span>

### <a name="get-azbatchcomputenode-new-azbatchpool"></a><span data-ttu-id="85fed-136">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="85fed-136">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>

<span data-ttu-id="85fed-137">A propriedade `PublicIPs` do tipo `Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-137">The property `PublicIPs` of type `Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` has been removed</span></span>

### <a name="get-azbatchapplicationpackage-new-azbatchapplicationpackage"></a><span data-ttu-id="85fed-138">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="85fed-138">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>

<span data-ttu-id="85fed-139">O tipo de propriedade `StorageUrlExpiry` do tipo `Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` foi alterado de `System.DateTime` para `System.DateTime?`.</span><span class="sxs-lookup"><span data-stu-id="85fed-139">The type of property `StorageUrlExpiry` of type `Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` has changed from `System.DateTime` to `System.DateTime?`.</span></span>

## <a name="azcompute"></a><span data-ttu-id="85fed-140">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="85fed-140">Az.Compute</span></span>

### `Remove-AzVmssDiagnosticsExtension`

<span data-ttu-id="85fed-141">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-141">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVMImage`

- <span data-ttu-id="85fed-142">O cmdlet `Get-AzVMImage` já não suporta o parâmetro `FilterExpression` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-142">The cmdlet `Get-AzVMImage` no longer supports the parameter `FilterExpression` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-143">O conjunto de parâmetros `ListVMImage` para o cmdlet `Get-AzVMImage` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-143">The parameter set `ListVMImage` for cmdlet `Get-AzVMImage` has been removed.</span></span>

### `New-AzVMConfig`

- <span data-ttu-id="85fed-144">O cmdlet `New-AzVMConfig` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-144">The cmdlet `New-AzVMConfig` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-145">O conjunto de parâmetros `AssignIdentityParameterSet` para o cmdlet `New-AzVMConfig` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-145">The parameter set `AssignIdentityParameterSet` for cmdlet `New-AzVMConfig` has been removed.</span></span>

### `Update-AzVM`

- <span data-ttu-id="85fed-146">O cmdlet `Update-AzVM` já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-146">The cmdlet `Update-AzVM` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-147">O conjunto de parâmetros `AssignIdentityParameterSet` para o cmdlet `Update-AzVM` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-147">The parameter set `AssignIdentityParameterSet` for cmdlet `Update-AzVM` has been removed.</span></span>

### `New-AzProximityPlacementGroup`

- <span data-ttu-id="85fed-148">O tipo genérico da propriedade `VirtualMachines`, `VirtualMachineScaleSets` e `AvailabilitySets` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span><span class="sxs-lookup"><span data-stu-id="85fed-148">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="85fed-149">As propriedades `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus` e `AvailabilitySetsColocationStatus` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="85fed-149">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-150">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-150">Before</span></span>

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

#### <a name="after"></a><span data-ttu-id="85fed-151">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-151">After</span></span>

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

- <span data-ttu-id="85fed-152">O tipo genérico da propriedade `VirtualMachines`, `VirtualMachineScaleSets` e `AvailabilitySets` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span><span class="sxs-lookup"><span data-stu-id="85fed-152">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="85fed-153">As propriedades `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus` e `AvailabilitySetsColocationStatus` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="85fed-153">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-154">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-154">Before</span></span>

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

#### <a name="after"></a><span data-ttu-id="85fed-155">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-155">After</span></span>

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

- <span data-ttu-id="85fed-156">O tipo genérico da propriedade `VirtualMachines`, `VirtualMachineScaleSets` e `AvailabilitySets` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span><span class="sxs-lookup"><span data-stu-id="85fed-156">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="85fed-157">As propriedades `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus` e `AvailabilitySetsColocationStatus` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` foram removidas.</span><span class="sxs-lookup"><span data-stu-id="85fed-157">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-158">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-158">Before</span></span>

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

#### <a name="after"></a><span data-ttu-id="85fed-159">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-159">After</span></span>

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

<span data-ttu-id="85fed-160">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-160">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssDataDisk`

<span data-ttu-id="85fed-161">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-161">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssExtension`

<span data-ttu-id="85fed-162">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-162">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="85fed-163">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-163">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSecret`

<span data-ttu-id="85fed-164">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-164">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSshPublicKey`

<span data-ttu-id="85fed-165">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-165">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssWinRMListener`

<span data-ttu-id="85fed-166">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-166">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmssConfig`

- <span data-ttu-id="85fed-167">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-167">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="85fed-168">Já não suporta o parâmetro `AutomaticRepairMaxInstanceRepairsPercent` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-168">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-169">Já não suporta o parâmetro `AssignIdentity` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-169">No longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-170">O conjunto de parâmetros `__AllParameterSets` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-170">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="85fed-171">O conjunto de parâmetros `ExplicitIdentityParameterSet` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-171">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>
- <span data-ttu-id="85fed-172">O conjunto de parâmetros `AssignIdentityParameterSet` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-172">The parameter set `AssignIdentityParameterSet` has been removed.</span></span>

### `Remove-AzVmssDataDisk`

<span data-ttu-id="85fed-173">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-173">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssExtension`

<span data-ttu-id="85fed-174">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-174">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="85fed-175">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-175">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssBootDiagnostic`

<span data-ttu-id="85fed-176">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-176">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOsProfile`

<span data-ttu-id="85fed-177">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-177">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssRollingUpgradePolicy`

<span data-ttu-id="85fed-178">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-178">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssStorageProfile`

<span data-ttu-id="85fed-179">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-179">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmss`

<span data-ttu-id="85fed-180">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-180">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Repair-AzVmssServiceFabricUpdateDomain`

<span data-ttu-id="85fed-181">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-181">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVmss`

<span data-ttu-id="85fed-182">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-182">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOrchestrationServiceState`

<span data-ttu-id="85fed-183">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-183">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Update-AzVmss`

- <span data-ttu-id="85fed-184">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-184">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="85fed-185">Já não suporta o parâmetro `AutomaticRepairMaxInstanceRepairsPercent` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-185">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-186">O conjunto de parâmetros `__AllParameterSets` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-186">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="85fed-187">O conjunto de parâmetros `ExplicitIdentityParameterSet` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-187">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>

### `Add-AzVmssDiagnosticsExtension`

<span data-ttu-id="85fed-188">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-188">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Disable-AzVmssDiskEncryption`

<span data-ttu-id="85fed-189">O tipo de propriedade `AutomaticRepairsPolicy` do tipo `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` foi alterado de `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` para `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-189">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

## <a name="azkeyvault"></a><span data-ttu-id="85fed-190">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="85fed-190">Az.KeyVault</span></span>

### `New-AzKeyVaultCertificateOrganizationDetail`

<span data-ttu-id="85fed-191">O alias `New-AzKeyVaultCertificateOrganizationDetails` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-191">The alias `New-AzKeyVaultCertificateOrganizationDetails` is removed.</span></span> <span data-ttu-id="85fed-192">Utilize `New-AzKeyVaultCertificateOrganizationDetail`.</span><span class="sxs-lookup"><span data-stu-id="85fed-192">Please use `New-AzKeyVaultCertificateOrganizationDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-193">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-193">Before</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetails -AdministratorDetails $AdminDetails
```

#### <a name="after"></a><span data-ttu-id="85fed-194">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-194">After</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetail -AdministratorDetails $AdminDetails
```

### `New-AzKeyVaultCertificateAdministratorDetail`

<span data-ttu-id="85fed-195">O alias `New-AzKeyVaultCertificateAdministratorDetails` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-195">The alias `New-AzKeyVaultCertificateAdministratorDetails` is removed.</span></span> <span data-ttu-id="85fed-196">Utilize `New-AzKeyVaultCertificateAdministratorDetail`.</span><span class="sxs-lookup"><span data-stu-id="85fed-196">Please use `New-AzKeyVaultCertificateAdministratorDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-197">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-197">Before</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetails -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

#### <a name="after"></a><span data-ttu-id="85fed-198">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-198">After</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetail -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

### `New-AzKeyVault`

<span data-ttu-id="85fed-199">`-EnableSoftDelete` é removido, uma vez que a eliminação recuperável está ativada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="85fed-199">`-EnableSoftDelete` is removed, as soft delete is enabled by default.</span></span> <span data-ttu-id="85fed-200">Se não pretender este comportamento, utilize `-DisableSoftDelete`.</span><span class="sxs-lookup"><span data-stu-id="85fed-200">Please use `-DisableSoftDelete` if you do not want this behavior.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-201">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-201">Before</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US' -EnableSoftDelete
```

#### <a name="after"></a><span data-ttu-id="85fed-202">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-202">After</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US'
```

## <a name="azmonitor"></a><span data-ttu-id="85fed-203">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="85fed-203">Az.Monitor</span></span>

### `Add-AzLogProfile`

<span data-ttu-id="85fed-204">O tipo de propriedade `RetentionPolicy` do tipo `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` foi alterado de `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` para `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-204">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `Get-AzLogProfile`

<span data-ttu-id="85fed-205">O tipo de propriedade `RetentionPolicy` do tipo `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` foi alterado de `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` para `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span><span class="sxs-lookup"><span data-stu-id="85fed-205">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `New-AzMetricAlertRuleV2Criteria`

<span data-ttu-id="85fed-206">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `New-AzMetricAlertRuleV2Criteria` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-206">The parameter set `__AllParameterSets` for cmdlet `New-AzMetricAlertRuleV2Criteria` has been removed.</span></span>

## <a name="aznetwork"></a><span data-ttu-id="85fed-207">Az.Network</span><span class="sxs-lookup"><span data-stu-id="85fed-207">Az.Network</span></span>

### `Get-AzNetworkWatcherConnectionMonitor`

<span data-ttu-id="85fed-208">O tipo genérico da propriedade `RoundTripTimeMs` foi alterado de `System.Nullable1[System.Int32]` para `System.Nullable1[System.Double]`.</span><span class="sxs-lookup"><span data-stu-id="85fed-208">The generic type for property `RoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

### `New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`

<span data-ttu-id="85fed-209">O tipo genérico do parâmetro `SuccessThresholdRoundTripTimeMs` foi alterado de `System.Nullable1[System.Int32]` para `System.Nullable1[System.Double]`.</span><span class="sxs-lookup"><span data-stu-id="85fed-209">The generic type for parameter `SuccessThresholdRoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

## <a name="azoperationalinsights"></a><span data-ttu-id="85fed-210">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="85fed-210">Az.OperationalInsights</span></span>

### `Get-AzOperationalInsightsDataSource`

<span data-ttu-id="85fed-211">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-211">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsApplicationInsightsDataSource`

<span data-ttu-id="85fed-212">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-212">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsAzureActivityLogDataSource`

<span data-ttu-id="85fed-213">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-213">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsCustomLogDataSource`

<span data-ttu-id="85fed-214">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-214">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxPerformanceObjectDataSource`

<span data-ttu-id="85fed-215">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-215">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxSyslogDataSource`

<span data-ttu-id="85fed-216">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-216">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsEventDataSource`

<span data-ttu-id="85fed-217">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-217">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsPerformanceCounterDataSource`

<span data-ttu-id="85fed-218">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-218">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsDataSource`

<span data-ttu-id="85fed-219">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-219">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="85fed-220">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-220">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="85fed-221">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-221">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="85fed-222">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-222">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="85fed-223">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-223">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="85fed-224">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-224">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="85fed-225">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-225">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="85fed-226">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-226">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="85fed-227">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-227">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearch`

<span data-ttu-id="85fed-228">A propriedade `Metadata` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-228">The property `Metadata` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearchResult`

<span data-ttu-id="85fed-229">O cmdlet `Get-AzOperationalInsightsSavedSearchResult` deixou de ser suportado pelo SDK e foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-229">The cmdlet `Get-AzOperationalInsightsSavedSearchResult` was not supported by SDK anymore and has been removed.</span></span>

### `Get-AzOperationalInsightsSearchResult`

<span data-ttu-id="85fed-230">O cmdlet `Get-AzOperationalInsightsSearchResult` deixou de ser suportado pelo SDK e foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-230">The cmdlet `Get-AzOperationalInsightsSearchResult` was not supported by SDK anymore and has been removed.</span></span>

### `Get-AzOperationalInsightsStorageInsight`

<span data-ttu-id="85fed-231">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-231">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsStorageInsight`

<span data-ttu-id="85fed-232">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-232">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsStorageInsight`

<span data-ttu-id="85fed-233">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-233">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsStorageInsight`

<span data-ttu-id="85fed-234">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-234">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsLinkTarget`

<span data-ttu-id="85fed-235">O cmdlet `Get-AzOperationalInsightsLinkTarget` deixou de ser suportado pelo SDK e foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-235">The cmdlet `Get-AzOperationalInsightsLinkTarget` was not supported by SDK anymore and has been removed.</span></span>

### `Get-AzOperationalInsightsWorkspace`

<span data-ttu-id="85fed-236">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-236">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWorkspace`

- <span data-ttu-id="85fed-237">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-237">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>
- <span data-ttu-id="85fed-238">O cmdlet `New-AzOperationalInsightsWorkspace` já não suporta o parâmetro `CustomerId` e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="85fed-238">The cmdlet `New-AzOperationalInsightsWorkspace` no longer supports the parameter `CustomerId` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="85fed-239">O conjunto de parâmetros `__AllParameterSets` para o cmdlet `New-AzOperationalInsightsWorkspace` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-239">The parameter set `__AllParameterSets` for cmdlet `New-AzOperationalInsightsWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsWorkspace`

<span data-ttu-id="85fed-240">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-240">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Invoke-AzOperationalInsightsQuery`

<span data-ttu-id="85fed-241">A propriedade `PortalUrl` do tipo `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` foi removida.</span><span class="sxs-lookup"><span data-stu-id="85fed-241">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

## <a name="azresources"></a><span data-ttu-id="85fed-242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="85fed-242">Az.Resources</span></span>

### `Get-AzDeploymentScript`

<span data-ttu-id="85fed-243">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="85fed-243">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzDeploymentScriptLog`

<span data-ttu-id="85fed-244">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="85fed-244">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Save-AzDeploymentScriptLog`

<span data-ttu-id="85fed-245">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="85fed-245">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`

<span data-ttu-id="85fed-246">O parâmetro `TenantLevel` foi removido.</span><span class="sxs-lookup"><span data-stu-id="85fed-246">Parameter `TenantLevel` has been removed.</span></span>

### `Get-AzPolicyAlias`

<span data-ttu-id="85fed-247">O tipo genérico da propriedade `Aliases` foi alterado de `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` para `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]`.</span><span class="sxs-lookup"><span data-stu-id="85fed-247">The generic type for property `Aliases` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]`.</span></span>

### `New-AzPolicyAssignment`

- <span data-ttu-id="85fed-248">O cmdlet `New-AzPolicyAssignment` já não suporta o tipo `System.Management.Automation.PSObject` para o parâmetro `PolicyDefinition`.</span><span class="sxs-lookup"><span data-stu-id="85fed-248">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicyDefinition`.</span></span>
- <span data-ttu-id="85fed-249">O cmdlet `New-AzPolicyAssignment` já não suporta o tipo `System.Management.Automation.PSObject` para o parâmetro `PolicySetDefinition`.</span><span class="sxs-lookup"><span data-stu-id="85fed-249">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicySetDefinition`.</span></span>

### `Remove-AzDeploymentScript`

<span data-ttu-id="85fed-250">O tipo de propriedade `Status` do tipo `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` foi alterado de `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` para `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span><span class="sxs-lookup"><span data-stu-id="85fed-250">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

## <a name="azstorage"></a><span data-ttu-id="85fed-251">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="85fed-251">Az.Storage</span></span>

### <a name="update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset"></a><span data-ttu-id="85fed-252">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="85fed-252">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>

<span data-ttu-id="85fed-253">O valor de NetWorkRule DefaultAction foi alterado de: Permitir = 1, Recusar = 0, para: Permitir = 0, Recusar = 1.</span><span class="sxs-lookup"><span data-stu-id="85fed-253">Changed NetWorkRule DefaultAction value from: Allow = 1, Deny = 0, to: Allow = 0, Deny = 1.</span></span>

### <a name="new-azstoragetable-get-azstoragetable"></a><span data-ttu-id="85fed-254">`New-AzStorageTable`, `Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="85fed-254">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>

<span data-ttu-id="85fed-255">Foram removidas duas propriedades ao objeto de saída AzureStorageTable.CloudTable.ServiceClient: ConnectionPolicy, ConsistencyLevel.</span><span class="sxs-lookup"><span data-stu-id="85fed-255">Output object AzureStorageTable.CloudTable.ServiceClient have 2 properties removed: ConnectionPolicy, ConsistencyLevel.</span></span>

### <a name="get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy"></a><span data-ttu-id="85fed-256">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="85fed-256">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>

<span data-ttu-id="85fed-257">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada "CloudFile" da saída nova</span><span class="sxs-lookup"><span data-stu-id="85fed-257">Change output type from CloudFile to AzureStorageFile, the original output will become child property "CloudFile" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-258">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-258">Before</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file
```

#### <a name="after"></a><span data-ttu-id="85fed-259">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-259">After</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file.CloudFile
```

### <a name="get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory"></a><span data-ttu-id="85fed-260">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="85fed-260">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>

<span data-ttu-id="85fed-261">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada "CloudFileDirectory" da saída nova</span><span class="sxs-lookup"><span data-stu-id="85fed-261">Change output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become child property "CloudFileDirectory" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-262">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-262">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="85fed-263">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-263">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```

### <a name="get-azstorageshare-new-azstorageshare-remove-azstorageshare"></a><span data-ttu-id="85fed-264">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="85fed-264">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>

<span data-ttu-id="85fed-265">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada "CloudFileShare" da saída nova</span><span class="sxs-lookup"><span data-stu-id="85fed-265">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become child property "CloudFileShare" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-266">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-266">Before</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share
```

#### <a name="after"></a><span data-ttu-id="85fed-267">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-267">After</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share.CloudFileShare
```

### `Set-AzStorageShareQuota`

<span data-ttu-id="85fed-268">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na subpropriedade subordinada "CloudFileShare.Properties" da saída nova</span><span class="sxs-lookup"><span data-stu-id="85fed-268">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become sub child property ""CloudFileShare.Properties"" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-269">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-269">Before</span></span>

```powershell
PS C:\> $shareProperties = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $shareProperties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

#### <a name="after"></a><span data-ttu-id="85fed-270">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-270">After</span></span>

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

<span data-ttu-id="85fed-271">Ao remover subdiretórios de ficheiros com objeto de diretório principal e -Path, já não é possível introduzir -Path a partir do pipeline com correspondência de tipo (cadeia).</span><span class="sxs-lookup"><span data-stu-id="85fed-271">When removing sub File Directories with parent Directory object and -Path, Can't input -Path from pipeline with type (string) match anymore.</span></span>

#### <a name="before"></a><span data-ttu-id="85fed-272">Antes</span><span class="sxs-lookup"><span data-stu-id="85fed-272">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> @('dir1', 'dir2') | Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="85fed-273">Depois</span><span class="sxs-lookup"><span data-stu-id="85fed-273">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> $paths = @(
    [PSCustomObject]@{  Path = 'dir1 }
    [PSCustomObject]@{ Path = 'dir2' }
)

PS C:\> $paths | Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```
