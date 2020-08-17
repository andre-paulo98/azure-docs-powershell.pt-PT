---
title: Descrição Geral do módulo Azure Stack Admin do PowerShell | Microsoft Docs
description: Descrição geral do módulo Azure Stack Admin com instruções para instalação e configuração.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 08/06/2020
ms.openlocfilehash: e314374eff433d1869378bdaa9a0370c3fd3d8d1
ms.sourcegitcommit: 09eb4dbfcad6fce303b793dafe9bebdef589db03
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/08/2020
ms.locfileid: "88022955"
---
# <a name="azure-stack-module-182"></a><span data-ttu-id="c91fc-103">Módulo 1.8.2 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c91fc-103">Azure Stack Module 1.8.2</span></span>

## <a name="requirements"></a><span data-ttu-id="c91fc-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="c91fc-104">Requirements:</span></span>

<span data-ttu-id="c91fc-105">A versão mínima suportada do Azure Stack é a 1910.</span><span class="sxs-lookup"><span data-stu-id="c91fc-105">Minimum supported Azure Stack version is 1910.</span></span>

<span data-ttu-id="c91fc-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="c91fc-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="c91fc-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="c91fc-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.8.2
```

## <a name="release-notes"></a><span data-ttu-id="c91fc-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="c91fc-108">Release Notes</span></span>

* <span data-ttu-id="c91fc-109">Suportado com a atualização 1910</span><span class="sxs-lookup"><span data-stu-id="c91fc-109">Supported with 1910 update</span></span>
