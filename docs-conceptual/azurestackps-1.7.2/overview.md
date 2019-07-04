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
ms.openlocfilehash: b77e09f6fcd5b7752af9f51a42d357db4f1b13db
ms.sourcegitcommit: febbbd3f75c8dd1a296281d265289f015b6cb537
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/12/2019
ms.locfileid: "67037682"
---
# <a name="azure-stack-module-172"></a><span data-ttu-id="454d1-103">Módulo 1.7.2 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="454d1-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="454d1-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="454d1-104">Requirements:</span></span>

<span data-ttu-id="454d1-105">A versão mínima suportada do Azure Stack é a 1904.</span><span class="sxs-lookup"><span data-stu-id="454d1-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="454d1-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="454d1-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="454d1-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="454d1-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a><span data-ttu-id="454d1-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="454d1-108">Release Notes</span></span>

* <span data-ttu-id="454d1-109">Suportado com a atualização 1904</span><span class="sxs-lookup"><span data-stu-id="454d1-109">Supported with 1904 update</span></span>
* <span data-ttu-id="454d1-110">Esta é uma versão com uma alteração interruptiva.</span><span class="sxs-lookup"><span data-stu-id="454d1-110">This a breaking change release.</span></span> <span data-ttu-id="454d1-111">Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170></span><span class="sxs-lookup"><span data-stu-id="454d1-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="454d1-112">Alteração interruptiva: Alterações de segurança ao modo de encriptação baseada em certificados.</span><span class="sxs-lookup"><span data-stu-id="454d1-112">Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="454d1-113">O suporte de chaves simétricas foi preterido.</span><span class="sxs-lookup"><span data-stu-id="454d1-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="454d1-114">Para obter detalhes sobre as alterações interruptivas, veja https://aka.ms/azspshmigration170</span><span class="sxs-lookup"><span data-stu-id="454d1-114">For details on the breaking changes, refer to https://aka.ms/azspshmigration170</span></span>
* <span data-ttu-id="454d1-115">Módulo Azs.Storage.Admin</span><span class="sxs-lookup"><span data-stu-id="454d1-115">Azs.Storage.Admin Module</span></span> 
* <span data-ttu-id="454d1-116">Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma.</span><span class="sxs-lookup"><span data-stu-id="454d1-116">Bug fix - New Storage Quota uses defaults if none provided.</span></span>
