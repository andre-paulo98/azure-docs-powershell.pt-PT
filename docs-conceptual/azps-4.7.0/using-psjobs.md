---
title: Executar cmdlets do Azure PowerShell em Tarefas do PowerShell
description: Saiba como executar cmdlets do Azure PowerShell em paralelo ou como tarefas em segundo plano, com -AsJob e Start-Job.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 5d9028c0a433149c8f6cc346651bb8bf875bb42a
ms.sourcegitcommit: 15f21c40dcb7610e2fbaaabf264ad925e4224500
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90928590"
---
# <a name="run-azure-powershell-cmdlets-in-powershell-jobs"></a>Executar cmdlets do Azure PowerShell em Tarefas do PowerShell

O Azure PowerShell depende da ligação a uma cloud do Azure e de aguardar respostas. Por isso, a maioria destes cmdlets bloqueia sua sessão do PowerShell até obterem uma resposta da cloud.
As tarefas do PowerShell permitem executar cmdlets em segundo plano ou realizar várias tarefas no Azure de uma só vez, a partir de uma única sessão do PowerShell.

Este artigo é uma breve descrição geral de como executar cmdlets do Azure PowerShell como Tarefas do PowerShell e verificar a conclusão. A execução de comandos no Azure PowerShell requer a utilização de contextos do Azure PowerShell, que são explicados em detalhe no artigo [Contextos e credenciais de início de sessão do Azure](context-persistence.md).
Para obter mais informações sobre as tarefas do PowerShell, veja [About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs) (Acerca das Tarefas do PowerShell).

## <a name="azure-contexts-with-powershell-jobs"></a>Contextos do Azure com tarefas do PowerShell

As Tarefas do PowerShell são executadas como processos separados sem uma sessão do PowerShell associada, pelo que as suas credenciais do Azure têm de ser partilhadas com elas. As credenciais são transmitidas como objetos do Azure, através de um destes métodos:

* Persistência de contexto automática. A persistência de contexto é ativada por predefinição e preserva as suas informações de início de sessão em várias sessões. Com a persistência de contexto ativada, o contexto atual do Azure é transmitido para o novo processo:

  ```azurepowershell-interactive
  Enable-AzContextAutosave # Enables context autosave if not already on
  $creds = Get-Credential
  $job = Start-Job { param($vmadmin) New-AzVM -Name MyVm -Credential $vmadmin } -ArgumentList $creds
  ```

* Utilize o parâmetro `-AzContext` com qualquer cmdlet do Azure PowerShell para fornecer um objeto de contexto do Azure:

  ```azurepowershell-interactive
  $context = Get-AzContext -Name 'mycontext' # Get an Azure context object
  $creds = Get-Credential
  $job = Start-Job { param($context, $vmadmin) New-AzVM -Name MyVm -AzContext $context -Credential $vmadmin} -ArgumentList $context,$creds }
  ```

  Se a persistência de contexto estiver desativada, o argumento `-AzContext` é necessário.

* Utilize o parâmetro `-AsJob` fornecido por alguns cmdlets do Azure PowerShell. Este parâmetro inicia automaticamente o cmdlet como uma Tarefa do PowerShell, com o contexto do Azure atualmente ativo:

  ```azurepowershell-interactive
  $creds = Get-Credential
  $job = New-AzVM -Name MyVm -Credential $creds -AsJob
  ```

  Para ver se um cmdlet suporta `-AsJob`, verifique a respetiva documentação de referência. O parâmetro `-AsJob` não exige que a gravação automática do contexto esteja ativada.

Pode verificar o estado de uma tarefa em execução com o cmdlet [Get-Job](/powershell/module/microsoft.powershell.core/get-job). Para obter a saída de uma tarefa até ao momento, utilize o cmdlet [Receive-Job](/powershell/module/microsoft.powershell.core/receive-job).

Para verificar o progresso de uma operação remotamente no Azure, utilize os cmdlets `Get-` associados ao tipo de recurso que está a ser modificado pela tarefa:

```azurepowershell-interactive
$creds = Get-Credential
$context = Get-AzContext -Name 'mycontext'
$vmName = "MyVm"

$job = Start-Job { param($context, $vmName, $vmadmin) New-AzVM -Name $vmName -AzContext $context -Credential $vmadmin} -ArgumentList $context,$vmName,$creds }

Get-Job $job
Get-AzVM -Name $vmName
```

## <a name="see-also"></a>Consulte também

* [Contextos do Azure PowerShell](context-persistence.md)
* [About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs) (Acerca das Tarefas do PowerShell)
* [Referência de Get-Job](/powershell/module/microsoft.powershell.core/get-job)
* [Referência de Receive-Job](/powershell/module/microsoft.powershell.core/receive-job)
