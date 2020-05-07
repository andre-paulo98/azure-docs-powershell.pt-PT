---
title: Descrição Geral do Azure Stack Hub Admin PowerShell | Microsoft Docs
description: Descrição geral do Azure Stack Hub Admin PowerShell com instruções de instalação e configuração.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 04/16/2020
ms.openlocfilehash: fd1f2a3778e348ba41b46acb4bdce19e18a7f4ec
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "81524970"
---
# <a name="azure-stack-hub-module-200"></a><span data-ttu-id="23a23-103">Azure Stack Hub, Módulo 2.0.0</span><span class="sxs-lookup"><span data-stu-id="23a23-103">Azure Stack Hub Module 2.0.0</span></span>

## <a name="requirements"></a><span data-ttu-id="23a23-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="23a23-104">Requirements:</span></span>

<span data-ttu-id="23a23-105">A versão mínima suportada do Azure Stack Hub é a 2002.</span><span class="sxs-lookup"><span data-stu-id="23a23-105">Minimum supported Azure Stack Hub version is 2002.</span></span>

<span data-ttu-id="23a23-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="23a23-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="23a23-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="23a23-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Az.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue

Install-Module -Name Az.BootStrapper -Force -AllowPrerelease

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 2.0.0-preview -AllowPrerelease
```


## <a name="release-notes"></a><span data-ttu-id="23a23-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="23a23-108">Release Notes</span></span>

* <span data-ttu-id="23a23-109">Suportado com a atualização 2002.</span><span class="sxs-lookup"><span data-stu-id="23a23-109">Supported with 2002 update.</span></span>  

  <span data-ttu-id="23a23-110">O Azure Stack Hub 2.0.0 é uma alteração interruptiva.</span><span class="sxs-lookup"><span data-stu-id="23a23-110">The Azure Stack Hub 2.0.0 is a breaking change.</span></span> <span data-ttu-id="23a23-111">O módulo utiliza o módulo Az em vez do módulo AzureRM.</span><span class="sxs-lookup"><span data-stu-id="23a23-111">The module uses the Az module rather than the AzureRM module.</span></span> <span data-ttu-id="23a23-112">Pode encontrar um guia de migração e uma lista de alterações interruptivas em [Migrar do AzureRM para o Azure PowerShell Az no Azure Stack Hub](https://aka.ms/AA7qsji).</span><span class="sxs-lookup"><span data-stu-id="23a23-112">You can find a migration guide and a list of breaking changes in [Migrate from AzureRM to Azure PowerShell Az in Azure Stack Hub](https://aka.ms/AA7qsji).</span></span>
