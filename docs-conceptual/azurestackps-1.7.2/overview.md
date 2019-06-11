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
# <a name="azure-stack-module-172"></a>Módulo 1.7.2 do Azure Stack

## <a name="requirements"></a>Requisitos:

A versão mínima suportada do Azure Stack é a 1904.

Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)

## <a name="install-powershell-for-azure-stack"></a>Instalar o PowerShell para o Azure Stack

A instalação tem três passos:

1. Instalar o PowerShell para o Azure Stack com base na versão do Azure Stack que utiliza
2. Ativar funcionalidades de armazenamento adicionais
3. Confirmar a instalação do PowerShell

### <a name="install-azure-stack-powershell"></a>Instalar o PowerShell para o Azure Stack

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

### <a name="enable-additional-storage-features"></a>Ativar funcionalidades de armazenamento adicionais

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

## <a name="release-notes"></a>Notas de Versão

* Suportado com a atualização 1904
* Esta é uma versão com uma alteração interruptiva. Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170>
* Alteração interruptiva do Módulo Azs.Backup.Admin *: Alterações de segurança ao modo de encriptação baseada em certificados. O suporte de chaves simétricas foi preterido.
* Módulo Azs.Fabric.Admin       * Preterição           * Get-AzsInfrastructureVolume foi preterido. Fornecemos o novo cmdlet Get-AzsVolume           * Get-AzsStorageSystem foi preterido. Fornecemos o novo cmdlet Get-AzsStorageSubSystem           * Get-AzsStoragePool foi preterido. O objeto StorageSubSystem tem a propriedade de capacidade
* Módulo Azs.Compute.Admin           * BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Chamar ConvertTo-PlatformImageObject apenas no caminho de sucesso           * BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Chamar ConvertTo-VmExtensionObject apenas no caminho de sucesso
* Módulo Azs.Storage.Admin           * Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma".
