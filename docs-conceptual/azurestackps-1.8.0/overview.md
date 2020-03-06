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
# <a name="azure-stack-module-180"></a>Módulo 1.8.0 do Azure Stack

## <a name="requirements"></a>Requisitos:

A versão mínima suportada do Azure Stack é a 1910.

Nota: Para versões anteriores do Azure Stack, veja [Instalar Powershell do Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)

## <a name="install"></a>Instalar

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.8.0
```

## <a name="release-notes"></a>Notas de Versão

* Suportado com a atualização 1910
* As alterações incluem:

    - **Novo módulo de administração do DRP**: o Deployment Resource Provider (DRP) permite implementações orquestradas de fornecedores de recursos para o Azure Stack Hub. Estes comandos interagem com a camada do Azure Resource Manager para interagir com o DRP.

    - **BRP**:
        - suporte de restauro de uma função única para cópia de segurança da infraestrutura do Azure Stack.
        - Adicione o parâmetro `RoleName` ao cmdlet R`estore-AzsBackup`.

    - **FRP**: alterações interruptivas para os recursos **Drive** e **Volume** com a versão de API de 01-05-2019. As funcionalidades são suportadas pelo Azure Stack Hub 1910 e posterior:
        - Os valores dos IDs `Name`, `HealthStatus` e `OperationalStatus` foram alterados.
        - São suportadas as novas propriedades `FirmwareVersion`, `IsIndicationEnabled`, `Manufacturer` e `StoragePool` para os recursos **Drive**.
        - As propriedades `CanPool` e `CannotPoolReason` dos recursos **Drive** foram preteridas. Em alternativa, utilize `OperationalStatus`.
