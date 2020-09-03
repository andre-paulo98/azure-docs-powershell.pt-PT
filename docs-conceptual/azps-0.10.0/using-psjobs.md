---
title: Executar cmdlets do Azure PowerShell em Tarefas do PowerShell
description: Saiba como executar cmdlets do Azure PowerShell em paralelo ou como tarefas em segundo plano, com -AsJob e Start-Job.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 5d9028c0a433149c8f6cc346651bb8bf875bb42a
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243162"
---
# <a name="run-azure-powershell-cmdlets-in-powershell-jobs"></a><span data-ttu-id="b84f5-103">Executar cmdlets do Azure PowerShell em Tarefas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="b84f5-103">Run Azure PowerShell cmdlets in PowerShell Jobs</span></span>

<span data-ttu-id="b84f5-104">O Azure PowerShell depende da ligação a uma cloud do Azure e de aguardar respostas. Por isso, a maioria destes cmdlets bloqueia sua sessão do PowerShell até obterem uma resposta da cloud.</span><span class="sxs-lookup"><span data-stu-id="b84f5-104">Azure PowerShell depends on connecting to an Azure cloud and waiting for responses, so most of these cmdlets block your PowerShell session until they get a response from the cloud.</span></span>
<span data-ttu-id="b84f5-105">As tarefas do PowerShell permitem executar cmdlets em segundo plano ou realizar várias tarefas no Azure de uma só vez, a partir de uma única sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b84f5-105">Powershell Jobs let you run cmdlets in the background or do multiple tasks on Azure at once, from inside a single PowerShell session.</span></span>

