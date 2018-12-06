---
title: Executar cmdlets em paralelo com as tarefas do PowerShell
description: Como executar os cmdlets em paralelo com o parâmetro -AsJob.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 85e4612146c07b963ca51a7203ea7782d058b93d
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/05/2018
ms.locfileid: "52827076"
---
# <a name="running-cmdlets-in-parallel-using-powershell-jobs"></a><span data-ttu-id="e02fa-103">Executar cmdlets em paralelo com as tarefas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="e02fa-103">Running cmdlets in parallel using PowerShell jobs</span></span>

<span data-ttu-id="e02fa-104">O PowerShell suporta ações assíncronas com as [tarefas do PowerShell](/powershell/module/microsoft.powershell.core/about/about_jobs).</span><span class="sxs-lookup"><span data-stu-id="e02fa-104">PowerShell supports asynchronous action with [PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>
<span data-ttu-id="e02fa-105">O Azure PowerShell é bastante dependente de realizar e receber chamadas de rede para o Azure.</span><span class="sxs-lookup"><span data-stu-id="e02fa-105">Azure PowerShell is heavily dependent on making, and waiting for, network calls to Azure.</span></span> <span data-ttu-id="e02fa-106">Muitas vezes, talvez se depare a fazer chamadas sem bloqueio.</span><span class="sxs-lookup"><span data-stu-id="e02fa-106">You may often find yourself needing to make non-blocking calls.</span></span> <span data-ttu-id="e02fa-107">Para resolver esta necessidade, o Azure PowerShell oferece suporte [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) de primeira classe.</span><span class="sxs-lookup"><span data-stu-id="e02fa-107">To address this need, Azure PowerShell provides first-class [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) support.</span></span>

## <a name="context-persistence-and-psjobs"></a><span data-ttu-id="e02fa-108">Persistência de Contexto e PSJobs</span><span class="sxs-lookup"><span data-stu-id="e02fa-108">Context Persistence and PSJobs</span></span>

<span data-ttu-id="e02fa-109">Uma vez que os PSJobs são executados como processos separados, a sua ligação do Azure tem de ser partilhada com eles.</span><span class="sxs-lookup"><span data-stu-id="e02fa-109">Since PSJobs are run as separate processes, your Azure connection must be shared with them.</span></span> <span data-ttu-id="e02fa-110">Depois de iniciar sessão na sua conta do Azure com `Connect-AzureRmAccount`, passe o contexto para uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="e02fa-110">After signing in to your Azure account with `Connect-AzureRmAccount`, pass the context to a job.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$job = Start-Job { param($context,$vmadmin) New-AzureRmVM -Name MyVm -AzureRmContext $context -Credential $vmadmin} -Arguments (Get-AzureRmContext),$creds
```

<span data-ttu-id="e02fa-111">No entanto, se tiver optado por ter o contexto guardado automaticamente com `Enable-AzureRmContextAutosave`, o contexto é automaticamente partilhado com quaisquer tarefas que crie.</span><span class="sxs-lookup"><span data-stu-id="e02fa-111">However, if you have chosen to have your context automatically saved with `Enable-AzureRmContextAutosave`, the context is automatically shared with any jobs you create.</span></span>

```azurepowershell-interactive
Enable-AzureRmContextAutosave
$creds = Get-Credential
$job = Start-Job { param($vmadmin) New-AzureRmVM -Name MyVm -Credential $vmadmin} -Arguments $creds
```

## <a name="automatic-jobs-with--asjob"></a><span data-ttu-id="e02fa-112">Tarefas automáticas com `-AsJob`</span><span class="sxs-lookup"><span data-stu-id="e02fa-112">Automatic Jobs with `-AsJob`</span></span>

<span data-ttu-id="e02fa-113">Para efeitos práticos, o Azure PowerShell também fornece um comutador `-AsJob` em alguns cmdlets de execução longa.</span><span class="sxs-lookup"><span data-stu-id="e02fa-113">As a convenience, Azure PowerShell also provides an `-AsJob` switch on some long-running cmdlets.</span></span>
<span data-ttu-id="e02fa-114">O comutador `-AsJob` permite criar PSJobs de forma ainda mais fácil.</span><span class="sxs-lookup"><span data-stu-id="e02fa-114">The `-AsJob` switch makes creating PSJobs even easier.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$job = New-AzureRmVM -Name MyVm -Credential $creds -AsJob
```

<span data-ttu-id="e02fa-115">Pode inspecionar a tarefa e o progresso a qualquer altura com `Get-Job` e `Get-AzureRmVM`.</span><span class="sxs-lookup"><span data-stu-id="e02fa-115">You can inspect the job and progress at any time with `Get-Job` and `Get-AzureRmVM`.</span></span>

```azurepowershell-interactive
Get-Job $job
Get-AzureRmVM MyVm
```

```output
Id Name                                       PSJobTypeName         State   HasMoreData Location  Command
-- ----                                       -------------         -----   ----------- --------  -------
1  Long Running Operation for 'New-AzureRmVM' AzureLongRunningJob`1 Running True        localhost New-AzureRmVM

ResourceGroupName    Name Location          VmSize  OsType     NIC ProvisioningState Zone
-----------------    ---- --------          ------  ------     --- ----------------- ----
MyVm                 MyVm   eastus Standard_DS1_v2 Windows    MyVm          Creating
```

<span data-ttu-id="e02fa-116">Quando a tarefa estiver concluída, obtenha o resultado da tarefa com `Receive-Job`.</span><span class="sxs-lookup"><span data-stu-id="e02fa-116">When the job completes, get the result of the job with `Receive-Job`.</span></span>

> [!NOTE]
> <span data-ttu-id="e02fa-117">`Receive-Job` devolve o resultado a partir do cmdlet como se o sinalizador `-AsJob` não estivesse presente.</span><span class="sxs-lookup"><span data-stu-id="e02fa-117">`Receive-Job` returns the result from the cmdlet as if the `-AsJob` flag were not present.</span></span>
> <span data-ttu-id="e02fa-118">Por exemplo, o resultado `Receive-Job` de `Do-Action -AsJob` é do mesmo tipo que o resultado de `Do-Action`.</span><span class="sxs-lookup"><span data-stu-id="e02fa-118">For example, the `Receive-Job` result of `Do-Action -AsJob` is of the same type as the result of `Do-Action`.</span></span>

```azurepowershell-interactive
$vm = Receive-Job $job
$vm
```

```output
ResourceGroupName        : MyVm
Id                       : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyVm/providers/Microsoft.Compute/virtualMachines/MyVm
VmId                     : dff1f79e-a8f7-4664-ab72-0ec28b9fbb5b
Name                     : MyVm
Type                     : Microsoft.Compute/virtualMachines
Location                 : eastus
Tags                     : {}
HardwareProfile          : {VmSize}
NetworkProfile           : {NetworkInterfaces}
OSProfile                : {ComputerName, AdminUsername, WindowsConfiguration, Secrets}
ProvisioningState        : Succeeded
StorageProfile           : {ImageReference, OsDisk, DataDisks}
FullyQualifiedDomainName : myvmmyvm.eastus.cloudapp.azure.com
```

## <a name="example-scenarios"></a><span data-ttu-id="e02fa-119">Cenários de Exemplo</span><span class="sxs-lookup"><span data-stu-id="e02fa-119">Example Scenarios</span></span>

<span data-ttu-id="e02fa-120">Crie várias VMs de uma só vez:</span><span class="sxs-lookup"><span data-stu-id="e02fa-120">Create several VMs at once:</span></span>

```azurepowershell-interactive
$creds = Get-Credential
# Create 10 jobs.
for($k = 0; $k -lt 10; $k++) {
    New-AzureRmVm -Name MyVm$k  -Credential $creds -AsJob
}

# Get all jobs and wait on them.
Get-Job | Wait-Job
"All jobs completed"
Get-AzureRmVM
```

<span data-ttu-id="e02fa-121">Neste exemplo, o cmdlet `Wait-Job` faz com que o script fique em pausa durante a execução de tarefas.</span><span class="sxs-lookup"><span data-stu-id="e02fa-121">In this example, the `Wait-Job` cmdlet causes the script to pause while jobs run.</span></span> <span data-ttu-id="e02fa-122">O script continua em execução depois de todas as tarefas terem concluído.</span><span class="sxs-lookup"><span data-stu-id="e02fa-122">The script continues executing once all of the jobs have completed.</span></span> <span data-ttu-id="e02fa-123">São executadas várias tarefas em paralelo e, em seguida, o script aguarda pela conclusão antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="e02fa-123">Several jobs run in parallel then the script waits for completion before continuing.</span></span>

```output
Id     Name            PSJobTypeName   State         HasMoreData     Location             Command
--     ----            -------------   -----         -----------     --------             -------
2      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
3      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
4      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
5      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
6      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
7      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
8      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
9      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
10     Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
11     Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
2      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
3      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
4      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
5      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
6      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
7      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
8      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
9      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
10     Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
11     Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
All Jobs completed.

ResourceGroupName        Name   Location          VmSize  OsType           NIC ProvisioningState Zone
-----------------        ----   --------          ------  ------           --- ----------------- ----
MYVM                     MyVm     eastus Standard_DS1_v2 Windows          MyVm         Succeeded
MYVM0                   MyVm0     eastus Standard_DS1_v2 Windows         MyVm0         Succeeded
MYVM1                   MyVm1     eastus Standard_DS1_v2 Windows         MyVm1         Succeeded
MYVM2                   MyVm2     eastus Standard_DS1_v2 Windows         MyVm2         Succeeded
MYVM3                   MyVm3     eastus Standard_DS1_v2 Windows         MyVm3         Succeeded
MYVM4                   MyVm4     eastus Standard_DS1_v2 Windows         MyVm4         Succeeded
MYVM5                   MyVm5     eastus Standard_DS1_v2 Windows         MyVm5         Succeeded
MYVM6                   MyVm6     eastus Standard_DS1_v2 Windows         MyVm6         Succeeded
MYVM7                   MyVm7     eastus Standard_DS1_v2 Windows         MyVm7         Succeeded
MYVM8                   MyVm8     eastus Standard_DS1_v2 Windows         MyVm8         Succeeded
MYVM9                   MyVm9     eastus Standard_DS1_v2 Windows         MyVm9         Succeeded
```
