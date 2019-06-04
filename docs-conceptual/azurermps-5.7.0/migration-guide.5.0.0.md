---
title: Alterações recentes ao Microsoft Azure PowerShell 5.0.0
description: Este guia de migração contém uma lista de alterações recentes realizadas no Azure PowerShell no lançamento da versão 5.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: f8dc413a91876e53e62d25cc38ac3b3ef6afda8e
ms.sourcegitcommit: bbd3f061cac3417ce588487c1ae4e0bc52c11d6a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/11/2019
ms.locfileid: "65534596"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a>Alterações recentes ao Microsoft Azure PowerShell 5.0.0

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell. Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço. Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.

## <a name="table-of-contents"></a>Índice

- [Alterações recentes aos cmdlets de ApiManagement ](#breaking-changes-to-apimanagement-cmdlets)
- [Alterações recentes aos cmdlets de Batch](#breaking-changes-to-batch-cmdlets)
- [Alterações recentes aos cmdlets de Computação](#breaking-changes-to-compute-cmdlets)
- [Alterações recentes aos cmdlets de EventHub](#breaking-changes-to-eventhub-cmdlets)
- [Alterações recentes aos cmdlets de Insights](#breaking-changes-to-insights-cmdlets)
- [Alterações recentes aos cmdlets de Rede](#breaking-changes-to-network-cmdlets)
- [Alterações recentes aos cmdlets de Recursos](#breaking-changes-to-resources-cmdlets)
- [Alterações recentes aos cmdlets de ServiceBus](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a>Alterações recentes aos cmdlets de ApiManagement

### <a name="new-azurermapimanagementbackendproxy"></a>**New-AzureRmApiManagementBackendProxy**
- Os parâmetros "UserName" e "Password" estão a ser substituídos em prol de uma PSCredential

```powershell-interactive
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a>**New-AzureRmApiManagementUser**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a>**Set-AzureRmApiManagementUser**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a>Alterações recentes aos cmdlets de Batch

### <a name="new-azurebatchcertificate"></a>**New-AzureBatchCertificate**
- O parâmetro `Password` está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a>**New-AzureBatchComputeNodeUser**
- O parâmetro `Password` está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a>**Set-AzureRmBatchComputeNodeUser**
- O parâmetro `Password` está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a>**New-AzureBatchTask**
 - O parâmetro `RunElevated` foi removido e substituído por `UserIdentity`.

```powershell-interactive
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

Esta alteração também afeta a propriedade `RunElevated` em `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` e `PSJobReleaseTask`.

### <a name="psmultiinstancesettings"></a>**PSMultiInstanceSettings**

- O construtor `PSMultiInstanceSettings` já não precisa de um parâmetro `numberOfInstances` obrigatório. Em vez disso, precisa de um parâmetro `coordinationCommandLine` obrigatório.

```powershell-interactive
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a>**Get-AzureBatchTask**
 - A propriedade `RunElevated` foi removida em `PSCloudTask`. A propriedade `UserIdentity` foi adicionada para substituir `RunElevated`.

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

Esta alteração também afeta a propriedade `RunElevated` em `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` e `PSJobReleaseTask`.

### <a name="multiple-types"></a>**Vários tipos**

- O nome da propriedade `SchedulingError` foi mudado em `PSExitConditions` para `PreProcessingError`.

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a>**Vários tipos**

- O nome da propriedade `SchedulingError` foi mudado em `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation` e `PSTaskExecutionInformation` para `FailureInformation`.
  - `FailureInformation` é devolvido sempre que ocorre uma falha de tarefa. Isto inclui todos os casos de erro de agendamento anteriores, bem como os códigos de saída de tarefa diferentes de zero e falhas de carregamento de ficheiros da nova funcionalidade de ficheiros de saída.
  - A estrutura continua igual à utilizada anteriormente, pelo que não é necessário efetuar qualquer alteração no código ao utilizar este tipo.

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

Esta alteração também afeta: Get-AzureBatchPool, Get-AzureBatchSubtask e Get-AzureBatchJobPreparationAndReleaseTaskStatus

### <a name="new-azurebatchpool"></a>**New-AzureBatchPool**
 - `TargetDedicated` foi removido e substituído por `TargetDedicatedComputeNodes` e `TargetLowPriorityComputeNodes`.
 - `TargetDedicatedComputeNodes` tem um alias `TargetDedicated`.

```powershell-interactive
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

Esta alteração também afeta: Start-AzureBatchPoolResize

### <a name="get-azurebatchpool"></a>**Get-AzureBatchPool**
 - O nome das propriedades `TargetDedicated` e `CurrentDedicated` foi mudado em `PSCloudPool` para `TargetDedicatedComputeNodes` e `CurrentDedicatedComputeNodes`.

```powershell-interactive
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicated
$pool.CurrentDedicated

# New
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicatedComputeNodes
$pool.CurrentDedicatedComputeNodes
```

### <a name="type-pscloudpool"></a>**Tipo PSCloudPool**

- O nome de `ResizeError` foi mudado para `ResizeErrors` em `PSCloudPool` e é agora uma coleção.

```powershell-interactive
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a>**New-AzureBatchJob**
- O nome da propriedade `TargetDedicated` foi mudado em `PSPoolSpecification` para `TargetDedicatedComputeNodes`.

```powershell-interactive
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

### <a name="get-azurebatchnodefile"></a>**Get-AzureBatchNodeFile**
 - `Name` foi removido e substituído por `Path`.
 - `Path` tem um alias `Name`.

```powershell-interactive
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

Esta alteração também afeta: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile

### <a name="type-psnodefile"></a>Tipo **PSNodeFile**

 - O nome da propriedade `Name` foi mudado em `PSNodeFile` para `Path`.

```powershell-interactive
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a>**Get-AzureBatchSubtask**
- As propriedades `PreviousState` e `State` de `PSSubtaskInformation` já não são do tipo `TaskState`, sendo agora do tipo `SubtaskState`.
  - Ao contrário de `TaskState`, `SubtaskState` não tem um valor `Active`, uma vez que as subtarefas não podem ter um estado `Active`.

```powershell-interactive
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a>Alterações recentes aos cmdlets de Computação

### <a name="set-azurermvmaccessextension"></a>**Set-AzureRmVMAccessExtension**
- Os parâmetros "UserName" e "Password" estão a ser substituídos em prol de uma PSCredential

```powershell-interactive
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a>Alterações recentes aos cmdlets de EventHub

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a>**New-AzureRmEventHubNamespaceAuthorizationRule**
- O cmdlet "New-AzureRmEventHubNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "New-AzureRmEventHubAuthorizationRule"
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a>**Get-AzureRmEventHubNamespaceAuthorizationRule**
- O cmdlet "Get-AzureRmEventHubNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "Get-AzureRmEventHubAuthorizationRule"
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a>**Set-AzureRmEventHubNamespaceAuthorizationRule**
- O cmdlet "Set-AzureRmEventHubNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "Set-AzureRmEventHubAuthorizationRule"
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a>**Remove-AzureRmEventHubNamespaceAuthorizationRule**
- O cmdlet "Remove-AzureRmEventHubNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "Remove-AzureRmEventHubAuthorizationRule"
    
### <a name="new-azurermeventhubnamespacekey"></a>**New-AzureRmEventHubNamespaceKey**
- O cmdlet "New-AzureRmEventHubNamespaceKey" foi removido. Utilize o cmdlet "New-AzureRmEventHubKey"
    
### <a name="get-azurermeventhubnamespacekey"></a>**Get-AzureRmEventHubNamespaceKey**
- O cmdlet "Get-AzureRmEventHubNamespaceKey" foi removido. Utilize o cmdlet "Get-AzureRmEventHubKey"
    
### <a name="new-azurermeventhubnamespace"></a>**New-AzureRmEventHubNamespace**
- As propriedades "Status" e "Enabled" de NamespceAttributes irão ser removidas. 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property  
$namespace = New-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="get-azurermeventhubnamespace"></a>**Get-AzureRmEventHubNamespace**
- As propriedades "Status" e "Enabled" de NamespceAttributes irão ser removidas. 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="set-azurermeventhubnamespace"></a>**Set-AzureRmEventHubNamespace**
- As propriedades "Status" e "Enabled" de NamespceAttributes irão ser removidas. 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Set-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Set-AzureRmEventHubNamespace <parameters>
``` 
  
### <a name="new-azurermeventhubconsumergroup"></a>**New-AzureRmEventHubConsumerGroup**
- A propriedade "EventHubPath" de ConsumerGroupAttributes irá ser removida.

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a>**Set-AzureRmEventHubConsumerGroup**
- A propriedade "EventHubPath" de ConsumerGroupAttributes irá ser removida.

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a>**Get-AzureRmEventHubConsumerGroup**
- A propriedade "EventHubPath" de ConsumerGroupAttributes irá ser removida.

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a>Alterações recentes aos cmdlets de Insights

### <a name="add-azurermlogalertrule"></a>**Add-AzureRMLogAlertRule**
- O cmdlet **Add-AzureRMLogAlertRule** foi preterido
- Após 1 de outubro, a utilização deste cmdlet já não terá qualquer efeito uma vez que esta funcionalidade está transitar para os Alertas de Registo de Atividade. Para obter mais informações, veja https://aka.ms/migratemealerts.

### <a name="get-azurermusage"></a>**Get-AzureRMUsage**
- O cmdlet **Get-AzureRMUsage** foi preterido

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a>**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**
- Alteração na saída: o campo EventChannels do objeto EventData (devolvido por estes cmdlets) está em vias de ser preterido visto que agora devolve um valor constante (Admin,Operation).

### <a name="get-azurermalertrule"></a>**Get-AzureRmAlertRule**
- Alteração na saída: a saída deste cmdlet vai ser simplificada, o que significa a eliminação do campo de propriedades, para melhorar a experiência do utilizador.

```powershell-interactive
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

### <a name="get-azurermautoscalesetting"></a>**Get-AzureRmAutoscaleSetting**
- Alteração na saída: o campo AutoscaleSettingResourceName irá ser preterido, uma vez que equivale sempre ao campo Name.

```powershell-interactive
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

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a>**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**
- Alteração na saída: o tipo da saída vai ser alterado para devolver um único objeto que contém o ID do pedido e o código de estado.

```powershell-interactive
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

## <a name="breaking-changes-to-network-cmdlets"></a>Alterações recentes aos cmdlets de Rede

### <a name="add-azurermapplicationgatewaysslcertificate"></a>**Add-AzureRmApplicationGatewaySslCertificate**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a>**New-AzureRmApplicationGatewaySslCertificate**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a>**Set-AzureRmApplicationGatewaySslCertificate**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a>Alterações recentes aos cmdlets de Recursos

### <a name="new-azurermadappcredential"></a>**New-AzureRmADAppCredential**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a>**New-AzureRmADApplication**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a>**New-AzureRmADServicePrincipal**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a>**New-AzureRmADSpCredential**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a>**New-AzureRmADUser**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a>**Set-AzureRmADUser**
- O parâmetro "Password" está a ser substituído em prol de uma SecureString

```powershell-interactive
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a>Alterações recentes aos cmdlets de ServiceBus

### <a name="get-azurermservicebustopicauthorizationrule"></a>**Get-AzureRmServiceBusTopicAuthorizationRule**
- O cmdlet "Get-AzureRmServiceBusTopicAuthorizationRule" foi removido. Utilize o cmdlet "Get-AzureRmServiceBusAuthorizationRule".    

### <a name="get-azurermservicebustopickey"></a>**Get-AzureRmServiceBusTopicKey**
- O cmdlet "Get-AzureRmServiceBusTopicKey" foi removido. Utilize o cmdlet "Get-AzureRmServiceBusKey".

### <a name="new-azurermservicebustopicauthorizationrule"></a>**New-AzureRmServiceBusTopicAuthorizationRule**
- O cmdlet "New-AzureRmServiceBusTopicAuthorizationRule" foi removido. Utilize o cmdlet "New-AzureRmServiceBusAuthorizationRule".

### <a name="new-azurermservicebustopickey"></a>**New-AzureRmServiceBusTopicKey**
- O cmdlet "New-AzureRmServiceBusTopicKey" foi removido. Utilize o cmdlet "New-AzureRmServiceBusKey".

### <a name="remove-azurermservicebustopicauthorizationrule"></a>**Remove-AzureRmServiceBusTopicAuthorizationRule**
- O cmdlet "Remove-AzureRmServiceBusTopicAuthorizationRule" foi removido. Utilize o cmdlet "Remove-AzureRmServiceBusAuthorizationRule".

### <a name="set-azurermservicebustopicauthorizationrule"></a>**Set-AzureRmServiceBusTopicAuthorizationRule**
- O cmdlet "Set-AzureRmServiceBusTopicAuthorizationRule" foi removido. Utilize o cmdlet "Set-AzureRmServiceBusAuthorizationRule".

### <a name="new-azurermservicebusnamespacekey"></a>**New-AzureRmServiceBusNamespaceKey**
- O cmdlet "New-AzureRmServiceBusNamespaceKey" foi removido. Utilize o cmdlet "New-AzureRmServiceBusKey".

### <a name="get-azurermservicebusqueueauthorizationrule"></a>**Get-AzureRmServiceBusQueueAuthorizationRule**
- O cmdlet "Get-AzureRmServiceBusQueueAuthorizationRule" foi removido. Utilize o cmdlet "Get-AzureRmServiceBusAuthorizationRule".

### <a name="get-azurermservicebusqueuekey"></a>**Get-AzureRmServiceBusQueueKey**
- O cmdlet "Get-AzureRmServiceBusQueueKey" foi removido. Utilize o cmdlet "Get-AzureRmServiceBusKey".

### <a name="new-azurermservicebusqueueauthorizationrule"></a>**New-AzureRmServiceBusQueueAuthorizationRule**
- O cmdlet "New-AzureRmServiceBusQueueAuthorizationRule" foi removido. Utilize o cmdlet "New-AzureRmServiceBusAuthorizationRule".

### <a name="new-azurermservicebusqueuekey"></a>**New-AzureRmServiceBusQueueKey**
- O cmdlet "New-AzureRmServiceBusQueueKey" foi removido. Utilize o cmdlet "New-AzureRmServiceBusKey".

### <a name="remove-azurermservicebusqueueauthorizationrule"></a>**Remove-AzureRmServiceBusQueueAuthorizationRule**
- O cmdlet "Remove-AzureRmServiceBusQueueAuthorizationRule" foi removido. Utilize o cmdlet "GRemove-AzureRmServiceBusAuthorizationRule".

### <a name="set-azurermservicebusqueueauthorizationrule"></a>**Set-AzureRmServiceBusQueueAuthorizationRule**
- O cmdlet "Set-AzureRmServiceBusQueueAuthorizationRule" foi removido. Utilize o cmdlet "Set-AzureRmServiceBusAuthorizationRule".

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a>**Get-AzureRmServiceBusNamespaceAuthorizationRule**
- O cmdlet "Get-AzureRmServiceBusNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "Get-AzureRmServiceBusAuthorizationRule".

### <a name="get-azurermservicebusnamespacekey"></a>**Get-AzureRmServiceBusNamespaceKey**
- O cmdlet "Get-AzureRmServiceBusNamespaceKey" foi removido. Utilize o cmdlet "Get-AzureRmServiceBusKey".

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a>**New-AzureRmServiceBusNamespaceAuthorizationRule**
- O cmdlet "New-AzureRmServiceBusNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "New-AzureRmServiceBusAuthorizationRule".

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a>**Remove-AzureRmServiceBusNamespaceAuthorizationRule**
- O cmdlet "Remove-AzureRmServiceBusNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "Remove-AzureRmServiceBusAuthorizationRule".

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a>**Set-AzureRmServiceBusNamespaceAuthorizationRule**
- O cmdlet "Set-AzureRmServiceBusNamespaceAuthorizationRule" foi removido. Utilize o cmdlet "Set-AzureRmServiceBusAuthorizationRule".

### <a name="type-namespaceattributes"></a>**Tipo NamespaceAttributes**
- As seguintes propriedades foram removidas
    - Ativado
    - Estado
   
```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmServiceBusNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Enabled and Status properties    
$namespace = Get-AzureRmServiceBusNamespace <parameters>
```

### <a name="type-queueattribute"></a>**Tipo QueueAttribute**
- As seguintes propriedades estão marcadas como obsoletas:
    - EnableBatchedOperations
    - EntityAvailabilityStatus
    - IsAnonymousAccessible
    - SupportOrdering

```powershell-interactive
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
   
### <a name="type-topicattribute"></a>**Tipo TopicAttribute**
- As seguintes propriedades estão marcadas como obsoletas:
    - Localização
    - IsExpress
    - IsAnonymousAccessible
    - FilteringMessagesBeforePublishing
    - EnableSubscriptionPartitioning
    - EntityAvailabilityStatus

```powershell-interactive
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
   
### <a name="type-subscriptionattribute"></a>**Tipo SubscriptionAttribute**
- As seguintes propriedades estão marcadas como obsoletas
    - DeadLetteringOnFilterEvaluationExceptions
    - EntityAvailabilityStatus
    - IsReadOnly
    - Localização
   
```powershell-interactive
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