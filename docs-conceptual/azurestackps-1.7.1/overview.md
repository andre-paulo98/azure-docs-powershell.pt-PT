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
ms.sourcegitcommit: d3069aba7d1ac248aff755e4b21533af1f73251d
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2019
ms.locfileid: "58808065"
---
# <a name="azure-stack-module-171"></a>Módulo 1.7.1 do Azure Stack

## <a name="requirements"></a>Requisitos:

A versão mínima suportada do Azure Stack é a 1901.

Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)

## <a name="install"></a>Instalar

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.1
```

## <a name="release-notes"></a>Notas de Versão

* Suportado com a atualização 1901
* Esta é uma versão com uma alteração interruptiva. Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170>
* Alteração interruptiva do Módulo Azs.Backup.Admin *: Alterações de segurança ao modo de encriptação baseada em certificados. O suporte de chaves simétricas foi preterido.
* Módulo Azs.Fabric.Admin       * Preterição           * Get-AzsInfrastructureVolume foi preterido. Fornecemos o novo cmdlet Get-AzsVolume           * Get-AzsStorageSystem foi preterido. Fornecemos o novo cmdlet Get-AzsStorageSubSystem           * Get-AzsStoragePool foi preterido. O objeto StorageSubSystem tem a propriedade de capacidade
* Módulo Azs.Compute.Admin           * BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Chamar ConvertTo-PlatformImageObject apenas no caminho de sucesso           * BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Chamar ConvertTo-VmExtensionObject apenas no caminho de sucesso
* Módulo Azs.Storage.Admin           * Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma".
