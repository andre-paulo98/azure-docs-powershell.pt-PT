---
title: Descrição Geral do módulo Azure Stack Admin do PowerShell | Microsoft Docs
description: Descrição geral do módulo Azure Stack Admin com instruções para instalação e configuração.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/24/2020
ms.openlocfilehash: ec406c80de6b457f7e340a23fe8caf2ab83be46a
ms.sourcegitcommit: a6f2fc500242de6248224278d743fd09aac2fafd
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2020
ms.locfileid: "78264415"
---
# <a name="azure-stack-module-180"></a><span data-ttu-id="c3b17-103">Módulo 1.8.0 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c3b17-103">Azure Stack Module 1.8.0</span></span>

## <a name="requirements"></a><span data-ttu-id="c3b17-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="c3b17-104">Requirements:</span></span>

<span data-ttu-id="c3b17-105">A versão mínima suportada do Azure Stack é a 1910.</span><span class="sxs-lookup"><span data-stu-id="c3b17-105">Minimum supported Azure Stack version is 1910.</span></span>

<span data-ttu-id="c3b17-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="c3b17-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="c3b17-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="c3b17-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.8.0
```

## <a name="release-notes"></a><span data-ttu-id="c3b17-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="c3b17-108">Release Notes</span></span>

* <span data-ttu-id="c3b17-109">Suportado com a atualização 1910</span><span class="sxs-lookup"><span data-stu-id="c3b17-109">Supported with 1910 update</span></span>
* <span data-ttu-id="c3b17-110">As alterações incluem:</span><span class="sxs-lookup"><span data-stu-id="c3b17-110">Changes include:</span></span>

    - <span data-ttu-id="c3b17-111">**Novo módulo de administração do DRP**: o Deployment Resource Provider (DRP) permite implementações orquestradas de fornecedores de recursos para o Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="c3b17-111">**New DRP Admin module**: The Deployment Resource Provider (DRP) enables orchestrated deployments of resource providers to Azure Stack Hub.</span></span> <span data-ttu-id="c3b17-112">Estes comandos interagem com a camada do Azure Resource Manager para interagir com o DRP.</span><span class="sxs-lookup"><span data-stu-id="c3b17-112">These commands interact with the Azure Resource Manager layer to interact with DRP.</span></span>

    - <span data-ttu-id="c3b17-113">**BRP**:</span><span class="sxs-lookup"><span data-stu-id="c3b17-113">**BRP**:</span></span>
        - <span data-ttu-id="c3b17-114">suporte de restauro de uma função única para cópia de segurança da infraestrutura do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c3b17-114">Support single role restore for Azures stack infrastructure backup.</span></span>
        - <span data-ttu-id="c3b17-115">Adicione o parâmetro `RoleName` ao cmdlet R`estore-AzsBackup`.</span><span class="sxs-lookup"><span data-stu-id="c3b17-115">Add parameter `RoleName` to cmdlet R`estore-AzsBackup`.</span></span>

    - <span data-ttu-id="c3b17-116">**FRP**: alterações interruptivas para os recursos **Drive** e **Volume** com a versão de API de 01-05-2019.</span><span class="sxs-lookup"><span data-stu-id="c3b17-116">**FRP**: Breaking changes for **Drive** and **Volume** resources with API version 2019-05-01.</span></span> <span data-ttu-id="c3b17-117">As funcionalidades são suportadas pelo Azure Stack Hub 1910 e posterior:</span><span class="sxs-lookup"><span data-stu-id="c3b17-117">The features are supported by Azure Stack Hub 1910 and later:</span></span>
        - <span data-ttu-id="c3b17-118">Os valores dos IDs `Name`, `HealthStatus` e `OperationalStatus` foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c3b17-118">The value of ID, `Name`, `HealthStatus`, and `OperationalStatus` have been changed.</span></span>
        - <span data-ttu-id="c3b17-119">São suportadas as novas propriedades `FirmwareVersion`, `IsIndicationEnabled`, `Manufacturer` e `StoragePool` para os recursos **Drive**.</span><span class="sxs-lookup"><span data-stu-id="c3b17-119">Supported new properties `FirmwareVersion`, `IsIndicationEnabled`, `Manufacturer`, and `StoragePool` for **Drive** resources.</span></span>
        - <span data-ttu-id="c3b17-120">As propriedades `CanPool` e `CannotPoolReason` dos recursos **Drive** foram preteridas. Em alternativa, utilize `OperationalStatus`.</span><span class="sxs-lookup"><span data-stu-id="c3b17-120">The properties `CanPool` and `CannotPoolReason` of **Drive** resources have been deprecated; use `OperationalStatus` instead.</span></span>
