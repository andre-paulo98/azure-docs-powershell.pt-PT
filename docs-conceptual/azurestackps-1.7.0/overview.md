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
ms.openlocfilehash: af34497f243ce8f4f718e88312f6ad54eb6ad848
ms.sourcegitcommit: 993db64e68b222acbcfdeef2e81eb3316b160858
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/14/2019
ms.locfileid: "56240536"
---
# <a name="azure-stack-module-170"></a>Módulo 1.7.0 do Azure Stack

## <a name="requirements"></a>Requisitos:
A versão mínima suportada do Azure Stack é a 1901.

Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.7.0

## <a name="install"></a>Instalar
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.0
```
## <a name="release-notes"></a>Notas de Versão
* Suportado com a atualização 1901
* Esta é uma versão com uma alteração interruptiva. Para obter detalhes sobre as alterações interruptivas, veja https://aka.ms/azspshmigration170
* Alteração interruptiva do Módulo Azs.Backup.Admin *: Alterações de segurança ao modo de encriptação baseada em certificados. O suporte de chaves simétricas foi preterido.
* Módulo Azs.Fabric.Admin       * Preterição           * Get-AzsInfrastructureVolume foi preterido. Fornecemos o novo cmdlet Get-AzsVolume           * Get-AzsStorageSystem foi preterido. Fornecemos o novo cmdlet Get-AzsStorageSubSystem           * Get-AzsStoragePool foi preterido. O objeto StorageSubSystem tem a propriedade de capacidade
* Módulo Azs.Compute.Admin           * BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Chamar ConvertTo-PlatformImageObject apenas no caminho de sucesso           * BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Chamar ConvertTo-VmExtensionObject apenas no caminho de sucesso
* Módulo Azs.Storage.Admin           * Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma".

