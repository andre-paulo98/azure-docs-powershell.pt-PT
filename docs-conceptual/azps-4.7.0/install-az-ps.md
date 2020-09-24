---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/14/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: a263f1d363b3d1a1cce433a6112c55afe65262a4
ms.sourcegitcommit: 15f21c40dcb7610e2fbaaabf264ad925e4224500
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90928447"
---
# <a name="install-azure-powershell"></a>Instalar o Azure PowerShell

Este artigo explica como instalar os módulos do Azure PowerShell com o [PowerShellGet](/powershell/scripting/gallery/installing-psget). Estas instruções funcionam nas plataformas Windows, macOS e Linux.

O Azure PowerShell também está disponível no [Azure Cloud Shell](/azure/cloud-shell/overview) e está agora pré-instalado nas [imagens do Docker](azureps-in-docker.md).

## <a name="requirements"></a>Requisitos

> [!NOTE]
> A versão recomendada do PowerShell para utilização com o Azure PowerShell em todas as plataformas é o PowerShell 7.x e posteriores.

O Azure PowerShell funciona com o PowerShell 6.2.4 e posteriores em todas as plataformas. Também é suportado com o PowerShell 5.1 no Windows. Instale a [versão mais recente do PowerShell](/powershell/scripting/install/installing-powershell) disponível para o seu sistema operativo. O Azure PowerShell não tem requisitos adicionais quando é executado no PowerShell 6.2.4 e posteriores.

Para consultar a sua versão do PowerShell, execute o comando:

```azurepowershell-interactive
$PSVersionTable.PSVersion
```

Para utilizar o Azure PowerShell no PowerShell 5.1 no Windows:

1. Atualize para o [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell).
   Se utilizar o Windows 10, versão 1607 ou superior, já tem o PowerShell 5.1 instalado.
2. Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).
3. Verifique se tem a versão mais recente do PowerShellGet. Execute `Install-Module -Name PowerShellGet -Force`.

## <a name="install-the-azure-powershell-module"></a>Instalar o módulo do Azure PowerShell

> [!WARNING]
> Não suportamos os módulos do AzureRM e do Az instalados em simultâneo para o PowerShell 5.1 para Windows. Se precisar de manter o AzureRM disponível no sistema, instale o módulo do Az para o PowerShell 6.2.4 ou posterior.

A utilização dos cmdlets do PowerShellGet é o método de instalação preferido. Instale o módulo do Az apenas no utilizador atual. Este é o âmbito de instalação recomendado. Este método funciona da mesma forma nas plataformas Windows, macOS e Linux. Execute o seguinte comando a partir de uma sessão do PowerShell:

```powershell-interactive
if ($PSVersionTable.PSEdition -eq 'Desktop' -and (Get-Module -Name AzureRM -ListAvailable)) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Scope CurrentUser
}
```

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the `Set-PSRepository` cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responda `Yes` ou `Yes to All` para continuar com a instalação.

A instalação do módulo para todos os utilizadores num sistema requer privilégios elevados. Inicie a sessão do PowerShell com a opção **Executar como administrador** no Windows ou utilize o comando `sudo` no macOS ou Linux:

```powershell-interactive
if ($PSVersionTable.PSEdition -eq 'Desktop' -and (Get-Module -Name AzureRM -ListAvailable)) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Scope AllUsers
}
```

O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell. A instalação do mesmo transfere todos os módulos do Az do PowerShell em disponibilidade geral e disponibiliza os respetivos cmdlets para utilização.

## <a name="install-offline"></a>Instalar offline

Em alguns ambientes, não é possível ligar à Galeria do PowerShell. Nessas situações, ainda pode instalar offline através de um destes métodos:

* Transfira os módulos para outra localização na sua rede e utilize-os como uma origem de instalação.
  Este método permite-lhe colocar em cache os módulos do PowerShell num único servidor ou que seja implementada a partilha de ficheiros através do PowerShellGet para quaisquer sistemas desligados. Saiba como configurar um repositório local e instalar em sistemas desligados com a opção [Trabalhar com repositórios do PowerShellGet locais](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).
