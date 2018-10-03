---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/24/2018
ms.openlocfilehash: 05e86d96b345455f3d3bb3fe6dedf933fff6187c
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179246"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Instalar o Azure PowerShell no macOS ou Linux

É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows. Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core. Para trabalhar com estas plataformas, está disponível uma versão standard de .NET do Azure PowerShell.

> [!NOTE]
> Atualmente, tanto o PowerShell Core v6, como o Azure PowerShell para .NET Standard, ainda se encontram em fase beta.
> O suporte para estes produtos é limitado. Se se deparar com problemas ou detetar erros, registe um problema no GitHub.
>
> * [Problemas do PowerShell Core v6](https://github.com/PowerShell/PowerShell/issues)
> * [Problemas do Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>Instalar o PowerShell Core

As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.
Pode encontrar instruções detalhadas nos seguintes artigos:

* [Instalar o PowerShell Core no macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Instalar o PowerShell Core no Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a>Instalar o Azure PowerShell para .NET Standard

> [!IMPORTANT]
> O módulo `AzureRM`, descrito noutros artigos, não funciona com o PowerShell Core.
> Tem de instalar o módulo `Az` para obter a funcionalidade do Azure PowerShell no Powershell Core.

O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado. Inicie o PowerShell com o comando:

```bash
pwsh
```

Para instalar o Azure PowerShell, execute o seguinte comando:

```powershell
Install-Module Az
```

> [!NOTE]
> Se se deparar com um erro de permissões quando tentar instalar o módulo, poderá ter de executar o PowerShell no modo de superutilizador para o instalar.
>
> ```bash
> sudo pwsh
> ```

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responda `Yes` ou `Yes to All` para continuar com a instalação.

## <a name="enable-aliases"></a>Permitir aliases

Para compatibilidade com o módulo `AzureRM` já existente, o módulo `Az` novo tem a capacidade de criar aliases de retrocompatibilidade para os cmdlets `AzureRM`. Antes de utilizar o módulo pela primeira vez, configure esses aliases com o comando seguinte:

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

Isto configura os aliases para o utilizador atual apenas. Veja a ajuda do cmdlet para obter outros valores que podem ser fornecidos a `-Scope`, para configurar os aliases.

> [!NOTE]
> Se se deparar com um erro sobre a localização de um caminho, confirme que o mesmo existe no seu sistema local. No âmbito `CurrentUser`, este erro pode ser resolvido mediante a execução do seguinte comando em `bash`:
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a>Iniciar sessão

Para começar a utilizar o Azure PowerShell, precisa de carregar `Az` para a sua sessão do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure. __Não__ precisa de privilégios elevados para importar um módulo.

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. A importação automática do módulo `Az` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).
No macOS e no Linux, deve trabalhar com o seu perfil através da variável de ambiente `$Profile`. Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="next-steps"></a>Passos Seguintes

Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).
