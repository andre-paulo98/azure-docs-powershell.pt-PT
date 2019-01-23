---
title: Descrição Geral do módulo Azure Stack Admin do PowerShell | Microsoft Docs
description: Descrição geral do módulo Azure Stack Admin com instruções para instalação e configuração.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: b0e85bec82b9b7c876b2bbf337b603c8d68cf6a3
ms.sourcegitcommit: 4e1174236796e7da929ff276addb32e42c18b707
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/12/2019
ms.locfileid: "54240140"
---
# <a name="azure-stack-module-160"></a>Módulo 1.6.0 do Azure Stack

## <a name="requirements"></a>Requisitos:
A versão mínima suportada do Azure Stack é a 1811.

Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.6.0

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

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.6.0
```

## <a name="release-notes"></a>Notas de Versão
* Suportado com a atualização 1811
* Módulo Azs.Compute.Admin
    * Foi corrigido o prefixo Azs em falta para New-DataDiskObject e foi adicionado o alias com aviso de preterição futura.
* Módulo Azs.Update.Admin
    * Foi adicionado um aviso para recomendar a execução de Test-AzureStack antes de Install-AzsUpdate
* Azs.Fabric.Admin
    * Novo cmdlet (as funcionalidades são suportadas pelo Azure Stack 1811+)
        * Get-AzsDrive
        * Get-AzsVolume
        * Get-AzsStorageSubSystem
    * Preterição
        * Get-AzsInfrastructureVolume passa a ser um alias de cmdlet Get-AzsVolume
* Azs.InfrastructureInsights.Admin
    *  Foi adicionado um novo cmdlet Repair-AzsAlert
* Azs.Storage.Admin
    * Correção de um erro em que os valores de quota predefinidos não estão a ser utilizados
* Módulo Azs.Subscriptions.Admin
    * Foi corrigido o prefixo Azs em falta para New-AddonPlanDefinitionObject e foi adicionado o alias com aviso de preterição futura.
