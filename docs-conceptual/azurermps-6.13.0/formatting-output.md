---
title: Formatar a saída de cmdlets do Azure PowerShell
description: Como formatar a saída de cmdlets do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 6a35024e1bac819fa9b69174195e5245361cb7cc
ms.sourcegitcommit: bbd3f061cac3417ce588487c1ae4e0bc52c11d6a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/11/2019
ms.locfileid: "65535006"
---
# <a name="format-azurepowershell-cmdlet-output"></a><span data-ttu-id="73981-103">Formatar a saída de cmdlets do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="73981-103">Format AzurePowerShell cmdlet output</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="73981-104">Por predefinição, cada cmdlet do Azure PowerShell inclui formatação de saída predefinida, o que facilita a respetiva leitura.</span><span class="sxs-lookup"><span data-stu-id="73981-104">By default each Azure PowerShell cmdlet has predefined formatting of output making it easy to read.</span></span>  <span data-ttu-id="73981-105">O PowerShell fornece também a flexibilidade para ajustar a saída ou converter a saída do cmdlet num formato diferente com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="73981-105">PowerShell also provides the flexibility to adjust the output or convert the cmdlet output to a different format with the following cmdlets:</span></span>

| <span data-ttu-id="73981-106">Formatação</span><span class="sxs-lookup"><span data-stu-id="73981-106">Formatting</span></span>      | <span data-ttu-id="73981-107">Conversão</span><span class="sxs-lookup"><span data-stu-id="73981-107">Conversion</span></span>       |
|-----------------|------------------|
| [<span data-ttu-id="73981-108">Format-Custom</span><span class="sxs-lookup"><span data-stu-id="73981-108">Format-Custom</span></span>](/powershell/module/microsoft.powershell.utility/format-custom) | [<span data-ttu-id="73981-109">ConvertTo-Csv</span><span class="sxs-lookup"><span data-stu-id="73981-109">ConvertTo-Csv</span></span>](/powershell/module/microsoft.powershell.utility/convertto-csv)  |
| [<span data-ttu-id="73981-110">Format-List</span><span class="sxs-lookup"><span data-stu-id="73981-110">Format-List</span></span>](/powershell/module/microsoft.powershell.utility/format-list)   | [<span data-ttu-id="73981-111">ConvertTo-Html</span><span class="sxs-lookup"><span data-stu-id="73981-111">ConvertTo-Html</span></span>](/powershell/module/microsoft.powershell.utility/convertto-html) |
| [<span data-ttu-id="73981-112">Format-Table</span><span class="sxs-lookup"><span data-stu-id="73981-112">Format-Table</span></span>](/powershell/module/microsoft.powershell.utility/format-table)  | [<span data-ttu-id="73981-113">ConvertTo-Json</span><span class="sxs-lookup"><span data-stu-id="73981-113">ConvertTo-Json</span></span>](/powershell/module/microsoft.powershell.utility/convertto-json) |
| [<span data-ttu-id="73981-114">Format-Wide</span><span class="sxs-lookup"><span data-stu-id="73981-114">Format-Wide</span></span>](/powershell/module/microsoft.powershell.utility/format-wide)   | [<span data-ttu-id="73981-115">ConvertTo-Xml</span><span class="sxs-lookup"><span data-stu-id="73981-115">ConvertTo-Xml</span></span>](/powershell/module/microsoft.powershell.utility/convertto-xml)  |

## <a name="format-examples"></a><span data-ttu-id="73981-116">Exemplos de formato</span><span class="sxs-lookup"><span data-stu-id="73981-116">Format examples</span></span>

<span data-ttu-id="73981-117">Neste exemplo obtemos uma lista de VMs do Azure na nossa subscrição predefinida.</span><span class="sxs-lookup"><span data-stu-id="73981-117">In this example, we get a list of Azure VMs in our default subscription.</span></span>  <span data-ttu-id="73981-118">O comando `Get-AzureRmVM` predefine a saída para um formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="73981-118">The `Get-AzureRmVM` command defaults output into a table format.</span></span>

