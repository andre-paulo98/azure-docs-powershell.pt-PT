---
title: Executar o Azure PowerShell num contentor do Docker
description: Como executar o Azure PowerShell num contentor do Docker.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 27ac176d8bd0b142b7740b2ba6793edb500a8af3
ms.sourcegitcommit: 7df99dc139e93a8a4e6d5b1a27968857588d75dd
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/16/2018
ms.locfileid: "40106556"
---
# <a name="run-azure-powershell-in-a-docker-container"></a>Executar o Azure PowerShell num contentor do Docker

Para facilitar a execução do Azure PowerShell em ambientes portáteis, a Microsoft publica imagens do Docker com o Azure PowerShell pré-instalado. Estas imagens oferecem um convidado do Linux que executa o PowerShell Core ou um convidado do Windows com o PowerShell Core ou PowerShell 5.

| Ambiente | Imagem do Docker |
|-------------|--------------|
| PowerShell no Windows | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| PowerShell Core no Windows | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| PowerShell Core no Linux | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

Para executar qualquer um destes contentores, utilize `docker run -it $ImageName` para obter um terminal interativo. Por exemplo, para executar o PowerShell Core no contentor do Linux, utilize:

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Para executar um contentor do Windows no Docker, o SO anfitrião tem de ser o Windows e o Docker tem de estar definido para executar contentores do Windows. Para saber mais sobre como alternar entre os ambientes Windows e Linux no Docker, veja a documentação do Docker [Alternar entre os contentores do Windows e do Linux](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).

## <a name="use-a-powershell-core-container"></a>Utilizar um contentor do PowerShell Core

Os contentores do PowerShell Core são fornecidos com o PowerShell Core v6 e o módulo `AzureRM.NetCore` pré-instalado. Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a>Utilizar o contentor do Windows com o PowerShell

O contentor do Windows tem o módulo `AzureRM` pré-instalado. Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
