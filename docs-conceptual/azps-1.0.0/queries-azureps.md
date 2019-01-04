---
title: Consultar saída de cmdlets do Azure PowerShell
description: Como consultar recursos no Azure e formatar os resultados.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: fd0135f981452a2425f4dc8b9c9708d4907eff2a
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594974"
---
# <a name="query-output-of-azure-powershell-cmdlets"></a><span data-ttu-id="f48bf-103">Consultar saída de cmdlets do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f48bf-103">Query output of Azure PowerShell cmdlets</span></span>

<span data-ttu-id="f48bf-104">A consulta no PowerShell pode ser concluída através de cmdlets incorporados.</span><span class="sxs-lookup"><span data-stu-id="f48bf-104">Querying in PowerShell can be completed by using built-in cmdlets.</span></span> <span data-ttu-id="f48bf-105">No PowerShell, os nomes dos cmdlets têm a forma de  **_Verbo-Nome_**.</span><span class="sxs-lookup"><span data-stu-id="f48bf-105">In PowerShell, cmdlet names take the form of **_Verb-Noun_**.</span></span> <span data-ttu-id="f48bf-106">Os cmdlets com o verbo **_Get_** são os cmdlets de consulta.</span><span class="sxs-lookup"><span data-stu-id="f48bf-106">The cmdlets using the verb **_Get_** are the query cmdlets.</span></span> <span data-ttu-id="f48bf-107">Os nomes dos cmdlets são os tipos de recursos do Azure alterados pelos verbos dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="f48bf-107">The cmdlet nouns are the types of Azure resources that are acted upon by the cmdlet verbs.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="f48bf-108">Selecionar propriedades simples</span><span class="sxs-lookup"><span data-stu-id="f48bf-108">Select simple properties</span></span>

<span data-ttu-id="f48bf-109">O Azure PowerShell tem formatação predefinida para cada cmdlet.</span><span class="sxs-lookup"><span data-stu-id="f48bf-109">Azure PowerShell has default formatting defined for each cmdlet.</span></span> <span data-ttu-id="f48bf-110">As propriedades mais comuns para cada tipo de recurso são apresentadas automaticamente num formato de tabela ou lista.</span><span class="sxs-lookup"><span data-stu-id="f48bf-110">The most common properties for each resource type are displayed in a table or list format automatically.</span></span> <span data-ttu-id="f48bf-111">Para obter mais informações sobre como formatar o resultado, veja [Formatar resultados da consulta](formatting-output.md).</span><span class="sxs-lookup"><span data-stu-id="f48bf-111">For more information about formatting output, see [Formatting query results](formatting-output.md).</span></span>

<span data-ttu-id="f48bf-112">Utilize o cmdlet `Get-AzVM` para consultar uma lista de VMs na sua conta.</span><span class="sxs-lookup"><span data-stu-id="f48bf-112">Use the `Get-AzVM` cmdlet to query for a list of VMs in your account.</span></span>

```azurepowershell-interactive
Get-AzVM
```

<span data-ttu-id="f48bf-113">O resultado predefinido é formatado automaticamente como uma tabela.</span><span class="sxs-lookup"><span data-stu-id="f48bf-113">The default output is automatically formatted as a table.</span></span>

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="f48bf-114">O cmdlet `Select-Object` pode ser utilizado para selecionar as propriedades específicas que lhe interessam.</span><span class="sxs-lookup"><span data-stu-id="f48bf-114">The `Select-Object` cmdlet can be used to select the specific properties that are interesting to you.</span></span>

```azurepowershell-interactive
Get-AzVM | Select Name,ResourceGroupName,Location
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

## <a name="select-complex-nested-properties"></a><span data-ttu-id="f48bf-115">Selecionar propriedades aninhadas complexas</span><span class="sxs-lookup"><span data-stu-id="f48bf-115">Select complex nested properties</span></span>

<span data-ttu-id="f48bf-116">Se a propriedade que quer estiver aninhada na saída JSON, tem de indicar o caminho completo para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="f48bf-116">If the property you want is nested in the JSON output, you need to supply the full path to the property.</span></span> <span data-ttu-id="f48bf-117">O exemplo seguinte mostra como selecionar o Nome da VM e o tipo de SO a partir do cmdlet `Get-AzVM`.</span><span class="sxs-lookup"><span data-stu-id="f48bf-117">The following example shows how to select the VM Name and the OS type from the `Get-AzVM` cmdlet.</span></span>

```azurepowershell-interactive
Get-AzVM | Select Name,@{Name='OSType'; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```output
Name           OSType
----           ------
MyUnbuntu1610   Linux
MyWin2016VM   Windows
```

## <a name="filter-results-with-the-where-object-cmdlet"></a><span data-ttu-id="f48bf-118">Filtrar resultados com o cmdlet Where-Object</span><span class="sxs-lookup"><span data-stu-id="f48bf-118">Filter results with the Where-Object cmdlet</span></span>

<span data-ttu-id="f48bf-119">O cmdlet `Where-Object` permite filtrar o resultado com base em qualquer valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f48bf-119">The `Where-Object` cmdlet allows you to filter the result based on any property value.</span></span> <span data-ttu-id="f48bf-120">No exemplo seguinte, filtro seleciona apenas as VMs com o texto "RGD" no respetivo nome.</span><span class="sxs-lookup"><span data-stu-id="f48bf-120">In the following example, the filter selects only VMs that have the text "RGD" in their name.</span></span>

```azurepowershell-interactive
Get-AzVM | Where ResourceGroupName -like RGD* | Select ResourceGroupName,Name
```

```output
ResourceGroupName  Name
-----------------  ----
RGDEMO001          KBDemo001VM
RGDEMO001          KBDemo020
```

<span data-ttu-id="f48bf-121">No próximo exemplo, os resultados vão devolver as VMs que tenham o tamanho de VM “Standard_DS1_V2”.</span><span class="sxs-lookup"><span data-stu-id="f48bf-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1_V2'.</span></span>

```azurepowershell-interactive
Get-AzVM | Where vmSize -eq Standard_DS1_V2
```

```output
ResourceGroupName          Name     Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----     --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610   westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM   westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```