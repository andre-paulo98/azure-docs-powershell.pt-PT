---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: d99265c7f156622d876d700106e2b06dd729e8b8
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365753"
---
# <a name="install-the-azure-powershell-module"></a>Instalar o módulo do Azure PowerShell

Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet. Estas instruções funcionam nas plataformas Windows, macOS e Linux. Não existem outros métodos de instalação suportados atualmente para o módulo do Az.

## <a name="requirements"></a>Requisitos

O Azure PowerShell funciona com o PowerShell 5.1 ou superior no Windows, ou com o PowerShell Core 6.x e posterior em todas as plataformas. Se não tiver a certeza se tem o PowerShell, ou está no macOS ou Linux, [instale a versão mais recente do PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).

Para consultar a sua versão do PowerShell, execute o comando:

```powershell-interactive
$PSVersionTable.PSVersion
```

Para executar o Azure PowerShell no PowerShell 5.1 no Windows:

1. Atualize para o [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) se for necessário. Se estiver no Windows 10, já tem o PowerShell 5.1 instalado.
2. Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).

Não existem requisitos adicionais para o Azure PowerShell quando utilizar o PowerShell Core.

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

Devido à forma como o módulo do Az é empacotado, o comando [Update-Module](/powershell/module/powershellget/update-module) não atualizará a sua instalação corretamente. O AZ é tecnicamente um meta-módulo que abrange todos os submódulos que contêm cmdlets para interagir com os serviços do Azure. Isso significa que para atualizar o módulo do Azure PowerShell, terá de o __reinstalar__, em vez de apenas o __atualizar__. Isto é feito como a instalação, mas poderá ter de adicionar o argumento `-Force`:

```powershell
Install-Module -Name Az -AllowClobber -Force
```

Embora os módulos instalados possam ser substituídos, poderá ainda ter versões antigas no seu sistema.
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