* [Transferira o MSI do Azure PowerShell](install-az-ps-msi.md) para um computador ligado a uma rede e, em seguida, copie o instalador para os sistemas sem o acesso à Galeria do PowerShell. Tenha em mente que o instalador MSI funciona apenas para o PowerShell 5.1 no Windows.
* Guarde o módulo com [Guardar-Módulo](/powershell/module/PowershellGet/Save-Module) numa partilha de ficheiros ou guarde noutra fonte e faça a cópia manualmente para outros computadores:

  ```powershell-interactive
  Save-Module -Name Az -Path '\\server\share\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a>Resolução de problemas

Seguem-se alguns problemas comuns vistos durante a instalação do módulo do Azure PowerShell. Se detetar um problema não mencionado neste artigo, [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).

### <a name="proxy-blocks-connection"></a>O proxy bloqueia a ligação

Se ocorrerem erros de `Install-Module` que indiquem que a Galeria do PowerShell não está acessível, pode estar atrás de um proxy. Diferentes sistemas operativos e ambientes de rede têm requisitos diferentes para configurar um proxy ao nível do sistema. Contacte o administrador de sistema para obter as suas definições de proxy e saber como configurá-las para o seu ambiente.

O PowerShell não pode ser configurado para utilizar este proxy automaticamente. Com o PowerShell 5.1 e posterior, pode configurar a sessão do PowerShell para utilizar um proxy com o seguinte comando:

```powershell
$webClient = New-Object System.Net.WebClient
$webClient.Proxy.Credentials = [System.Net.CredentialCache]::DefaultNetworkCredentials
```

Se as credenciais do seu sistema operativo estiverem configuradas corretamente, esta configuração encaminha os pedidos do PowerShell através do proxy. Para manter esta definição entre sessões, adicione os comandos ao seu [perfil do PowerShell](/powershell/module/microsoft.powershell.core/about/about_profiles).

Para instalar o pacote, o proxy tem de permitir ligações HTTPS no seguinte endereço:

* `https://www.powershellgallery.com`

## <a name="sign-in"></a>Iniciar sessão

Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
> Se tiver desativado o carregamento automático do módulo, importe o módulo manualmente com `Import-Module -Name Az`.
> Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. Para saber como manter o início de sessão do Azure entre sessões do PowerShell, veja [Manter as credenciais do utilizador entre sessões do PowerShell](context-persistence.md).

## <a name="update-the-azure-powershell-module"></a>Atualizar o módulo do Azure PowerShell

Para atualizar qualquer módulo do PowerShell, deve utilizar o mesmo método utilizado para instalar o módulo. Por exemplo, se utilizou originalmente `Install-Module`, deve utilizar [Update-Module](/powershell/module/powershellget/update-module) para obter a versão mais recente. Se utilizou originalmente o pacote MSI, deve transferir e instalar o novo pacote MSI.

Os cmdlets do PowerShellGet não conseguem atualizar os módulos instalados a partir de um pacote MSI. Os pacotes MSI não atualizam os módulos instalados com o PowerShellGet. Se tiver problemas ao utilizar o PowershellGet, deve **reinstalá-lo**, em vez de **o atualizar**. A reinstalação é feita como a instalação, mas terá ter de adicionar o parâmetro `-Force`:

```powershell
if ($PSVersionTable.PSEdition -eq 'Desktop' -and (Get-Module -Name AzureRM -ListAvailable)) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Force
}
```

Ao contrário das instalações baseadas em MSI, instalar ou atualizar com o PowerShellGet não remove as versões mais antigas que possam existir no seu sistema. Para remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md). Para obter mais informações sobre instalações baseadas em MSI, veja [Instalar o Azure PowerShell com um MSI](install-az-ps-msi.md).

## <a name="use-multiple-versions-of-azure-powershell"></a>Utilizar várias versões do Azure PowerShell

Pode instalar mais de uma versão do Azure PowerShell. Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | Select-Object -Property Name, Version
```

Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).

Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.

Pode instalar ou carregar uma versão específica do módulo `Az` com o parâmetro `-RequiredVersion`:

```powershell-interactive
# Install Az version 3.6.1
Install-Module -Name Az -RequiredVersion 3.6.1
# Load Az version 3.6.1
Import-Module -Name Az -RequiredVersion 3.6.1
```

## <a name="use-multiple-repositories-with-powershellget"></a>Utilizar vários repositórios no PowerShellGet

O parâmetro **Repository** é necessário se tiver repositórios adicionais ao PowerShellGet no seu sistema e o módulo do Az se encontrar em mais de um desses repositórios.

```powershell-interactive
if ($PSVersionTable.PSEdition -eq 'Desktop' -and (Get-Module -Name AzureRM -ListAvailable)) {
    Write-Warning -Message 'Az module not installed. Having both the AzureRM and Az modules installed at the same time is not supported.'
} else {
    Install-Module -Name Az -Repository PSGallery -AllowClobber -Force
}
```

## <a name="provide-feedback"></a>Enviar comentários

Se encontrar um erro no Azure PowerShell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues). Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).

## <a name="next-steps"></a>Passos Seguintes

Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md). Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).
