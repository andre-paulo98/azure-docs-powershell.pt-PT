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
ms.openlocfilehash: af0343e5ad92fa7f2b5c10e3e67cb7e10feb81c6
ms.sourcegitcommit: 0fdccb57a356b6e7c35a77b1f76e01fb96ef582b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/17/2019
ms.locfileid: "65855793"
---
# <a name="azure-stack-module-172"></a><span data-ttu-id="75ac7-103">Módulo 1.7.2 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="75ac7-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="75ac7-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="75ac7-104">Requirements:</span></span>

<span data-ttu-id="75ac7-105">A versão mínima suportada do Azure Stack é a 1904.</span><span class="sxs-lookup"><span data-stu-id="75ac7-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="75ac7-106">Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span><span class="sxs-lookup"><span data-stu-id="75ac7-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install-powershell-for-azure-stack"></a><span data-ttu-id="75ac7-107">Instalar o PowerShell para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="75ac7-107">Install PowerShell for Azure Stack</span></span>

<span data-ttu-id="75ac7-108">A instalação tem três passos:</span><span class="sxs-lookup"><span data-stu-id="75ac7-108">Installation has three steps:</span></span>

1. <span data-ttu-id="75ac7-109">Instalar o PowerShell para o Azure Stack com base na versão do Azure Stack que utiliza</span><span class="sxs-lookup"><span data-stu-id="75ac7-109">Install Azure Stack PowerShell depending on your version of Azure Stack</span></span>
2. <span data-ttu-id="75ac7-110">Ativar funcionalidades de armazenamento adicionais</span><span class="sxs-lookup"><span data-stu-id="75ac7-110">Enable additional storage features</span></span>
3. <span data-ttu-id="75ac7-111">Confirmar a instalação do PowerShell</span><span class="sxs-lookup"><span data-stu-id="75ac7-111">Confirm the installation of PowerShell</span></span>

### <a name="install-azure-stack-powershell"></a><span data-ttu-id="75ac7-112">Instalar o PowerShell para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="75ac7-112">Install Azure Stack PowerShell</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install the AzureRM.BootStrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRM.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Get-AzureRmProfile -Update
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

### <a name="enable-additional-storage-features"></a><span data-ttu-id="75ac7-113">Ativar funcionalidades de armazenamento adicionais</span><span class="sxs-lookup"><span data-stu-id="75ac7-113">Enable additional storage features</span></span>

```
# Install the Azure.Storage module version 4.5.0
Install-Module -Name Azure.Storage -RequiredVersion 4.5.0 -Force -AllowClobber

# Install the AzureRm.Storage module version 5.0.4
Install-Module -Name AzureRM.Storage -RequiredVersion 5.0.4 -Force -AllowClobber

# Remove incompatible storage module installed by AzureRM.Storage
Uninstall-Module Azure.Storage -RequiredVersion 4.6.1 -Force

# Load the modules explicitly specifying the versions
Import-Module -Name Azure.Storage -RequiredVersion 4.5.0
Import-Module -Name AzureRM.Storage -RequiredVersion 5.0.4
```

## <a name="release-notes"></a><span data-ttu-id="75ac7-114">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="75ac7-114">Release Notes</span></span>

* <span data-ttu-id="75ac7-115">Suportado com a atualização 1904</span><span class="sxs-lookup"><span data-stu-id="75ac7-115">Supported with 1904 update</span></span>
* <span data-ttu-id="75ac7-116">Esta é uma versão com uma alteração interruptiva.</span><span class="sxs-lookup"><span data-stu-id="75ac7-116">This a breaking change release.</span></span> <span data-ttu-id="75ac7-117">Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170></span><span class="sxs-lookup"><span data-stu-id="75ac7-117">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="75ac7-118">Alteração interruptiva do Módulo Azs.Backup.Admin \*: Alterações de segurança ao modo de encriptação baseada em certificados.</span><span class="sxs-lookup"><span data-stu-id="75ac7-118">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="75ac7-119">O suporte de chaves simétricas foi preterido.</span><span class="sxs-lookup"><span data-stu-id="75ac7-119">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="75ac7-120">Módulo Azs.Fabric.Admin       \* Preterição           \* Get-AzsInfrastructureVolume foi preterido. Fornecemos o novo cmdlet Get-AzsVolume           \* Get-AzsStorageSystem foi preterido. Fornecemos o novo cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool foi preterido. O objeto StorageSubSystem tem a propriedade de capacidade</span><span class="sxs-lookup"><span data-stu-id="75ac7-120">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="75ac7-121">Módulo Azs.Compute.Admin           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Chamar ConvertTo-PlatformImageObject apenas no caminho de sucesso           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Chamar ConvertTo-VmExtensionObject apenas no caminho de sucesso</span><span class="sxs-lookup"><span data-stu-id="75ac7-121">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="75ac7-122">Módulo Azs.Storage.Admin           \* Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma".</span><span class="sxs-lookup"><span data-stu-id="75ac7-122">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
