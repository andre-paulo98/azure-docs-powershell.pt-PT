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
ms.openlocfilehash: 6568dc4e6c51e8f250aad2c4dd765c065fe6a8bf
ms.sourcegitcommit: ae4540a90508db73335a54408dfd6cdf3712a1e9
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/18/2019
ms.locfileid: "58808065"
---
# <a name="azure-stack-module-171"></a><span data-ttu-id="d92b1-103">Módulo 1.7.1 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d92b1-103">Azure Stack Module 1.7.1</span></span>

## <a name="requirements"></a><span data-ttu-id="d92b1-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="d92b1-104">Requirements:</span></span>

<span data-ttu-id="d92b1-105">A versão mínima suportada do Azure Stack é a 1901.</span><span class="sxs-lookup"><span data-stu-id="d92b1-105">Minimum supported Azure Stack version is 1901.</span></span>

<span data-ttu-id="d92b1-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="d92b1-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="d92b1-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="d92b1-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.1
```

## <a name="release-notes"></a><span data-ttu-id="d92b1-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="d92b1-108">Release Notes</span></span>

* <span data-ttu-id="d92b1-109">Suportado com a atualização 1901</span><span class="sxs-lookup"><span data-stu-id="d92b1-109">Supported with 1901 update</span></span>
* <span data-ttu-id="d92b1-110">Esta é uma versão com uma alteração interruptiva.</span><span class="sxs-lookup"><span data-stu-id="d92b1-110">This a breaking change release.</span></span> <span data-ttu-id="d92b1-111">Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170></span><span class="sxs-lookup"><span data-stu-id="d92b1-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="d92b1-112">Alteração interruptiva do Módulo Azs.Backup.Admin \*: Alterações de segurança ao modo de encriptação baseada em certificados.</span><span class="sxs-lookup"><span data-stu-id="d92b1-112">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="d92b1-113">O suporte de chaves simétricas foi preterido.</span><span class="sxs-lookup"><span data-stu-id="d92b1-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="d92b1-114">Módulo Azs.Fabric.Admin       \* Preterição           \* Get-AzsInfrastructureVolume foi preterido. Fornecemos o novo cmdlet Get-AzsVolume           \* Get-AzsStorageSystem foi preterido. Fornecemos o novo cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool foi preterido. O objeto StorageSubSystem tem a propriedade de capacidade</span><span class="sxs-lookup"><span data-stu-id="d92b1-114">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="d92b1-115">Módulo Azs.Compute.Admin           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Chamar ConvertTo-PlatformImageObject apenas no caminho de sucesso           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Chamar ConvertTo-VmExtensionObject apenas no caminho de sucesso</span><span class="sxs-lookup"><span data-stu-id="d92b1-115">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="d92b1-116">Módulo Azs.Storage.Admin           \* Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma".</span><span class="sxs-lookup"><span data-stu-id="d92b1-116">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
