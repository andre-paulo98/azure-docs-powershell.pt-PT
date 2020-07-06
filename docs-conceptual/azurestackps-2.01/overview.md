---
title: Descrição Geral do Azure Stack Hub Admin PowerShell | Microsoft Docs
description: Descrição geral do Azure Stack Hub Admin PowerShell com instruções de instalação e configuração.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 06/22/2020
ms.openlocfilehash: 860a32d120e203093038130a535e8b6801e2bce2
ms.sourcegitcommit: 199e9c800e58e88c4cbfd3f221bafe02b3e8294d
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/24/2020
ms.locfileid: "85306569"
---
# <a name="azure-stack-hub-module-201"></a><span data-ttu-id="4f842-103">Azure Stack Hub, Módulo 2.0.1</span><span class="sxs-lookup"><span data-stu-id="4f842-103">Azure Stack Hub Module 2.0.1</span></span>

## <a name="requirements"></a><span data-ttu-id="4f842-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="4f842-104">Requirements:</span></span>

<span data-ttu-id="4f842-105">A versão mínima suportada do Azure Stack Hub é a 2002.</span><span class="sxs-lookup"><span data-stu-id="4f842-105">Minimum supported Azure Stack Hub version is 2002.</span></span>

<span data-ttu-id="4f842-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="4f842-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="4f842-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="4f842-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Az.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue

Install-Module -Name Az.BootStrapper -Force -AllowPrerelease

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 2.0.1-preview -AllowPrerelease
```


## <a name="release-notes"></a><span data-ttu-id="4f842-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="4f842-108">Release Notes</span></span>

* <span data-ttu-id="4f842-109">Suportado com a atualização 2002.</span><span class="sxs-lookup"><span data-stu-id="4f842-109">Supported with 2002 update.</span></span>  

  <span data-ttu-id="4f842-110">O Azure Stack Hub 2.0.0 é uma alteração interruptiva.</span><span class="sxs-lookup"><span data-stu-id="4f842-110">The Azure Stack Hub 2.0.0 is a breaking change.</span></span> <span data-ttu-id="4f842-111">O módulo utiliza o módulo Az em vez do módulo AzureRM.</span><span class="sxs-lookup"><span data-stu-id="4f842-111">The module uses the Az module rather than the AzureRM module.</span></span> <span data-ttu-id="4f842-112">Pode encontrar um guia de migração e uma lista de alterações interruptivas em [Migrar do AzureRM para o Azure PowerShell Az no Azure Stack Hub](https://aka.ms/AA7qsji).</span><span class="sxs-lookup"><span data-stu-id="4f842-112">You can find a migration guide and a list of breaking changes in [Migrate from AzureRM to Azure PowerShell Az in Azure Stack Hub](https://aka.ms/AA7qsji).</span></span>
