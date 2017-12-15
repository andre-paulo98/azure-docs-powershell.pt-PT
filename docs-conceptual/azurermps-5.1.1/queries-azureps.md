---
title: "Consultar recursos e resultados de formatação do Azure | Microsoft Docs"
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
ms.openlocfilehash: 93a031ce90352286bb1a5e01dc65e6db7cbe5c7e
ms.sourcegitcommit: c42c7176276ec4e1cc3360a93e6b15d32083bf9f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/14/2017
---
# <a name="querying-for-azure-resources"></a><span data-ttu-id="c8df5-103">Consultar recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="c8df5-103">Querying for Azure resources</span></span>

<span data-ttu-id="c8df5-104">A consulta no PowerShell pode ser concluída através de cmdlets incorporados.</span><span class="sxs-lookup"><span data-stu-id="c8df5-104">Querying in PowerShell can be completed by using built-in cmdlets.</span></span> <span data-ttu-id="c8df5-105">No PowerShell, os nomes dos cmdlets têm a forma de  **_Verbo-Nome_**.</span><span class="sxs-lookup"><span data-stu-id="c8df5-105">In PowerShell, cmdlet names take the form of **_Verb-Noun_**.</span></span> <span data-ttu-id="c8df5-106">Os cmdlets com o verbo **_Get_** são os cmdlets de consulta.</span><span class="sxs-lookup"><span data-stu-id="c8df5-106">The cmdlets using the verb **_Get_** are the query cmdlets.</span></span> <span data-ttu-id="c8df5-107">Os nomes dos cmdlets são os tipos de recursos do Azure alterados pelos verbos dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c8df5-107">The cmdlet nouns are the types of Azure resources that are acted upon by the cmdlet verbs.</span></span>


## <a name="selecting-simple-properties"></a><span data-ttu-id="c8df5-108">Selecionar propriedades simples</span><span class="sxs-lookup"><span data-stu-id="c8df5-108">Selecting simple properties</span></span>

<span data-ttu-id="c8df5-109">O Azure PowerShell tem formatação predefinida para cada cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c8df5-109">Azure PowerShell has default formatting defined for each cmdlet.</span></span> <span data-ttu-id="c8df5-110">As propriedades mais comuns para cada tipo de recurso são apresentadas automaticamente num formato de tabela ou lista.</span><span class="sxs-lookup"><span data-stu-id="c8df5-110">The most common properties for each resource type are displayed in a table or list format automatically.</span></span> <span data-ttu-id="c8df5-111">Para obter mais informações sobre como formatar o resultado, veja [Formatar resultados da consulta](formatting-output.md).</span><span class="sxs-lookup"><span data-stu-id="c8df5-111">For more information about formatting output, see [Formatting query results](formatting-output.md).</span></span>

<span data-ttu-id="c8df5-112">Utilize o cmdlet `Get-AzureRmVM` para consultar uma lista de VMs na sua conta.</span><span class="sxs-lookup"><span data-stu-id="c8df5-112">Use the `Get-AzureRmVM` cmdlet to query for a list of VMs in your account.</span></span>

```powershell
Get-AzureRmVM
```

<span data-ttu-id="c8df5-113">O resultado predefinido é formatado automaticamente como uma tabela.</span><span class="sxs-lookup"><span data-stu-id="c8df5-113">The default output is automatically formatted as a table.</span></span>

```
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="c8df5-114">O cmdlet `Select-Object` pode ser utilizado para selecionar as propriedades específicas que lhe interessam.</span><span class="sxs-lookup"><span data-stu-id="c8df5-114">The `Select-Object` cmdlet can be used to select the specific properties that are interesting to you.</span></span>

```powershell
Get-AzureRmVM | Select Name,ResourceGroupName,Location
```

```
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

## <a name="selecting-complex-nested-properties"></a><span data-ttu-id="c8df5-115">Selecionar propriedades aninhadas complexas</span><span class="sxs-lookup"><span data-stu-id="c8df5-115">Selecting complex nested properties</span></span>

<span data-ttu-id="c8df5-116">Se a propriedade que quer selecionar estiver muito aninhada na saída JSON, tem de indicar o caminho completo para essa propriedade aninhada.</span><span class="sxs-lookup"><span data-stu-id="c8df5-116">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="c8df5-117">O exemplo seguinte mostra como selecionar o Nome da VM e o tipo de SO a partir do cmdlet `Get-AzureRmVM`.</span><span class="sxs-lookup"><span data-stu-id="c8df5-117">The following example shows how to select the VM Name and the OS type from the `Get-AzureRmVM` cmdlet.</span></span>

```powershell
Get-AzureRmVM | Select Name,@{Name='OSType'; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```
Name           OSType
----           ------
MyUnbuntu1610   Linux
MyWin2016VM   Windows
```

## <a name="filter-result-using-the-where-object-cmdlet"></a><span data-ttu-id="c8df5-118">Filtrar resultado com o cmdlet Where-Object</span><span class="sxs-lookup"><span data-stu-id="c8df5-118">Filter result using the Where-Object cmdlet</span></span>

<span data-ttu-id="c8df5-119">O cmdlet `Where-Object` permite filtrar o resultado com base em qualquer valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c8df5-119">The `Where-Object` cmdlet allows you to filter the result based on any property value.</span></span> <span data-ttu-id="c8df5-120">No exemplo seguinte, filtro seleciona apenas as VMs com o texto "RGD" no respetivo nome.</span><span class="sxs-lookup"><span data-stu-id="c8df5-120">In the following example, the filter selects only VMs that have the text "RGD" in their name.</span></span>

```powershell
Get-AzureRmVM | Where ResourceGroupName -like RGD* | Select ResourceGroupName,Name
```

```
ResourceGroupName  Name
-----------------  ----
RGDEMO001          KBDemo001VM
RGDEMO001          KBDemo020
```

<span data-ttu-id="c8df5-121">No próximo exemplo, os resultados vão devolver as VMs que tenham o tamanho de VM “Standard_DS1_V2”.</span><span class="sxs-lookup"><span data-stu-id="c8df5-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1_V2'.</span></span>

```powershell
Get-AzureRmVM | Where vmSize -eq Standard_DS1_V2
```

```
ResourceGroupName          Name     Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----     --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610   westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM   westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```
