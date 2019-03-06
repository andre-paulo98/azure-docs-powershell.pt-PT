---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 269119333b2197a15ed7bb50e3e5d90588456174
ms.sourcegitcommit: 5630030c5cfa9828c3c024b69de59248263ef17f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/26/2019
ms.locfileid: "56837576"
---
# <a name="install-the-azure-powershell-module"></a>Instalar o módulo do Azure PowerShell

Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet. Estas instruções funcionam nas plataformas Windows, macOS e Linux. Não existem outros métodos de instalação suportados atualmente para o módulo do Az.

## <a name="requirements"></a>Requisitos

O Azure PowerShell funciona com o PowerShell 5.1 ou superior no Windows, ou com o PowerShell 6 em qualquer plataforma.
Para consultar a sua versão do PowerShell, execute o comando:

```powershell-interactive
$PSVersionTable.PSVersion
```

Se tiver uma versão desatualizada ou precisar de instalar o PowerShell, veja [Instalar várias versões do PowerShell](/powershell/scripting/setup/installing-powershell). As informações sobre a instalação da sua plataforma estão associadas a essa página.

Se estiver a utilizar o PowerShell 5 no Windows, também precisa de ter o .NET Framework 4.7.2 instalado. Para obter instruções sobre como atualizar ou instalar uma nova versão do .NET Framework, veja o [Guia de instalação do .NET Framework](/dotnet/framework/install).

## <a name="install-the-azure-powershell-module"></a>Instalar o módulo do Azure PowerShell

> [!IMPORTANT]
>
> Pode ter ambos os módulos, AzureRM e Az, instalados em simultâneo. Se tiver ambos os módulos instalados, __não ative os aliases__.
> A ativação dos aliases irá causar conflitos entre os cmdlets do AzureRM e os aliases de comandos do Az, o que pode dar origem a um comportamento inesperado.
> Recomenda-se que desinstale o AzureRM antes de instalar o módulo do Az. Pode sempre desinstalar o AzureRM ou ativar os aliases em qualquer altura. Para obter mais informações sobre os aliases de comandos do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).
> Para obter instruções de desinstalação, veja [Desinstalar o módulo do AzureRM](uninstall-az-ps.md#uninstall-the-azurerm-module). 

Para instalar módulo num âmbito global, precisa de privilégios elevados para instalar módulos da Galeria do PowerShell. Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada ("Executar como Administrador" no Windows, ou com privilégios de superutilizador no macOS ou Linux):

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

Se não tiver acesso a privilégios de administrador, pode instalar para o utilizador atual, ao adicionar o argumento `-Scope`.

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responda `Yes` ou `Yes to All` para continuar com a instalação.

O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell. A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.

## <a name="sign-in"></a>Iniciar sessão

Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`. Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="update-the-azure-powershell-module"></a>Atualizar o módulo do Azure PowerShell

Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module). Este comando __não__ desinstala versões mais antigas.

```powershell-interactive
Update-Module -Name Az
```

Para obter mais informações sobre como remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).

## <a name="use-multiple-versions-of-azure-powershell"></a>Utilizar várias versões do Azure PowerShell

Pode instalar mais de uma versão do Azure PowerShell. Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).

Pode instalar ou carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion`:

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.

## <a name="provide-feedback"></a>Enviar comentários

Se encontrar um erro no Azure Powershell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).
Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).

## <a name="next-steps"></a>Passos Seguintes

Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).
Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).
