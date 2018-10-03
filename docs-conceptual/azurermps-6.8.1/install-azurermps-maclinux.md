---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: f014d62e898da195a38052db6b7e37a2cd96dfdd
ms.sourcegitcommit: 3a02e0c85c83de873981dd392500bc82c1cf9286
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/24/2018
ms.locfileid: "46560121"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Instalar o Azure PowerShell no macOS ou Linux

É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows. Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core. Para trabalhar com estas plataformas, está disponível uma versão standard de .NET do Azure PowerShell.

> [!NOTE]
> Atualmente, tanto o PowerShell Core v6 como o Azure PowerShell para .NET Core ainda se encontram em fase beta.
> O suporte para estes produtos é limitado. Se se deparar com problemas ou detetar erros, registe um problema no GitHub.
>
> * [Problemas do PowerShell Core v6](https://github.com/PowerShell/PowerShell/issues)
> * [Problemas do Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>Instalar o PowerShell Core

As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.
Pode encontrar instruções detalhadas nos seguintes artigos:

* [Instalar o PowerShell Core no macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Instalar o PowerShell Core no Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Instalar o Azure PowerShell para o .NET Core

O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado. A instalação de módulos no PowerShell exige privilégios elevados, pelo que irá precisar de iniciar a sua sessão como um superutilizador:

```bash
sudo pwsh
```

Para instalar o Azure PowerShell, execute o seguinte comando:

```powershell
Install-Module Az
```

> [!IMPORTANT]
> O módulo `AzureRM` descrito noutros artigos não é criado para o .NET Core e não irá funcionar com o PowerShell Core. Os módulos `Az` contêm aliases de comandos para todos os cmdlets `AzureRM`, pelo que se aplica toda a documentação de `AzureRM`.

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responda `Yes` ou `Yes to All` para continuar com a instalação.

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
