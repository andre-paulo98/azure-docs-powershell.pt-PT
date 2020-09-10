---
title: Consultar saída de cmdlets do Azure PowerShell
description: Como consultar recursos no Azure e formatar os resultados.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/10/2019
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 2754df5132ca9d528217fa5caad95b7f59cc8215
ms.sourcegitcommit: 2f1e3c275626fba1c4275cae8ef1d13b11f55735
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2020
ms.locfileid: "89449981"
---
# <a name="query-output-of-azure-powershell"></a>Consultar a saída do Azure PowerShell 

Os resultados de cada cmdlet do Azure PowerShell são um objeto do Azure PowerShell. Até os cmdlets que não são explicitamente operações `Get-` podem devolver um valor que pode ser inspecionado, para fornecer informações sobre um recurso que foi criado ou modificado. Embora a maioria dos cmdlets devolva um único objeto, alguns devolvem uma matriz que deve ser iterada.

Em quase todos os casos, irá consultar a saída do Azure PowerShell com o cmdlet [Select-Object](/powershell/module/Microsoft.PowerShell.Utility/Select-Object), frequentemente abreviado para `select`. A saída pode ser filtrada com [Where-Object](/powershell/module/Microsoft.PowerShell.Core/Where-Object) ou com o respetivo alias `where`.

## <a name="select-simple-properties"></a>Selecionar propriedades simples

No formato de tabela predefinido, os cmdlets do Azure PowerShell não apresentam todas as respetivas propriedades disponíveis. Pode obter as propriedades completas com o cmdlet [Format-List](/powershell/module/microsoft.powershell.utility/format-list) ou ao encaminhar a saída para `Select-Object *`:

```azurepowershell-interactive
Get-AzVM -Name TestVM -ResourceGroupName TestGroup | Select-Object *
```

```output
ResourceGroupName        : TESTGROUP
Id                       : /subscriptions/711d8ed1-b888-4c52-8ab9-66f07b87eb6b/resourceGroups/TESTGROUP/providers/Micro
                           soft.Compute/virtualMachines/TestVM
VmId                     : 711d8ed1-b888-4c52-8ab9-66f07b87eb6b
Name                     : TestVM
Type                     : Microsoft.Compute/virtualMachines
Location                 : westus2
LicenseType              :
Tags                     : {}
AvailabilitySetReference :
DiagnosticsProfile       :
Extensions               : {}
HardwareProfile          : Microsoft.Azure.Management.Compute.Models.HardwareProfile
InstanceView             :
NetworkProfile           : Microsoft.Azure.Management.Compute.Models.NetworkProfile
OSProfile                : Microsoft.Azure.Management.Compute.Models.OSProfile
Plan                     :
ProvisioningState        : Succeeded
StorageProfile           : Microsoft.Azure.Management.Compute.Models.StorageProfile
DisplayHint              : Compact
Identity                 :
Zones                    : {}
FullyQualifiedDomainName :
AdditionalCapabilities   :
RequestId                : 711d8ed1-b888-4c52-8ab9-66f07b87eb6b
StatusCode               : OK
```

Quando souber os nomes das propriedades em que está interessado, pode utilizar esses nomes de propriedades com `Select-Object` para obtê-los diretamente:

```azurepowershell-interactive
Get-AzVM -Name TestVM -ResourceGroupName TestGroup | Select-Object Name,VmId,ProvisioningState
```

```output
Name   VmId                                 ProvisioningState
----   ----                                 -----------------
TestVM 711d8ed1-b888-4c52-8ab9-66f07b87eb6b Succeeded
```

A saída resultante da utilização de `Select-Object` é sempre formatada para apresentar as informações pedidas. Para saber mais sobre como utilizar a formatação como parte da consulta de resultados de cmdlet, veja [Formatar a saída de cmdlet do Azure PowerShell](formatting-output.md).

## <a name="select-nested-properties"></a>Selecionar propriedades aninhadas

Algumas propriedades na saída de cmdlet do Azure PowerShell utilizam objetos aninhados, como a propriedade `StorageProfile` da saída `Get-AzVM`. Para obter um valor de uma propriedade aninhada, forneça um nome a apresentar e o caminho completo para o valor que quer inspecionar como parte de um argumento de dicionário para `Select-Object`:

```azurepowershell-interactive
Get-AzVM -ResourceGroupName TestGroup | `
    Select-Object Name,@{Name="OSType"; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```output
Name     OSType
----     ------
TestVM    Linux
TestVM2   Linux
WinVM   Windows
```

Cada argumento de dicionário seleciona uma propriedade do objeto. A propriedade a extrair tem de fazer parte de uma expressão.

## <a name="filter-results"></a>Filtrar os resultados 

O cmdlet `Where-Object` permite-lhe filtrar o resultado com base em qualquer valor de propriedade, incluindo propriedades aninhadas. O exemplo seguinte mostra como utilizar `Where-Object` para encontrar as VMs do Linux num grupo de recursos.

```azurepowershell-interactive
Get-AzVM -ResourceGroupName TestGroup | `
    Where-Object {$_.StorageProfile.OSDisk.OSType -eq "Linux"}
```

```output
ResourceGroupName    Name Location          VmSize OsType        NIC ProvisioningState Zone
-----------------    ---- --------          ------ ------        --- ----------------- ----
TestGroup          TestVM  westus2 Standard_D2s_v3  Linux  testvm299         Succeeded
TestGroup         TestVM2  westus2 Standard_D2s_v3  Linux testvm2669         Succeeded
```

Pode encaminhar os resultados de `Select-Object` e `Where-Object` entre um e outro. Por motivos de desempenho, recomendamos sempre que coloque a operação `Where-Object` antes de `Select-Object`:

```azurepowershell-interactive
Get-AzVM -ResourceGroupName TestGroup | `
    Where-Object {$_.StorageProfile.OsDisk.OsType -eq "Linux"} | `
    Select-Object Name,VmID,ProvisioningState
```

```output
Name    VmId                                 ProvisioningState
----    ----                                 -----------------
TestVM  711d8ed1-b888-4c52-8ab9-66f07b87eb6  Succeeded
TestVM2 cbcee769-dd78-45e3-a14d-2ad11c647d0  Succeeded
```
