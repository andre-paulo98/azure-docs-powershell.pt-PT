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
# <a name="azure-stack-module-172"></a>Módulo 1.7.2 do Azure Stack

## <a name="requirements"></a>Requisitos:

A versão mínima suportada do Azure Stack é a 1904.

Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)

## <a name="install"></a>Instalar

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a>Notas de Versão

* Suportado com a atualização 1904
* Esta é uma versão com uma alteração interruptiva. Para obter detalhes sobre as alterações interruptivas, veja <https://aka.ms/azspshmigration170>
* Alteração interruptiva: Alterações de segurança ao modo de encriptação baseada em certificados. O suporte de chaves simétricas foi preterido.
* Para obter detalhes sobre as alterações interruptivas, veja https://aka.ms/azspshmigration170
* Módulo Azs.Storage.Admin 
* Correção de erro - A nova Quota de Armazenamento utiliza a predefinição se não for fornecida nenhuma.
