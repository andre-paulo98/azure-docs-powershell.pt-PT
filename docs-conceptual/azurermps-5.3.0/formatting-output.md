---
title: Formatar resultados de consulta | Microsoft Docs
description: Como consultar recursos no Azure e formatar os resultados.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 916cf8590de89762bade4f01ce5a502383d51796
ms.sourcegitcommit: 7e77fe7ecd2112d6b4515517509c5c723e750e27
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/19/2018
---
# <a name="formatting-query-results"></a><span data-ttu-id="c4c16-103">Formatar resultados de consulta</span><span class="sxs-lookup"><span data-stu-id="c4c16-103">Formatting query results</span></span>

<span data-ttu-id="c4c16-104">Por predefinição, cada cmdlet do PowerShell possui formatação de saída predefinida, facilitando a leitura.</span><span class="sxs-lookup"><span data-stu-id="c4c16-104">By default each PowerShell cmdlet has predefined formatting of output making it easy to read.</span></span>  <span data-ttu-id="c4c16-105">O PowerShell fornece também a flexibilidade para ajustar a saída ou converter a saída do cmdlet num formato diferente com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c4c16-105">PowerShell also provides the flexibility to adjust the output or convert the cmdlet output to a different format with the following cmdlets:</span></span>

| <span data-ttu-id="c4c16-106">Formatação</span><span class="sxs-lookup"><span data-stu-id="c4c16-106">Formatting</span></span>      | <span data-ttu-id="c4c16-107">Conversão</span><span class="sxs-lookup"><span data-stu-id="c4c16-107">Conversion</span></span>       |
|-----------------|------------------|
| `Format-Custom` | `ConvertTo-Csv`  |
| `Format-List`   | `ConvertTo-Html` |
| `Format-Table`  | `ConvertTo-Json` |
| `Format-Wide`   | `ConvertTo-Xml`  |

## <a name="formatting-examples"></a><span data-ttu-id="c4c16-108">Exemplos de formatação</span><span class="sxs-lookup"><span data-stu-id="c4c16-108">Formatting examples</span></span>

<span data-ttu-id="c4c16-109">Neste exemplo obtemos uma lista de VMs do Azure na nossa subscrição predefinida.</span><span class="sxs-lookup"><span data-stu-id="c4c16-109">In this example we get a list of Azure VMs in our default subscription.</span></span>  <span data-ttu-id="c4c16-110">O comando Get-AzureRmVM predefine a saída para um formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="c4c16-110">The Get-AzureRmVM command defaults output into a table format.</span></span>

```powershell
Get-AzureRmVM
```

```
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="c4c16-111">Se pretende limitar as colunas devolvidas pode utilizar o cmdlet `Format-Table`.</span><span class="sxs-lookup"><span data-stu-id="c4c16-111">If you would like to limit the columns returned you can use the `Format-Table` cmdlet.</span></span> <span data-ttu-id="c4c16-112">No exemplo seguinte obtemos a mesma lista de máquinas virtuais, mas restringimos a saída para apenas o nome da VM, o grupo de recursos e a localização da VM.</span><span class="sxs-lookup"><span data-stu-id="c4c16-112">In the following example we get the same list of virtual machines but restrict the output to just the name of the VM, the resource group, and the location of the VM.</span></span>  <span data-ttu-id="c4c16-113">O parâmetro `-Autosize` define o tamanho das colunas, de acordo com o tamanho dos dados.</span><span class="sxs-lookup"><span data-stu-id="c4c16-113">The `-Autosize` parameter sizes the columns according to the size of the data.</span></span>

```powershell
Get-AzureRmVM | Format-Table Name,ResourceGroupName,Location -AutoSize
```

```
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

<span data-ttu-id="c4c16-114">Se preferir, pode visualizar as informações em formato de lista.</span><span class="sxs-lookup"><span data-stu-id="c4c16-114">If you would prefer you can view information in a list format.</span></span> <span data-ttu-id="c4c16-115">O exemplo seguinte mostra este utilizando o cmdlet `Format-List`.</span><span class="sxs-lookup"><span data-stu-id="c4c16-115">The following example shows this using the`Format-List` cmdlet.</span></span>

```powershell
Get-AzureRmVM | Format-List Name,VmId,Location,ResourceGroupName
```

```
Name              : MyUnbuntu1610
VmId              : 33422f9b-e339-4704-bad8-dbe094585496
Location          : westeurope
ResourceGroupName : MYWESTEURG

Name              : MyWin2016VM
VmId              : 4650c755-fc2b-4fc7-a5bc-298d5c00808f
Location          : westeurope
ResourceGroupName : MYWESTEURG
```

## <a name="converting-to-other-data-types"></a><span data-ttu-id="c4c16-116">Converter para outros tipos de dados</span><span class="sxs-lookup"><span data-stu-id="c4c16-116">Converting to other data types</span></span>

<span data-ttu-id="c4c16-117">O PowerShell também oferece vários formatos de saída que pode utilizar para corresponder às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="c4c16-117">PowerShell also offers multiple output format you can use to meet your needs.</span></span>  <span data-ttu-id="c4c16-118">No exemplo seguinte utilizamos o cmdlet `Select-Object` para obter os atributos das máquinas virtuais na nossa subscrição e para converter o resultado em formato CSV para uma importação mais fácil numa base de dados ou folha de cálculo.</span><span class="sxs-lookup"><span data-stu-id="c4c16-118">In the following example we use the `Select-Object` cmdlet to get attributes of the virtual machines in our subscription and and convert the output to CSV format for easy import into a database or spreadsheet.</span></span>

```powershell
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Csv -NoTypeInformation
```

```
"ResourceGroupName","Id","VmId","Name","Location","ProvisioningState"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610","33422f9b-e339-4704-bad8-dbe094585496","MyUnbuntu1610","westeurope","Succeeded"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM","4650c755-fc2b-4fc7-a5bc-298d5c00808f","MyWin2016VM","westeurope","Succeeded"
```

<span data-ttu-id="c4c16-119">Também pode converter o resultado no formato JSON.</span><span class="sxs-lookup"><span data-stu-id="c4c16-119">You can also convert the output into JSON format.</span></span>  <span data-ttu-id="c4c16-120">O exemplo seguinte cria a mesma lista de VMs mas altera o formato de saída para JSON.</span><span class="sxs-lookup"><span data-stu-id="c4c16-120">The following example creates the same list of VMs but changes the output format to JSON.</span></span>

```powershell
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Json
```

```
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
