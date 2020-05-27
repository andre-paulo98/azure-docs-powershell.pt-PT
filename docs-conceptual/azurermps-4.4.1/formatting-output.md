---
title: Formatar resultados de consulta | Microsoft Docs
description: Como consultar recursos no Azure e formatar os resultados.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: a76ceee5ae1172630d74afd3c671031592d78a8b
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386770"
---
# <a name="formatting-query-results"></a><span data-ttu-id="5f71c-103">Formatar resultados de consulta</span><span class="sxs-lookup"><span data-stu-id="5f71c-103">Formatting query results</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="5f71c-104">Por predefinição, cada cmdlet do PowerShell possui formatação de saída predefinida, facilitando a leitura.</span><span class="sxs-lookup"><span data-stu-id="5f71c-104">By default each PowerShell cmdlet has predefined formatting of output making it easy to read.</span></span>  <span data-ttu-id="5f71c-105">O PowerShell fornece também a flexibilidade para ajustar a saída ou converter a saída do cmdlet num formato diferente com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5f71c-105">PowerShell also provides the flexibility to adjust the output or convert the cmdlet output to a different format with the following cmdlets:</span></span>

| <span data-ttu-id="5f71c-106">Formatação</span><span class="sxs-lookup"><span data-stu-id="5f71c-106">Formatting</span></span>      | <span data-ttu-id="5f71c-107">Conversão</span><span class="sxs-lookup"><span data-stu-id="5f71c-107">Conversion</span></span>       |
|-----------------|------------------|
| `Format-Custom` | `ConvertTo-Csv`  |
| `Format-List`   | `ConvertTo-Html` |
| `Format-Table`  | `ConvertTo-Json` |
| `Format-Wide`   | `ConvertTo-Xml`  |

## <a name="formatting-examples"></a><span data-ttu-id="5f71c-108">Exemplos de formatação</span><span class="sxs-lookup"><span data-stu-id="5f71c-108">Formatting examples</span></span>

<span data-ttu-id="5f71c-109">Neste exemplo obtemos uma lista de VMs do Azure na nossa subscrição predefinida.</span><span class="sxs-lookup"><span data-stu-id="5f71c-109">In this example we get a list of Azure VMs in our default subscription.</span></span>  <span data-ttu-id="5f71c-110">O comando Get-AzureRmVM predefine a saída para um formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="5f71c-110">The Get-AzureRmVM command defaults output into a table format.</span></span>

```powershell-interactive
Get-AzureRmVM
```

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="5f71c-111">Se pretende limitar as colunas devolvidas pode utilizar o cmdlet `Format-Table`.</span><span class="sxs-lookup"><span data-stu-id="5f71c-111">If you would like to limit the columns returned you can use the `Format-Table` cmdlet.</span></span> <span data-ttu-id="5f71c-112">No exemplo seguinte obtemos a mesma lista de máquinas virtuais, mas restringimos a saída para apenas o nome da VM, o grupo de recursos e a localização da VM.</span><span class="sxs-lookup"><span data-stu-id="5f71c-112">In the following example we get the same list of virtual machines but restrict the output to just the name of the VM, the resource group, and the location of the VM.</span></span>  <span data-ttu-id="5f71c-113">O parâmetro `-Autosize` define o tamanho das colunas, de acordo com o tamanho dos dados.</span><span class="sxs-lookup"><span data-stu-id="5f71c-113">The `-Autosize` parameter sizes the columns according to the size of the data.</span></span>

```powershell-interactive
Get-AzureRmVM | Format-Table Name,ResourceGroupName,Location -AutoSize
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

<span data-ttu-id="5f71c-114">Se preferir, pode visualizar as informações em formato de lista.</span><span class="sxs-lookup"><span data-stu-id="5f71c-114">If you would prefer you can view information in a list format.</span></span> <span data-ttu-id="5f71c-115">O exemplo seguinte mostra este utilizando o cmdlet `Format-List`.</span><span class="sxs-lookup"><span data-stu-id="5f71c-115">The following example shows this using the`Format-List` cmdlet.</span></span>

```powershell-interactive
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

## <a name="converting-to-other-data-types"></a><span data-ttu-id="5f71c-116">Converter para outros tipos de dados</span><span class="sxs-lookup"><span data-stu-id="5f71c-116">Converting to other data types</span></span>

<span data-ttu-id="5f71c-117">O PowerShell também oferece vários formatos de saída que pode utilizar para corresponder às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="5f71c-117">PowerShell also offers multiple output format you can use to meet your needs.</span></span>  <span data-ttu-id="5f71c-118">No exemplo seguinte utilizamos o cmdlet `Select-Object` para obter os atributos das máquinas virtuais na nossa subscrição e para converter o resultado em formato CSV para uma importação mais fácil numa base de dados ou folha de cálculo.</span><span class="sxs-lookup"><span data-stu-id="5f71c-118">In the following example we use the `Select-Object` cmdlet to get attributes of the virtual machines in our subscription and convert the output to CSV format for easy import into a database or spreadsheet.</span></span>

```powershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Csv -NoTypeInformation
```

```output
"ResourceGroupName","Id","VmId","Name","Location","ProvisioningState"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610","33422f9b-e339-4704-bad8-dbe094585496","MyUnbuntu1610","westeurope","Succeeded"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM","4650c755-fc2b-4fc7-a5bc-298d5c00808f","MyWin2016VM","westeurope","Succeeded"
```

<span data-ttu-id="5f71c-119">Também pode converter o resultado no formato JSON.</span><span class="sxs-lookup"><span data-stu-id="5f71c-119">You can also convert the output into JSON format.</span></span>  <span data-ttu-id="5f71c-120">O exemplo seguinte cria a mesma lista de VMs mas altera o formato de saída para JSON.</span><span class="sxs-lookup"><span data-stu-id="5f71c-120">The following example creates the same list of VMs but changes the output format to JSON.</span></span>

```powershell-interactive
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