```azurepowershell-interactive
Get-AzureRmVM
```

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="73981-119">Se pretende limitar as colunas devolvidas pode utilizar o cmdlet `Format-Table`.</span><span class="sxs-lookup"><span data-stu-id="73981-119">If you would like to limit the columns returned you can use the `Format-Table` cmdlet.</span></span> <span data-ttu-id="73981-120">No exemplo seguinte obtemos a mesma lista de máquinas virtuais, mas restringimos a saída para apenas o nome da VM, o grupo de recursos e a localização da VM.</span><span class="sxs-lookup"><span data-stu-id="73981-120">In the following example, we get the same list of virtual machines but restrict the output to just the name of the VM, the resource group, and the location of the VM.</span></span>  <span data-ttu-id="73981-121">O parâmetro `-Autosize` define o tamanho das colunas, de acordo com o tamanho dos dados.</span><span class="sxs-lookup"><span data-stu-id="73981-121">The `-Autosize` parameter sizes the columns according to the size of the data.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Format-Table Name,ResourceGroupName,Location -AutoSize
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

<span data-ttu-id="73981-122">A saída também pode ser formatada numa lista.</span><span class="sxs-lookup"><span data-stu-id="73981-122">Output can also be formatted into a list.</span></span> <span data-ttu-id="73981-123">O exemplo seguinte mostra este utilizando o cmdlet `Format-List`.</span><span class="sxs-lookup"><span data-stu-id="73981-123">The following example shows this using the`Format-List` cmdlet.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Format-List Name,VmId,Location,ResourceGroupName
```

```output
Name              : MyUnbuntu1610
VmId              : 33422f9b-e339-4704-bad8-dbe094585496
Location          : westeurope
ResourceGroupName : MYWESTEURG

Name              : MyWin2016VM
VmId              : 4650c755-fc2b-4fc7-a5bc-298d5c00808f
Location          : westeurope
ResourceGroupName : MYWESTEURG
```

## <a name="convert-to-other-data-types"></a><span data-ttu-id="73981-124">Converter noutros tipos de dados</span><span class="sxs-lookup"><span data-stu-id="73981-124">Convert to other data types</span></span>

<span data-ttu-id="73981-125">O PowerShell também permite converter a saída de comandos em vários formatos de dados.</span><span class="sxs-lookup"><span data-stu-id="73981-125">PowerShell also allows taking command output and converting it into multiple data formats.</span></span> <span data-ttu-id="73981-126">No exemplo seguinte, o cmdlet `Select-Object` serve para obter os atributos das máquinas virtuais da subscrição e converter a saída em formato CSV a fim de facilitar a importação para uma base de dados ou folha de cálculo.</span><span class="sxs-lookup"><span data-stu-id="73981-126">In the following example, the `Select-Object` cmdlet is used to get attributes of the virtual machines in our subscription and convert the output to CSV format for easy import into a database or spreadsheet.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Csv -NoTypeInformation
```

```output
"ResourceGroupName","Id","VmId","Name","Location","ProvisioningState"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610","33422f9b-e339-4704-bad8-dbe094585496","MyUnbuntu1610","westeurope","Succeeded"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM","4650c755-fc2b-4fc7-a5bc-298d5c00808f","MyWin2016VM","westeurope","Succeeded"
```

<span data-ttu-id="73981-127">A saída também pode ser convertida no formato JSON.</span><span class="sxs-lookup"><span data-stu-id="73981-127">Output can also be converted into the JSON format.</span></span>  <span data-ttu-id="73981-128">O exemplo seguinte cria a mesma lista de VMs mas altera o formato de saída para JSON.</span><span class="sxs-lookup"><span data-stu-id="73981-128">The following example creates the same list of VMs but changes the output format to JSON.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Json
```

```output
[
    {
        "ResourceGroupName":  "MYWESTEURG",
        "Id":  "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTEURG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610",
        "VmId":  "33422f9b-e339-4704-bad8-dbe094585496",
        "Name":  "MyUnbuntu1610",
        "Location":  "westeurope",
        "ProvisioningState":  "Succeeded"
    },
    {
        "ResourceGroupName":  "MYWESTEURG",
        "Id":  "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTEURG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM",
        "VmId":  "4650c755-fc2b-4fc7-a5bc-298d5c00808f",
        "Name":  "MyWin2016VM",
        "Location":  "westeurope",
        "ProvisioningState":  "Succeeded"
    }
]
```
