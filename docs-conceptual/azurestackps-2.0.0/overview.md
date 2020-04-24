---
title: Descrição Geral do Azure Stack Hub Admin PowerShell | Microsoft Docs
description: Descrição geral do Azure Stack Hub Admin PowerShell com instruções de instalação e configuração.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 04/16/2020
ms.openlocfilehash: fd1f2a3778e348ba41b46acb4bdce19e18a7f4ec
ms.sourcegitcommit: 4c61442a2df1cee633ce93cad9f6bc793803baa2
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/16/2020
ms.locfileid: "81524970"
---
# <a name="azure-stack-hub-module-200"></a>Azure Stack Hub, Módulo 2.0.0

## <a name="requirements"></a>Requisitos:

A versão mínima suportada do Azure Stack Hub é a 2002.

Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)

## <a name="install"></a>Instalar

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Az.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue

Install-Module -Name Az.BootStrapper -Force -AllowPrerelease

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 2.0.0-preview -AllowPrerelease
```


## <a name="release-notes"></a>Notas de Versão

* Suportado com a atualização 2002.  

  O Azure Stack Hub 2.0.0 é uma alteração interruptiva. O módulo utiliza o módulo Az em vez do módulo AzureRM. Pode encontrar um guia de migração e uma lista de alterações interruptivas em [Migrar do AzureRM para o Azure PowerShell Az no Azure Stack Hub](https://aka.ms/AA7qsji).
