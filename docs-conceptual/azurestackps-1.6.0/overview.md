---
title: Descrição Geral do módulo Azure Stack Admin do PowerShell | Microsoft Docs
description: Descrição geral do módulo Azure Stack Admin com instruções para instalação e configuração.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: b0e85bec82b9b7c876b2bbf337b603c8d68cf6a3
ms.sourcegitcommit: 4e1174236796e7da929ff276addb32e42c18b707
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/12/2019
ms.locfileid: "54240140"
---
# <a name="azure-stack-module-160"></a><span data-ttu-id="43943-103">Módulo 1.6.0 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="43943-103">Azure Stack Module 1.6.0</span></span>

## <a name="requirements"></a><span data-ttu-id="43943-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="43943-104">Requirements:</span></span>
<span data-ttu-id="43943-105">A versão mínima suportada do Azure Stack é a 1811.</span><span class="sxs-lookup"><span data-stu-id="43943-105">Minimum supported Azure Stack version is 1811.</span></span>

<span data-ttu-id="43943-106">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.6.0</span><span class="sxs-lookup"><span data-stu-id="43943-106">Note: If you are using an earlier version install version 1.6.0</span></span>

## <a name="install"></a><span data-ttu-id="43943-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="43943-107">Install</span></span>
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.6.0
```

## <a name="release-notes"></a><span data-ttu-id="43943-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="43943-108">Release Notes</span></span>
* <span data-ttu-id="43943-109">Suportado com a atualização 1811</span><span class="sxs-lookup"><span data-stu-id="43943-109">Supported with 1811 update</span></span>
* <span data-ttu-id="43943-110">Módulo Azs.Compute.Admin</span><span class="sxs-lookup"><span data-stu-id="43943-110">Azs.Compute.Admin Module</span></span>
    * <span data-ttu-id="43943-111">Foi corrigido o prefixo Azs em falta para New-DataDiskObject e foi adicionado o alias com aviso de preterição futura.</span><span class="sxs-lookup"><span data-stu-id="43943-111">Fixed missing Azs prefix for New-DataDiskObject and added alias with warning of future deprecation.</span></span>
* <span data-ttu-id="43943-112">Módulo Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="43943-112">Azs.Update.Admin Module</span></span>
    * <span data-ttu-id="43943-113">Foi adicionado um aviso para recomendar a execução de Test-AzureStack antes de Install-AzsUpdate</span><span class="sxs-lookup"><span data-stu-id="43943-113">Added a warning to recommend running Test-AzureStack before Install-AzsUpdate</span></span>
* <span data-ttu-id="43943-114">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="43943-114">Azs.Fabric.Admin</span></span>
    * <span data-ttu-id="43943-115">Novo cmdlet (as funcionalidades são suportadas pelo Azure Stack 1811+)</span><span class="sxs-lookup"><span data-stu-id="43943-115">New cmdlet (The features are supported by Azure Stack 1811+)</span></span>
        * <span data-ttu-id="43943-116">Get-AzsDrive</span><span class="sxs-lookup"><span data-stu-id="43943-116">Get-AzsDrive</span></span>
        * <span data-ttu-id="43943-117">Get-AzsVolume</span><span class="sxs-lookup"><span data-stu-id="43943-117">Get-AzsVolume</span></span>
        * <span data-ttu-id="43943-118">Get-AzsStorageSubSystem</span><span class="sxs-lookup"><span data-stu-id="43943-118">Get-AzsStorageSubSystem</span></span>
    * <span data-ttu-id="43943-119">Preterição</span><span class="sxs-lookup"><span data-stu-id="43943-119">Deprecation</span></span>
        * <span data-ttu-id="43943-120">Get-AzsInfrastructureVolume passa a ser um alias de cmdlet Get-AzsVolume</span><span class="sxs-lookup"><span data-stu-id="43943-120">Get-AzsInfrastructureVolume is an alias now to the cmdlet Get-AzsVolume</span></span>
* <span data-ttu-id="43943-121">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="43943-121">Azs.InfrastructureInsights.Admin</span></span>
    *  <span data-ttu-id="43943-122">Foi adicionado um novo cmdlet Repair-AzsAlert</span><span class="sxs-lookup"><span data-stu-id="43943-122">Added a new cmdlet Repair-AzsAlert</span></span>
* <span data-ttu-id="43943-123">Azs.Storage.Admin</span><span class="sxs-lookup"><span data-stu-id="43943-123">Azs.Storage.Admin</span></span>
    * <span data-ttu-id="43943-124">Correção de um erro em que os valores de quota predefinidos não estão a ser utilizados</span><span class="sxs-lookup"><span data-stu-id="43943-124">Bug fix where default quota values are not being used</span></span>
* <span data-ttu-id="43943-125">Módulo Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="43943-125">Azs.Subscriptions.Admin Module</span></span>
    * <span data-ttu-id="43943-126">Foi corrigido o prefixo Azs em falta para New-AddonPlanDefinitionObject e foi adicionado o alias com aviso de preterição futura.</span><span class="sxs-lookup"><span data-stu-id="43943-126">Fixed missing Azs prefix for New-AddonPlanDefinitionObject and added alias with warning of future deprecation.</span></span>
