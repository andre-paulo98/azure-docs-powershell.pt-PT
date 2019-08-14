---
title: Descrição Geral do módulo Azure Stack Admin do PowerShell | Microsoft Docs
description: Descrição geral do módulo Azure Stack Admin com instruções para instalação e configuração.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/06/2019
ms.openlocfilehash: 1b3d707e862dd0c21e9e6b0a89f429ff21b1a99d
ms.sourcegitcommit: b02cbcd00748a4a9a4790a5fba229ce53c3bf973
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/09/2019
ms.locfileid: "68861351"
---
# <a name="azure-stack-module-172"></a><span data-ttu-id="f5878-103">Módulo 1.7.2 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f5878-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="f5878-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="f5878-104">Requirements:</span></span>

<span data-ttu-id="f5878-105">A versão mínima suportada do Azure Stack é a 1904.</span><span class="sxs-lookup"><span data-stu-id="f5878-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="f5878-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="f5878-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="f5878-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="f5878-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a><span data-ttu-id="f5878-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="f5878-108">Release Notes</span></span>

* <span data-ttu-id="f5878-109">Suportado com a atualização 1904</span><span class="sxs-lookup"><span data-stu-id="f5878-109">Supported with 1904 update</span></span>
* <span data-ttu-id="f5878-110">Esta é uma versão com uma alteração interruptiva.</span><span class="sxs-lookup"><span data-stu-id="f5878-110">This a breaking change release.</span></span> <span data-ttu-id="f5878-111">Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170></span><span class="sxs-lookup"><span data-stu-id="f5878-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="f5878-112">Alteração interruptiva: Alterações de segurança ao modo de encriptação baseada em certificados.</span><span class="sxs-lookup"><span data-stu-id="f5878-112">Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="f5878-113">O suporte de chaves simétricas foi preterido.</span><span class="sxs-lookup"><span data-stu-id="f5878-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="f5878-114">Para obter detalhes sobre as alterações interruptivas, veja https://aka.ms/azspshmigration170</span><span class="sxs-lookup"><span data-stu-id="f5878-114">For details on the breaking changes, refer to https://aka.ms/azspshmigration170</span></span>
* <span data-ttu-id="f5878-115">Módulo Azs.Storage.Admin</span><span class="sxs-lookup"><span data-stu-id="f5878-115">Azs.Storage.Admin Module</span></span> 
* <span data-ttu-id="f5878-116">Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma.</span><span class="sxs-lookup"><span data-stu-id="f5878-116">Bug fix - New Storage Quota uses defaults if none provided.</span></span>
