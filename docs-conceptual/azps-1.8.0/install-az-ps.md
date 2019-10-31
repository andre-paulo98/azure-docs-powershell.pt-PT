---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/22/2019
ms.openlocfilehash: 7f22a420068db87fa2c3c007bd36f515384162fb
ms.sourcegitcommit: ad7677d703a8512d371d3123dc7e541156b95cb8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/23/2019
ms.locfileid: "72814379"
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

> [!WARNING]
> __Não__ pode ter os módulos AzureRM e Az instalados em simultâneo para o PowerShell 5.1 para Windows. Se precisar de manter o AzureRM disponível no sistema, instale o módulo do Az para o PowerShell Core 6.x ou posterior. Para tal, [instale o PowerShell Core 6.x ou posterior](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows) e, em seguida, siga estas instruções num terminal do PowerShell Core.

O método de instalação recomendado é instalar apenas para o utilizador ativo:

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

Se quiser instalar para todos os utilizadores num sistema, precisará de privilégios de administrador. Numa sessão do PowerShell elevada, execute como administrador ou com o comando `sudo` no macOS ou Linux:

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope AllUsers
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

## <a name="install-offline"></a>Instalar offline

Em alguns ambientes, não é possível ligar à Galeria do PowerShell. Nessas situações, ainda pode instalar offline através de um destes métodos:

* Transfira os módulos para outra localização e utilize-os como uma origem de instalação na sua rede. Isso pode ser um processo complicado, mas irá permitir que armazene em cache os módulos do PowerShell num único servidor ou que seja implementada a partilha de ficheiros através do PowerShellGet para quaisquer sistemas desligados. Saiba como configurar um repositório local e instalar em sistemas desligados com a opção [Trabalhar com repositórios do PowerShellGet locais](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).
* [Transferira o MSI do Azure PowerShell](install-az-ps-msi.md) para um computador ligado a uma rede e, em seguida, copie o instalador para os sistemas sem o acesso à Galeria do PowerShell. Tenha em mente que o instalador MSI funciona apenas para o PowerShell 5.1 no Windows.
* Guarde o módulo com [Guardar-Módulo](/powershell/module/PowershellGet/Save-Module) numa partilha de ficheiros ou guarde noutra fonte e faça a cópia manualmente para outros computadores:
  
  ```powershell-interactive
  Save-Module -Name Az -Path '\\someshare\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a>Resolução de problemas

Seguem-se alguns problemas comuns vistos durante a instalação do módulo do Azure PowerShell. Se detetar um problema não mencionado neste artigo, [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).

### <a name="proxy-blocks-connection"></a>O proxy bloqueia a ligação

Se ocorrerem erros de `Install-Module` que indiquem que a Galeria do PowerShell não está acessível, pode estar atrás de um proxy. Diferentes sistemas operativos têm requisitos diferentes para configurar um proxy ao nível do sistema, não abordados detalhadamente aqui. Contacte o administrador de sistema para obter as suas definições de proxy e saber como configurá-las para o seu SO.

O PowerShell não pode ser configurado para utilizar este proxy automaticamente. Com o PowerShell 5.1 e posterior, pode configurar o proxy a utilizar numa sessão do PowerShell com o seguinte comando:

```powershell
(New-Object System.Net.WebClient).Proxy.Credentials = `
  [System.Net.CredentialCache]::DefaultNetworkCredentials
```

Se as credenciais do seu sistema operativo estiverem configuradas corretamente, os pedidos do PowerShell serão encaminhados através do proxy.
Para manter esta definição entre sessões, adicione o comando a um [perfil do PowerShell](/powershell/module/microsoft.powershell.core/about/about_profiles).

Para instalar o pacote, o proxy tem de permitir ligações HTTPS no seguinte endereço:

* `https://www.powershellgallery.com`

## <a name="sign-in"></a>Iniciar sessão

Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> Se tiver desativado o carregamento automático do módulo, importe o módulo manualmente com `Import-Module Az`. Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="update-the-azure-powershell-module"></a>Atualizar o módulo do Azure PowerShell

Devido à forma como o módulo do Az é empacotado, o comando [Update-Module](/powershell/module/powershellget/update-module) não atualizará a sua instalação corretamente. Quando instala o módulo Az, este recolhe e instala todos os respetivos submódulos dependentes, os quais fornecem os cmdlets para cada serviço.
Isso significa que para atualizar o módulo do Azure PowerShell, terá de o __reinstalar__, em vez de apenas o __atualizar__. Isto é feito como a instalação, mas poderá ter de adicionar o argumento `-Force`:

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
