---
title: Instalar o Azure PowerShell com um MSI
description: Como instalar o Azure PowerShell sem o PowerShellGet utilizar um MSI
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 33d9214544ddb126b717685f9e7986bed926b149
ms.sourcegitcommit: 15f21c40dcb7610e2fbaaabf264ad925e4224500
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90928487"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a>Instalar o Azure PowerShell no Windows com o MSI

Este artigo explica como instalar o Azure PowerShell no Windows com um Instalador do MSI. O instalador MSI é fornecido para ambientes onde a Galeria do PowerShell pode ser bloqueada por uma firewall ou onde for necessário um instalador offline. A forma recomendada para instalar o Azure PowerShell é através do PowerShellGet. Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-az-ps.md).

## <a name="requirements"></a>Requisitos

O instalador MSI no Windows foi criado para instalar o Azure PowerShell apenas para o PowerShell 5.1. Para a instalação em plataformas que não sejam do Windows ou versões posteriores do PowerShell, utilize a opção [Instalar com o PowerShellGet](install-az-ps.md). Para consultar a sua versão do PowerShell, execute o comando:

```powershell-interactive
$PSVersionTable.PSVersion
```

Para utilizar o Azure PowerShell no PowerShell 5.1:

1. Atualize para o [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell) se for necessário. Se estiver no Windows 10, já tem o PowerShell 5.1 instalado.
2. Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).

## <a name="install-or-update-on-windows-using-the-msi-package"></a>Instalar ou atualizar no Windows com o Pacote MSI

O pacote MSI para o Azure PowerShell está disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest). Se tiver instalado versões anteriores do Azure PowerShell com o MSI, o instalador remove-as automaticamente. O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`.

Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzAccount
```

> [!NOTE]
> Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`. Devido à forma como o módulo está estruturado, esta operação pode demorar um minuto.

Terá de repetir este passo para cada nova sessão do PowerShell que iniciar. Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="provide-feedback"></a>Enviar comentários

Se encontrar um erro no Azure PowerShell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues). Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).

## <a name="next-steps"></a>Passos Seguintes

Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md). Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).
