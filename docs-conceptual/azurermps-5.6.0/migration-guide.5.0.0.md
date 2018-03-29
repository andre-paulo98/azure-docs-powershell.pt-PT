# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a><span data-ttu-id="2a2c7-101">Alterações recentes ao Microsoft Azure PowerShell 5.0.0</span><span class="sxs-lookup"><span data-stu-id="2a2c7-101">Breaking changes for Microsoft Azure PowerShell 5.0.0</span></span>

<span data-ttu-id="2a2c7-102">Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="2a2c7-103">Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="2a2c7-104">Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="2a2c7-105">Índice</span><span class="sxs-lookup"><span data-stu-id="2a2c7-105">Table of Contents</span></span>

- [<span data-ttu-id="2a2c7-106">Alterações recentes aos cmdlets de ApiManagement </span><span class="sxs-lookup"><span data-stu-id="2a2c7-106">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
- [<span data-ttu-id="2a2c7-107">Alterações recentes aos cmdlets de Batch</span><span class="sxs-lookup"><span data-stu-id="2a2c7-107">Breaking changes to Batch cmdlets</span></span>](#breaking-changes-to-batch-cmdlets)
- [<span data-ttu-id="2a2c7-108">Alterações recentes aos cmdlets de Computação</span><span class="sxs-lookup"><span data-stu-id="2a2c7-108">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="2a2c7-109">Alterações recentes aos cmdlets de EventHub</span><span class="sxs-lookup"><span data-stu-id="2a2c7-109">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="2a2c7-110">Alterações recentes aos cmdlets de Insights</span><span class="sxs-lookup"><span data-stu-id="2a2c7-110">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="2a2c7-111">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="2a2c7-111">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="2a2c7-112">Alterações recentes aos cmdlets de Recursos</span><span class="sxs-lookup"><span data-stu-id="2a2c7-112">Breaking changes to Resources cmdlets</span></span>](#breaking-changes-to-resources-cmdlets)
- [<span data-ttu-id="2a2c7-113">Alterações recentes aos cmdlets de ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2a2c7-113">Breaking Changes to ServiceBus Cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="2a2c7-114">Alterações recentes aos cmdlets de ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2a2c7-114">Breaking changes to ApiManagement cmdlets</span></span>

### <a name="new-azurermapimanagementbackendproxy"></a><span data-ttu-id="2a2c7-115">**New-AzureRmApiManagementBackendProxy**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-115">**New-AzureRmApiManagementBackendProxy**</span></span>
- <span data-ttu-id="2a2c7-116">Os parâmetros "UserName" e "Password" estão a ser substituídos em prol de uma PSCredential</span><span class="sxs-lookup"><span data-stu-id="2a2c7-116">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a><span data-ttu-id="2a2c7-117">**New-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-117">**New-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="2a2c7-118">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-118">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a><span data-ttu-id="2a2c7-119">**Set-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-119">**Set-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="2a2c7-120">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-120">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a><span data-ttu-id="2a2c7-121">Alterações recentes aos cmdlets de Batch</span><span class="sxs-lookup"><span data-stu-id="2a2c7-121">Breaking changes to Batch cmdlets</span></span>

### <a name="new-azurebatchcertificate"></a><span data-ttu-id="2a2c7-122">**New-AzureBatchCertificate**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-122">**New-AzureBatchCertificate**</span></span>
- <span data-ttu-id="2a2c7-123">O parâmetro `Password` está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-123">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a><span data-ttu-id="2a2c7-124">**New-AzureBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-124">**New-AzureBatchComputeNodeUser**</span></span>
- <span data-ttu-id="2a2c7-125">O parâmetro `Password` está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-125">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a><span data-ttu-id="2a2c7-126">**Set-AzureRmBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-126">**Set-AzureRmBatchComputeNodeUser**</span></span>
- <span data-ttu-id="2a2c7-127">O parâmetro `Password` está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-127">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a><span data-ttu-id="2a2c7-128">**New-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-128">**New-AzureBatchTask**</span></span>
 - <span data-ttu-id="2a2c7-129">O parâmetro `RunElevated` foi removido e substituído por `UserIdentity`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-129">Removed the `RunElevated` switch and replaced it with `UserIdentity`.</span></span>

```powershell
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

<span data-ttu-id="2a2c7-130">Esta alteração também afeta a propriedade `RunElevated` em `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` e `PSJobReleaseTask`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-130">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="psmultiinstancesettings"></a><span data-ttu-id="2a2c7-131">**PSMultiInstanceSettings**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-131">**PSMultiInstanceSettings**</span></span>

- <span data-ttu-id="2a2c7-132">O construtor `PSMultiInstanceSettings` já não precisa de um parâmetro `numberOfInstances` obrigatório. Em vez disso, precisa de um parâmetro `coordinationCommandLine` obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-132">`PSMultiInstanceSettings` constructor no longer takes a required `numberOfInstances` parameter, instead it takes a required `coordinationCommandLine` parameter.</span></span>

```powershell
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a><span data-ttu-id="2a2c7-133">**Get-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-133">**Get-AzureBatchTask**</span></span>
 - <span data-ttu-id="2a2c7-134">A propriedade `RunElevated` foi removida em `PSCloudTask`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-134">Removed the `RunElevated` property on `PSCloudTask`.</span></span> <span data-ttu-id="2a2c7-135">A propriedade `UserIdentity` foi adicionada para substituir `RunElevated`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-135">The `UserIdentity` property has been added to replace `RunElevated`.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

<span data-ttu-id="2a2c7-136">Esta alteração também afeta a propriedade `RunElevated` em `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` e `PSJobReleaseTask`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-136">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="multiple-types"></a><span data-ttu-id="2a2c7-137">**Vários tipos**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-137">**Multiple types**</span></span>

- <span data-ttu-id="2a2c7-138">O nome da propriedade `SchedulingError` foi mudado em `PSExitConditions` para `PreProcessingError`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-138">Renamed the `SchedulingError` property on `PSExitConditions` to `PreProcessingError`.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a><span data-ttu-id="2a2c7-139">**Vários tipos**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-139">**Multiple types**</span></span>

- <span data-ttu-id="2a2c7-140">O nome da propriedade `SchedulingError` foi mudado em `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation` e `PSTaskExecutionInformation` para `FailureInformation`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-140">Renamed the `SchedulingError` property on `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation`, and `PSTaskExecutionInformation` to `FailureInformation`.</span></span>
  - <span data-ttu-id="2a2c7-141">`FailureInformation` é devolvido sempre que ocorre uma falha de tarefa.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-141">`FailureInformation` is returned any time there is a task failure.</span></span> <span data-ttu-id="2a2c7-142">Isto inclui todos os casos de erro de agendamento anteriores, bem como os códigos de saída de tarefa diferentes de zero e falhas de carregamento de ficheiros da nova funcionalidade de ficheiros de saída.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-142">This includes all previous scheduling error cases, as well as nonzero task exit codes, and file upload failures from the new output files feature.</span></span>
  - <span data-ttu-id="2a2c7-143">A estrutura continua igual à utilizada anteriormente, pelo que não é necessário efetuar qualquer alteração no código ao utilizar este tipo.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-143">This is structured the same as before, so no code change is needed when using this type.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

<span data-ttu-id="2a2c7-144">Esta alteração também afeta: Get-AzureBatchPool, Get-AzureBatchSubtask e Get-AzureBatchJobPreparationAndReleaseTaskStatus</span><span class="sxs-lookup"><span data-stu-id="2a2c7-144">This additionally impacts: Get-AzureBatchPool, Get-AzureBatchSubtask, and Get-AzureBatchJobPreparationAndReleaseTaskStatus</span></span>

### <a name="new-azurebatchpool"></a><span data-ttu-id="2a2c7-145">**New-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-145">**New-AzureBatchPool**</span></span>
 - <span data-ttu-id="2a2c7-146">`TargetDedicated` foi removido e substituído por `TargetDedicatedComputeNodes` e `TargetLowPriorityComputeNodes`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-146">Removed `TargetDedicated` and replaced it with `TargetDedicatedComputeNodes` and `TargetLowPriorityComputeNodes`.</span></span>
 - <span data-ttu-id="2a2c7-147">`TargetDedicatedComputeNodes` tem um alias `TargetDedicated`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-147">`TargetDedicatedComputeNodes` has an alias `TargetDedicated`.</span></span>

```powershell
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

<span data-ttu-id="2a2c7-148">Esta alteração também afeta: Start-AzureBatchPoolResize</span><span class="sxs-lookup"><span data-stu-id="2a2c7-148">This also impacts: Start-AzureBatchPoolResize</span></span>

### <a name="get-azurebatchpool"></a><span data-ttu-id="2a2c7-149">**Get-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-149">**Get-AzureBatchPool**</span></span>
 - <span data-ttu-id="2a2c7-150">O nome das propriedades `TargetDedicated` e `CurrentDedicated` foi mudado em `PSCloudPool` para `TargetDedicatedComputeNodes` e `CurrentDedicatedComputeNodes`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-150">Renamed the `TargetDedicated` and `CurrentDedicated` properties on `PSCloudPool` to `TargetDedicatedComputeNodes` and `CurrentDedicatedComputeNodes`.</span></span>

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicated
$pool.CurrentDedicated

# New
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicatedComputeNodes
$pool.CurrentDedicatedComputeNodes
```

### <a name="type-pscloudpool"></a><span data-ttu-id="2a2c7-151">**Tipo PSCloudPool**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-151">**Type PSCloudPool**</span></span>

- <span data-ttu-id="2a2c7-152">O nome de `ResizeError` foi mudado para `ResizeErrors` em `PSCloudPool` e é agora uma coleção.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-152">Renamed `ResizeError` to `ResizeErrors` on `PSCloudPool`, and it is now a collection.</span></span>

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a><span data-ttu-id="2a2c7-153">**New-AzureBatchJob**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-153">**New-AzureBatchJob**</span></span>
- <span data-ttu-id="2a2c7-154">O nome da propriedade `TargetDedicated` foi mudado em `PSPoolSpecification` para `TargetDedicatedComputeNodes`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-154">Renamed the `TargetDedicated` property on `PSPoolSpecification` to `TargetDedicatedComputeNodes`.</span></span>

```powershell
# Old
$poolInfo = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolInformation
$poolInfo.AutoPoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification.TargetDedicated = 5
New-AzureBatchJob [other parameters] -PoolInformation $poolInfo

# New
$poolInfo = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolInformation
$poolInfo.AutoPoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification.TargetDedicatedComputeNodes = 5
New-AzureBatchJob [other parameters] -PoolInformation $poolInfo
```

### <a name="get-azurebatchnodefile"></a><span data-ttu-id="2a2c7-155">**Get-AzureBatchNodeFile**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-155">**Get-AzureBatchNodeFile**</span></span>
 - <span data-ttu-id="2a2c7-156">`Name` foi removido e substituído por `Path`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-156">Removed `Name` and replaced it with `Path`.</span></span>
 - <span data-ttu-id="2a2c7-157">`Path` tem um alias `Name`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-157">`Path` has an alias `Name`.</span></span>

```powershell
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

<span data-ttu-id="2a2c7-158">Esta alteração também afeta: Get-AzureBatchNodeFileContent e Remove-AzureBatchNodeFile</span><span class="sxs-lookup"><span data-stu-id="2a2c7-158">This also impacts: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile</span></span>

### <a name="type-psnodefile"></a><span data-ttu-id="2a2c7-159">Tipo **PSNodeFile**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-159">Type **PSNodeFile**</span></span>

 - <span data-ttu-id="2a2c7-160">O nome da propriedade `Name` foi mudado em `PSNodeFile` para `Path`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-160">Renamed the `Name` property on `PSNodeFile` to `Path`.</span></span>

```powershell
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a><span data-ttu-id="2a2c7-161">**Get-AzureBatchSubtask**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-161">**Get-AzureBatchSubtask**</span></span>
- <span data-ttu-id="2a2c7-162">As propriedades `PreviousState` e `State` de `PSSubtaskInformation` já não são do tipo `TaskState`, sendo agora do tipo `SubtaskState`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-162">The `PreviousState` and `State` properties of `PSSubtaskInformation` are no longer of type `TaskState`, instead they are of type `SubtaskState`.</span></span>
  - <span data-ttu-id="2a2c7-163">Ao contrário de `TaskState`, `SubtaskState` não tem um valor `Active`, uma vez que as subtarefas não podem ter um estado `Active`.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-163">Unlike `TaskState`, `SubtaskState` has no `Active` value, since it is not possible for subtasks to be in an `Active` state.</span></span>

```powershell
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="2a2c7-164">Alterações recentes aos cmdlets de Computação</span><span class="sxs-lookup"><span data-stu-id="2a2c7-164">Breaking changes to Compute cmdlets</span></span>

### <a name="set-azurermvmaccessextension"></a><span data-ttu-id="2a2c7-165">**Set-AzureRmVMAccessExtension**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-165">**Set-AzureRmVMAccessExtension**</span></span>
- <span data-ttu-id="2a2c7-166">Os parâmetros "UserName" e "Password" estão a ser substituídos em prol de uma PSCredential</span><span class="sxs-lookup"><span data-stu-id="2a2c7-166">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="2a2c7-167">Alterações recentes aos cmdlets de EventHub</span><span class="sxs-lookup"><span data-stu-id="2a2c7-167">Breaking changes to EventHub cmdlets</span></span>

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-168">**New-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-168">**New-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-169">O cmdlet "New-AzureRmEventHubNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-169">The 'New-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-170">Utilize o cmdlet "New-AzureRmEventHubAuthorizationRule"</span><span class="sxs-lookup"><span data-stu-id="2a2c7-170">Please use the 'New-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-171">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-171">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-172">O cmdlet "Get-AzureRmEventHubNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-172">The 'Get-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-173">Utilize o cmdlet "Get-AzureRmEventHubAuthorizationRule"</span><span class="sxs-lookup"><span data-stu-id="2a2c7-173">Please use the 'Get-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-174">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-174">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-175">O cmdlet "Set-AzureRmEventHubNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-175">The 'Set-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-176">Utilize o cmdlet "Set-AzureRmEventHubAuthorizationRule"</span><span class="sxs-lookup"><span data-stu-id="2a2c7-176">Please use the 'Set-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-177">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-177">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-178">O cmdlet "Remove-AzureRmEventHubNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-178">The 'Remove-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-179">Utilize o cmdlet "Remove-AzureRmEventHubAuthorizationRule"</span><span class="sxs-lookup"><span data-stu-id="2a2c7-179">Please use the 'Remove-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespacekey"></a><span data-ttu-id="2a2c7-180">**New-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-180">**New-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="2a2c7-181">O cmdlet "New-AzureRmEventHubNamespaceKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-181">The 'New-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-182">Utilize o cmdlet "New-AzureRmEventHubKey"</span><span class="sxs-lookup"><span data-stu-id="2a2c7-182">Please use the 'New-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespacekey"></a><span data-ttu-id="2a2c7-183">**Get-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-183">**Get-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="2a2c7-184">O cmdlet "Get-AzureRmEventHubNamespaceKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-184">The 'Get-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-185">Utilize o cmdlet "Get-AzureRmEventHubKey"</span><span class="sxs-lookup"><span data-stu-id="2a2c7-185">Please use the 'Get-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="2a2c7-186">**New-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-186">**New-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="2a2c7-187">As propriedades "Status" e "Enabled" de NamespceAttributes irão ser removidas.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-187">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property  
$namespace = New-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="2a2c7-188">**Get-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-188">**Get-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="2a2c7-189">As propriedades "Status" e "Enabled" de NamespceAttributes irão ser removidas.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-189">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="set-azurermeventhubnamespace"></a><span data-ttu-id="2a2c7-190">**Set-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-190">**Set-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="2a2c7-191">As propriedades "Status" e "Enabled" de NamespceAttributes irão ser removidas.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-191">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Set-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Set-AzureRmEventHubNamespace <parameters>
``` 
  
### <a name="new-azurermeventhubconsumergroup"></a><span data-ttu-id="2a2c7-192">**New-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-192">**New-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="2a2c7-193">A propriedade "EventHubPath" de ConsumerGroupAttributes irá ser removida.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-193">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a><span data-ttu-id="2a2c7-194">**Set-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-194">**Set-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="2a2c7-195">A propriedade "EventHubPath" de ConsumerGroupAttributes irá ser removida.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-195">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a><span data-ttu-id="2a2c7-196">**Get-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-196">**Get-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="2a2c7-197">A propriedade "EventHubPath" de ConsumerGroupAttributes irá ser removida.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-197">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="2a2c7-198">Alterações recentes aos cmdlets de Insights</span><span class="sxs-lookup"><span data-stu-id="2a2c7-198">Breaking changes to Insights cmdlets</span></span>

### <a name="add-azurermlogalertrule"></a><span data-ttu-id="2a2c7-199">**Add-AzureRMLogAlertRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-199">**Add-AzureRMLogAlertRule**</span></span>
- <span data-ttu-id="2a2c7-200">O cmdlet **Add-AzureRMLogAlertRule** foi preterido</span><span class="sxs-lookup"><span data-stu-id="2a2c7-200">The **Add-AzureRMLogAlertRule** cmdlet has been deprecated</span></span>
- <span data-ttu-id="2a2c7-201">Após 1 de outubro, a utilização deste cmdlet já não terá qualquer efeito uma vez que esta funcionalidade está transitar para os Alertas de Registo de Atividade.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-201">After October 1st using this cmdlet will no longer have any effect as this functionality is being transitioned to Activity Log Alerts.</span></span> <span data-ttu-id="2a2c7-202">Para obter mais informações, veja https://aka.ms/migratemealerts.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-202">Please see https://aka.ms/migratemealerts for more information.</span></span>

### <a name="get-azurermusage"></a><span data-ttu-id="2a2c7-203">**Get-AzureRMUsage**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-203">**Get-AzureRMUsage**</span></span>
- <span data-ttu-id="2a2c7-204">O cmdlet **Get-AzureRMUsage** foi preterido</span><span class="sxs-lookup"><span data-stu-id="2a2c7-204">The **Get-AzureRMUsage** cmdlet has been deprecated</span></span>

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a><span data-ttu-id="2a2c7-205">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-205">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span></span>
- <span data-ttu-id="2a2c7-206">Alteração na saída: o campo EventChannels do objeto EventData (devolvido por estes cmdlets) está em vias de ser preterido visto que agora devolve um valor constante (Admin,Operation).</span><span class="sxs-lookup"><span data-stu-id="2a2c7-206">Output change: The field EventChannels from the EventData object (returned by these cmdlets) is being deprecated since it now returns a constant value (Admin,Operation.)</span></span>

### <a name="get-azurermalertrule"></a><span data-ttu-id="2a2c7-207">**Get-AzureRmAlertRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-207">**Get-AzureRmAlertRule**</span></span>
- <span data-ttu-id="2a2c7-208">Alteração na saída: a saída deste cmdlet irá ser simplificada, o que significa a eliminação do campo de propriedades, para melhorar a experiência do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-208">Output change: The output of this cmdlet will be flattened, i.e. elimination of the properties field, to improve the user experience.</span></span>

```powershell
# Old
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -Foreground Red "Error updating alert rule"
    Write-Host $rules[0].Id
    Write-Host $rules[0].Properties.IsEnabled
    Write-Host $rules[0].Properties.Condition
}

# New
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -Foreground red "Error updating alert rule"
    Write-Host $rules[0].Id

    # Properties will remain for a while
    Write-Host $rules[0].Properties.IsEnabled
      
    # But the properties will be at the top level too. Later Properties will be removed
    Write-Host $rules[0].IsEnabled
    Write-Host $rules[0].Condition
}
```

### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="2a2c7-209">**Get-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-209">**Get-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="2a2c7-210">Alteração na saída: o campo AutoscaleSettingResourceName irá ser preterido, uma vez que equivale sempre ao campo Name.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-210">Output change: The AutoscaleSettingResourceName field will be deprecated since it always equals the Name field.</span></span>

```powershell
# Old
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
if ($s1.AutoscaleSettingResourceName -ne $s1.Name)
{
    Write-Host "There is something wrong with the name"
}

# New
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
    
# there won't be a AutoscaleSettingResourceName
Write-Host $s1.Name    
```

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a><span data-ttu-id="2a2c7-211">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-211">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span></span>
- <span data-ttu-id="2a2c7-212">Alteração na saída: o tipo da saída irá ser alterado para devolver um único objeto que contém o ID do pedido e o código de estado.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-212">Output change: The type of the output will change to return a single object containing the request Id and the status code.</span></span>

```powershell
# Old
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name $ruleName
if ($s1 -ne $null)
{
    $r = $s1[0].RequestId
    $s = $s1[0].StatusCode
}

# New
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name $ruleName
$r = $s1.RequestId
$s = $s1.StatusCode
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="2a2c7-213">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="2a2c7-213">Breaking changes to Network cmdlets</span></span>

### <a name="add-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="2a2c7-214">**Add-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-214">**Add-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="2a2c7-215">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-215">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="2a2c7-216">**New-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-216">**New-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="2a2c7-217">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-217">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="2a2c7-218">**Set-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-218">**Set-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="2a2c7-219">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-219">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a><span data-ttu-id="2a2c7-220">Alterações recentes aos cmdlets de Recursos</span><span class="sxs-lookup"><span data-stu-id="2a2c7-220">Breaking changes to Resources cmdlets</span></span>

### <a name="new-azurermadappcredential"></a><span data-ttu-id="2a2c7-221">**New-AzureRmADAppCredential**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-221">**New-AzureRmADAppCredential**</span></span>
- <span data-ttu-id="2a2c7-222">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-222">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a><span data-ttu-id="2a2c7-223">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-223">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="2a2c7-224">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-224">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a><span data-ttu-id="2a2c7-225">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-225">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="2a2c7-226">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-226">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a><span data-ttu-id="2a2c7-227">**New-AzureRmADSpCredential**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-227">**New-AzureRmADSpCredential**</span></span>
- <span data-ttu-id="2a2c7-228">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-228">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a><span data-ttu-id="2a2c7-229">**New-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-229">**New-AzureRmADUser**</span></span>
- <span data-ttu-id="2a2c7-230">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-230">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a><span data-ttu-id="2a2c7-231">**Set-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-231">**Set-AzureRmADUser**</span></span>
- <span data-ttu-id="2a2c7-232">O parâmetro "Password" está a ser substituído em prol de uma SecureString</span><span class="sxs-lookup"><span data-stu-id="2a2c7-232">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="2a2c7-233">Alterações recentes aos cmdlets de ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2a2c7-233">Breaking changes to ServiceBus cmdlets</span></span>

### <a name="get-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="2a2c7-234">**Get-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-234">**Get-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-235">O cmdlet "Get-AzureRmServiceBusTopicAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-235">The 'Get-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-236">Utilize o cmdlet "Get-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-236">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>    

### <a name="get-azurermservicebustopickey"></a><span data-ttu-id="2a2c7-237">**Get-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-237">**Get-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="2a2c7-238">O cmdlet "Get-AzureRmServiceBusTopicKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-238">The 'Get-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-239">Utilize o cmdlet "Get-AzureRmServiceBusKey".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-239">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="2a2c7-240">**New-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-240">**New-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-241">O cmdlet "New-AzureRmServiceBusTopicAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-241">The 'New-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-242">Utilize o cmdlet "New-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-242">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebustopickey"></a><span data-ttu-id="2a2c7-243">**New-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-243">**New-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="2a2c7-244">O cmdlet "New-AzureRmServiceBusTopicKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-244">The 'New-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-245">Utilize o cmdlet "New-AzureRmServiceBusKey".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-245">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="2a2c7-246">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-246">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-247">O cmdlet "Remove-AzureRmServiceBusTopicAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-247">The 'Remove-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-248">Utilize o cmdlet "Remove-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-248">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="2a2c7-249">**Set-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-249">**Set-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-250">O cmdlet "Set-AzureRmServiceBusTopicAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-250">The 'Set-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-251">Utilize o cmdlet "Set-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-251">Please use the 'Set-AzureRmServiceBusAuthorizationRule'cmdlet.</span></span>

### <a name="new-azurermservicebusnamespacekey"></a><span data-ttu-id="2a2c7-252">**New-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-252">**New-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="2a2c7-253">O cmdlet "New-AzureRmServiceBusNamespaceKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-253">The 'New-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-254">Utilize o cmdlet "New-AzureRmServiceBusKey".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-254">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="get-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="2a2c7-255">**Get-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-255">**Get-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-256">O cmdlet "Get-AzureRmServiceBusQueueAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-256">The 'Get-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-257">Utilize o cmdlet "Get-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-257">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusqueuekey"></a><span data-ttu-id="2a2c7-258">**Get-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-258">**Get-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="2a2c7-259">O cmdlet "Get-AzureRmServiceBusQueueKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-259">The 'Get-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-260">Utilize o cmdlet "Get-AzureRmServiceBusKey".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-260">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="2a2c7-261">**New-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-261">**New-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-262">O cmdlet "New-AzureRmServiceBusQueueAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-262">The 'New-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-263">Utilize o cmdlet "New-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-263">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebusqueuekey"></a><span data-ttu-id="2a2c7-264">**New-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-264">**New-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="2a2c7-265">O cmdlet "New-AzureRmServiceBusQueueKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-265">The 'New-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-266">Utilize o cmdlet "New-AzureRmServiceBusKey".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-266">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="2a2c7-267">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-267">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-268">O cmdlet "Remove-AzureRmServiceBusQueueAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-268">The 'Remove-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-269">Utilize o cmdlet "GRemove-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-269">Please use the 'GRemove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="2a2c7-270">**Set-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-270">**Set-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-271">O cmdlet "Set-AzureRmServiceBusQueueAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-271">The 'Set-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-272">Utilize o cmdlet "Set-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-272">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-273">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-273">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-274">O cmdlet "Get-AzureRmServiceBusNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-274">The 'Get-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-275">Utilize o cmdlet "Get-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-275">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespacekey"></a><span data-ttu-id="2a2c7-276">**Get-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-276">**Get-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="2a2c7-277">O cmdlet "Get-AzureRmServiceBusNamespaceKey" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-277">The 'Get-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-278">Utilize o cmdlet "Get-AzureRmServiceBusKey".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-278">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-279">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-279">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-280">O cmdlet "New-AzureRmServiceBusNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-280">The 'New-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-281">Utilize o cmdlet "New-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-281">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-282">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-282">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-283">O cmdlet "Remove-AzureRmServiceBusNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-283">The 'Remove-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-284">Utilize o cmdlet "Remove-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-284">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="2a2c7-285">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-285">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="2a2c7-286">O cmdlet "Set-AzureRmServiceBusNamespaceAuthorizationRule" foi removido.</span><span class="sxs-lookup"><span data-stu-id="2a2c7-286">The 'Set-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="2a2c7-287">Utilize o cmdlet "Set-AzureRmServiceBusAuthorizationRule".</span><span class="sxs-lookup"><span data-stu-id="2a2c7-287">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="type-namespaceattributes"></a><span data-ttu-id="2a2c7-288">**Tipo NamespaceAttributes**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-288">**Type NamespaceAttributes**</span></span>
- <span data-ttu-id="2a2c7-289">As seguintes propriedades foram removidas</span><span class="sxs-lookup"><span data-stu-id="2a2c7-289">The following properties have been removed</span></span>
    - <span data-ttu-id="2a2c7-290">Ativado</span><span class="sxs-lookup"><span data-stu-id="2a2c7-290">Enabled</span></span>
    - <span data-ttu-id="2a2c7-291">Estado</span><span class="sxs-lookup"><span data-stu-id="2a2c7-291">Status</span></span>
   
```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmServiceBusNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Enabled and Status properties    
$namespace = Get-AzureRmServiceBusNamespace <parameters>
```

### <a name="type-queueattribute"></a><span data-ttu-id="2a2c7-292">**Tipo QueueAttribute**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-292">**Type QueueAttribute**</span></span>
- <span data-ttu-id="2a2c7-293">As seguintes propriedades estão marcadas como obsoletas:</span><span class="sxs-lookup"><span data-stu-id="2a2c7-293">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="2a2c7-294">EnableBatchedOperations</span><span class="sxs-lookup"><span data-stu-id="2a2c7-294">EnableBatchedOperations</span></span>
    - <span data-ttu-id="2a2c7-295">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="2a2c7-295">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="2a2c7-296">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="2a2c7-296">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="2a2c7-297">SupportOrdering</span><span class="sxs-lookup"><span data-stu-id="2a2c7-297">SupportOrdering</span></span>

```powershell
# Old
# The $queue has EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties
$queue = Get-AzureRmServiceBusQueue <parameters>
$queue.EntityAvailabilityStatus
$queue.EnableBatchedOperations
$queue.IsAnonymousAccessible
$queue.SupportOrdering  

# New
# The call remains the same, but the returned values Queue object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$queue = Get-AzureRmServiceBusQueue <parameters>
```
   
### <a name="type-topicattribute"></a><span data-ttu-id="2a2c7-298">**Tipo TopicAttribute**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-298">**Type TopicAttribute**</span></span>
- <span data-ttu-id="2a2c7-299">As seguintes propriedades estão marcadas como obsoletas:</span><span class="sxs-lookup"><span data-stu-id="2a2c7-299">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="2a2c7-300">Localização</span><span class="sxs-lookup"><span data-stu-id="2a2c7-300">Location</span></span>
    - <span data-ttu-id="2a2c7-301">IsExpress</span><span class="sxs-lookup"><span data-stu-id="2a2c7-301">IsExpress</span></span>
    - <span data-ttu-id="2a2c7-302">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="2a2c7-302">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="2a2c7-303">FilteringMessagesBeforePublishing</span><span class="sxs-lookup"><span data-stu-id="2a2c7-303">FilteringMessagesBeforePublishing</span></span>
    - <span data-ttu-id="2a2c7-304">EnableSubscriptionPartitioning</span><span class="sxs-lookup"><span data-stu-id="2a2c7-304">EnableSubscriptionPartitioning</span></span>
    - <span data-ttu-id="2a2c7-305">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="2a2c7-305">EntityAvailabilityStatus</span></span>

```powershell
# Old
# The $topic has EntityAvailabilityStatus, EnableSubscriptionPartitioning, IsAnonymousAccessible, IsExpress, Location and FilteringMessagesBeforePublishing properties
$topic = Get-AzureRmServiceBusTopic <parameters>
$topic.EntityAvailabilityStatus
$topic.EnableSubscriptionPartitioning
$topic.IsAnonymousAccessible
$topic.IsExpress
$topic.FilteringMessagesBeforePublishing
$topic.Location

# New
# The call remains the same, but the returned values Topic object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$topic = Get-AzureRmServiceBusTopic <parameters>
```
   
### <a name="type-subscriptionattribute"></a><span data-ttu-id="2a2c7-306">**Tipo SubscriptionAttribute**</span><span class="sxs-lookup"><span data-stu-id="2a2c7-306">**Type SubscriptionAttribute**</span></span>
- <span data-ttu-id="2a2c7-307">As seguintes propriedades estão marcadas como obsoletas</span><span class="sxs-lookup"><span data-stu-id="2a2c7-307">The following properties are marked as obsolete</span></span>
    - <span data-ttu-id="2a2c7-308">DeadLetteringOnFilterEvaluationExceptions</span><span class="sxs-lookup"><span data-stu-id="2a2c7-308">DeadLetteringOnFilterEvaluationExceptions</span></span>
    - <span data-ttu-id="2a2c7-309">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="2a2c7-309">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="2a2c7-310">IsReadOnly</span><span class="sxs-lookup"><span data-stu-id="2a2c7-310">IsReadOnly</span></span>
    - <span data-ttu-id="2a2c7-311">Localização</span><span class="sxs-lookup"><span data-stu-id="2a2c7-311">Location</span></span>
   
```powershell
# Old
# The $subscription has EntityAvailabilityStatus, EnableSubscriptionPartitioning, IsAnonymousAccessible, IsExpress, Location and FilteringMessagesBeforePublishing properties
$subscription = Get-AzureRmServiceBussubscription <parameters>
$subscription.EntityAvailabilityStatus
$subscription.EnableSubscriptionPartitioning
$subscription.IsAnonymousAccessible
$subscription.IsExpress
$subscription.FilteringMessagesBeforePublishing
$subscription.Location

# New
# The call remains the same, but the returned values Topic object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$subscription = Get-AzureRmServiceBussubscription <parameters>
```