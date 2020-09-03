---
title: Executar cmdlets em paralelo com as tarefas do PowerShell
description: Como executar os cmdlets em paralelo com o parâmetro -AsJob.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/11/2017
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: b5385a9fa3da508e6f0841baea2e4bcd20503b9f
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243553"
---
# <a name="running-cmdlets-in-parallel-using-powershell-jobs"></a><span data-ttu-id="6808d-103">Executar cmdlets em paralelo com as tarefas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="6808d-103">Running cmdlets in parallel using PowerShell jobs</span></span>

[!INCLUDE [migrate-to-az-banner](../../includes/migrate-to-az-banner.md)]

<span data-ttu-id="6808d-104">O PowerShell suporta ações assíncronas com as [tarefas do PowerShell](/powershell/module/microsoft.powershell.core/about/about_jobs).</span><span class="sxs-lookup"><span data-stu-id="6808d-104">PowerShell supports asynchronous action with [PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>
<span data-ttu-id="6808d-105">O Azure PowerShell é bastante dependente de realizar e receber chamadas de rede para o Azure.</span><span class="sxs-lookup"><span data-stu-id="6808d-105">Azure PowerShell is heavily dependent on making, and waiting for, network calls to Azure.</span></span> <span data-ttu-id="6808d-106">Como programador, pode encontrar-se várias vezes à procura de fazer várias chamadas não bloqueadas ao Azure num script ou pode querer criar recursos do Azure no REPL sem bloquear a sessão atual.</span><span class="sxs-lookup"><span data-stu-id="6808d-106">As a developer, you may often find yourself looking to make multiple non-blocking calls to Azure in a script, or you may find that you want to create Azure resources in the REPL without blocking the current session.</span></span> <span data-ttu-id="6808d-107">Para resolver estas necessidades, o Azure PowerShell fornece suporte [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) de primeira classe.</span><span class="sxs-lookup"><span data-stu-id="6808d-107">To address these needs, Azure PowerShell provides first-class [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) support.</span></span>

## <a name="context-persistence-and-psjobs"></a><span data-ttu-id="6808d-108">Persistência de Contexto e PSJobs</span><span class="sxs-lookup"><span data-stu-id="6808d-108">Context Persistence and PSJobs</span></span>

<span data-ttu-id="6808d-109">Os PSJobs são executados em processos separados, o que significa que as informações sobre a sua ligação do Azure devem ser partilhadas corretamente com as tarefas que cria.</span><span class="sxs-lookup"><span data-stu-id="6808d-109">PSJobs are run in separate processes, which means that information about your Azure connection must be properly shared with the jobs you create.</span></span> <span data-ttu-id="6808d-110">Ao ligar a sua conta do Azure à sua sessão do PowerShell com `Connect-AzureRmAccount`, pode passar o contexto para uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="6808d-110">Upon connecting your Azure account to your PowerShell session with `Connect-AzureRmAccount`, you can pass the context to a job.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$job = Start-Job { param($context,$vmadmin) New-AzureRmVM -Name MyVm -AzureRmContext $context -Credential $vmadmin} -Arguments (Get-AzureRmContext),$creds
```

<span data-ttu-id="6808d-111">No entanto, se tiver optado por ter o contexto guardado automaticamente com `Enable-AzureRmContextAutosave`, o contexto é automaticamente partilhado com quaisquer tarefas que crie.</span><span class="sxs-lookup"><span data-stu-id="6808d-111">However, if you have chosen to have your context automatically saved with `Enable-AzureRmContextAutosave`, the context is automatically shared with any jobs you create.</span></span>

```azurepowershell-interactive
Enable-AzureRmContextAutosave
$creds = Get-Credential
$job = Start-Job { param($vmadmin) New-AzureRmVM -Name MyVm -Credential $vmadmin} -Arguments $creds
```

## <a name="automatic-jobs-with--asjob"></a><span data-ttu-id="6808d-112">Tarefas automáticas com `-AsJob`</span><span class="sxs-lookup"><span data-stu-id="6808d-112">Automatic Jobs with `-AsJob`</span></span>

<span data-ttu-id="6808d-113">Para efeitos práticos, o Azure PowerShell também fornece um comutador `-AsJob` em alguns cmdlets de execução longa.</span><span class="sxs-lookup"><span data-stu-id="6808d-113">As a convenience, Azure PowerShell also provides an `-AsJob` switch on some long-running cmdlets.</span></span>
<span data-ttu-id="6808d-114">O comutador `-AsJob` permite criar PSJobs de forma ainda mais fácil.</span><span class="sxs-lookup"><span data-stu-id="6808d-114">The `-AsJob` switch makes creating PSJobs even easier.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$job = New-AzureRmVM -Name MyVm -Credential $creds -AsJob
```

<span data-ttu-id="6808d-115">Pode inspecionar a tarefa e o progresso a qualquer altura com `Get-Job` e `Get-AzureRmVM`.</span><span class="sxs-lookup"><span data-stu-id="6808d-115">You can inspect the job and progress at any time with `Get-Job` and `Get-AzureRmVM`.</span></span>

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

<span data-ttu-id="6808d-116">Posteriormente, após a conclusão, pode obter o resultado da tarefa com `Receive-Job`.</span><span class="sxs-lookup"><span data-stu-id="6808d-116">Subsequently, upon completion, you can obtain the result of the job with `Receive-Job`.</span></span>

> [!NOTE]
> <span data-ttu-id="6808d-117">`Receive-Job` devolve o resultado a partir do cmdlet como se o sinalizador `-AsJob` não estivesse presente.</span><span class="sxs-lookup"><span data-stu-id="6808d-117">`Receive-Job` returns the result from the cmdlet as if the `-AsJob` flag were not present.</span></span>
> <span data-ttu-id="6808d-118">Por exemplo, o resultado `Receive-Job` de `Do-Action -AsJob` é do mesmo tipo que o resultado de `Do-Action`.</span><span class="sxs-lookup"><span data-stu-id="6808d-118">For example, the `Receive-Job` result of `Do-Action -AsJob` is of the same type as the result of `Do-Action`.</span></span>

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

## <a name="example-scenarios"></a><span data-ttu-id="6808d-119">Cenários de Exemplo</span><span class="sxs-lookup"><span data-stu-id="6808d-119">Example Scenarios</span></span>

<span data-ttu-id="6808d-120">Criar múltiplas VMs ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6808d-120">Create multiple VMs at once.</span></span>

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

<span data-ttu-id="6808d-121">Neste exemplo, o cmdlet `Wait-Job` faz com que o script fique em pausa durante a execução de tarefas.</span><span class="sxs-lookup"><span data-stu-id="6808d-121">In this example, the `Wait-Job` cmdlet causes the script to pause while jobs run.</span></span> <span data-ttu-id="6808d-122">O script continua em execução depois de todas as tarefas terem concluído.</span><span class="sxs-lookup"><span data-stu-id="6808d-122">The script continues executing once all of the jobs have completed.</span></span> <span data-ttu-id="6808d-123">Isto permite-lhe criar várias tarefas em execução em paralelo e então aguardar pela conclusão antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="6808d-123">This allows you to create several jobs running in parallel then wait for completion before continuing.</span></span>

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