<span data-ttu-id="b84f5-106">Este artigo é uma breve descrição geral de como executar cmdlets do Azure PowerShell como Tarefas do PowerShell e verificar a conclusão.</span><span class="sxs-lookup"><span data-stu-id="b84f5-106">This article is a brief overview of how to run Azure PowerShell cmdlets as PowerShell Jobs and check for completion.</span></span> <span data-ttu-id="b84f5-107">A execução de comandos no Azure PowerShell requer a utilização de contextos do Azure PowerShell, que são explicados em detalhe no artigo [Contextos e credenciais de início de sessão do Azure](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="b84f5-107">Running commands in Azure PowerShell requires the use of Azure PowerShell contexts, which are covered in detail in [Azure contexts and sign-in credentials](context-persistence.md).</span></span>
<span data-ttu-id="b84f5-108">Para obter mais informações sobre as tarefas do PowerShell, veja [About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs) (Acerca das Tarefas do PowerShell).</span><span class="sxs-lookup"><span data-stu-id="b84f5-108">To learn more about PowerShell Jobs, see [About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="azure-contexts-with-powershell-jobs"></a><span data-ttu-id="b84f5-109">Contextos do Azure com tarefas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="b84f5-109">Azure contexts with PowerShell jobs</span></span>

<span data-ttu-id="b84f5-110">As Tarefas do PowerShell são executadas como processos separados sem uma sessão do PowerShell associada, pelo que as suas credenciais do Azure têm de ser partilhadas com elas.</span><span class="sxs-lookup"><span data-stu-id="b84f5-110">PowerShell Jobs are run as separate processes without an attached PowerShell session, so your Azure credentials must be shared with them.</span></span> <span data-ttu-id="b84f5-111">As credenciais são transmitidas como objetos do Azure, através de um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="b84f5-111">Credentials are passed as Azure context objects, using one of these methods:</span></span>

* <span data-ttu-id="b84f5-112">Persistência de contexto automática.</span><span class="sxs-lookup"><span data-stu-id="b84f5-112">Automatic context persistence.</span></span> <span data-ttu-id="b84f5-113">A persistência de contexto é ativada por predefinição e preserva as suas informações de início de sessão em várias sessões.</span><span class="sxs-lookup"><span data-stu-id="b84f5-113">Context persistence is enabled by default and preserves your sign-in information across multiple sessions.</span></span> <span data-ttu-id="b84f5-114">Com a persistência de contexto ativada, o contexto atual do Azure é transmitido para o novo processo:</span><span class="sxs-lookup"><span data-stu-id="b84f5-114">With context persistence enabled, the current Azure context is passed to the new process:</span></span>

  ```azurepowershell-interactive
  Enable-AzContextAutosave # Enables context autosave if not already on
  $creds = Get-Credential
  $job = Start-Job { param($vmadmin) New-AzVM -Name MyVm -Credential $vmadmin } -ArgumentList $creds
  ```

* <span data-ttu-id="b84f5-115">Utilize o parâmetro `-AzContext` com qualquer cmdlet do Azure PowerShell para fornecer um objeto de contexto do Azure:</span><span class="sxs-lookup"><span data-stu-id="b84f5-115">Use the `-AzContext` parameter with any Azure PowerShell cmdlets to provide an Azure context object:</span></span>

  ```azurepowershell-interactive
  $context = Get-AzContext -Name 'mycontext' # Get an Azure context object
  $creds = Get-Credential
  $job = Start-Job { param($context, $vmadmin) New-AzVM -Name MyVm -AzContext $context -Credential $vmadmin} -ArgumentList $context,$creds }
  ```

  <span data-ttu-id="b84f5-116">Se a persistência de contexto estiver desativada, o argumento `-AzContext` é necessário.</span><span class="sxs-lookup"><span data-stu-id="b84f5-116">If context persistence is disabled, the `-AzContext` argument is required.</span></span>

* <span data-ttu-id="b84f5-117">Utilize o parâmetro `-AsJob` fornecido por alguns cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b84f5-117">Use the `-AsJob` switch provided by some Azure PowerShell cmdlets.</span></span> <span data-ttu-id="b84f5-118">Este parâmetro inicia automaticamente o cmdlet como uma Tarefa do PowerShell, com o contexto do Azure atualmente ativo:</span><span class="sxs-lookup"><span data-stu-id="b84f5-118">This switch automatically starts the cmdlet as a PowerShell Job, using the currently active Azure context:</span></span>

  ```azurepowershell-interactive
  $creds = Get-Credential
  $job = New-AzVM -Name MyVm -Credential $creds -AsJob
  ```

  <span data-ttu-id="b84f5-119">Para ver se um cmdlet suporta `-AsJob`, verifique a respetiva documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="b84f5-119">To see if a cmdlet supports `-AsJob`, check its reference documentation.</span></span> <span data-ttu-id="b84f5-120">O parâmetro `-AsJob` não exige que a gravação automática do contexto esteja ativada.</span><span class="sxs-lookup"><span data-stu-id="b84f5-120">The `-AsJob` switch doesn't require context autosave to be enabled.</span></span>

<span data-ttu-id="b84f5-121">Pode verificar o estado de uma tarefa em execução com o cmdlet [Get-Job](/powershell/module/microsoft.powershell.core/get-job).</span><span class="sxs-lookup"><span data-stu-id="b84f5-121">You can check the status of a running job with the [Get-Job](/powershell/module/microsoft.powershell.core/get-job) cmdlet.</span></span> <span data-ttu-id="b84f5-122">Para obter a saída de uma tarefa até ao momento, utilize o cmdlet [Receive-Job](/powershell/module/microsoft.powershell.core/receive-job).</span><span class="sxs-lookup"><span data-stu-id="b84f5-122">To get the output from a job so far, use the [Receive-Job](/powershell/module/microsoft.powershell.core/receive-job) cmdlet.</span></span>

<span data-ttu-id="b84f5-123">Para verificar o progresso de uma operação remotamente no Azure, utilize os cmdlets `Get-` associados ao tipo de recurso que está a ser modificado pela tarefa:</span><span class="sxs-lookup"><span data-stu-id="b84f5-123">To check an operation's progress remotely on Azure, use the `Get-` cmdlets associated with the type of resource being modified by the job:</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$context = Get-AzContext -Name 'mycontext'
$vmName = "MyVm"

$job = Start-Job { param($context, $vmName, $vmadmin) New-AzVM -Name $vmName -AzContext $context -Credential $vmadmin} -ArgumentList $context,$vmName,$creds }

Get-Job $job
Get-AzVM -Name $vmName
```

## <a name="see-also"></a><span data-ttu-id="b84f5-124">Consulte também</span><span class="sxs-lookup"><span data-stu-id="b84f5-124">See Also</span></span>

* [<span data-ttu-id="b84f5-125">Contextos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b84f5-125">Azure PowerShell contexts</span></span>](context-persistence.md)
* <span data-ttu-id="b84f5-126">[About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs) (Acerca das Tarefas do PowerShell)</span><span class="sxs-lookup"><span data-stu-id="b84f5-126">[About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs)</span></span>
* [<span data-ttu-id="b84f5-127">Referência de Get-Job</span><span class="sxs-lookup"><span data-stu-id="b84f5-127">Get-Job reference</span></span>](/powershell/module/microsoft.powershell.core/get-job)
* [<span data-ttu-id="b84f5-128">Referência de Receive-Job</span><span class="sxs-lookup"><span data-stu-id="b84f5-128">Receive-Job reference</span></span>](/powershell/module/microsoft.powershell.core/receive-job)
