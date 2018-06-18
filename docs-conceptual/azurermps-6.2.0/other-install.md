---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell através do pacote MSI ou do Instalador de Plataforma Web.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323327"
---
# <a name="other-installation-methods"></a>Outros métodos de instalação

Este artigo explica como instalar o Azure PowerShell com um pacote MSI ou o Instalador de Plataforma Web (WebPI). Também pode executar o Azure PowerShell a partir de um contentor de Docker. Utilize estes métodos de instalação apenas se forem necessários para o seu sistema. A forma canónica de instalar o Azure PowerShell é através do PowerShellGet. Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).

Para instalar em ambientes Linux ou macOS, veja [Instalar o Azure PowerShell no macOS ou Linux](install-azurermps-maclinux.md).

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>Instalar ou atualizar no Windows com o Instalador de Plataforma Web

Instalar o Azure PowerShell mais recente a partir do WebPI é o mesmo que para versões anteriores.
Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.

> [!NOTE]
> Se tiver instalado anteriormente os módulos do Azure a partir da Galeria do PowerShell, o instalador irá removê-los automaticamente. Isto simplifica o seu ambiente ao assegurar que está instalada apenas uma versão do Azure PowerShell. No entanto, existem cenários onde poderá precisar de múltiplas versões instaladas ao mesmo tempo.
>
> Os módulos da Galeria do PowerShell instalam módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`. Em contrapartida, o instalador WebPI instalará os módulos do Azure em `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.
>
> Se ocorrer um erro durante a instalação, pode remover manualmente as pastas `Azure*` na pasta `$env:ProgramFiles\WindowsPowerShell\Modules` e tentar instalar novamente.

Depois de concluída a instalação, a definição `$env:PSModulePath` deve incluir os diretórios que contêm os cmdlets do Azure PowerShell. O comando que se segue pode ser utilizado para verificar se o Azure PowerShell está instalado corretamente:

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> Existe um problema conhecido que pode ocorrer ao instalar a partir do WebPI. Se o seu computador tiver de ser reiniciado devido a atualizações do sistema ou outras instalações, isto poderá provocar a falha das atualizações em `$env:PSModulePath` para incluir o caminho onde o Azure PowerShell está instalado.

Ao tentar carregar ou executar os cmdlets após a instalação, pode receber a seguinte mensagem de erro:

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

Este erro pode ser corrigido ao reiniciar o computador ou ao importar o módulo através do caminho totalmente qualificado.

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a>Instalar ou atualizar no Windows com o Pacote MSI

O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://aka.ms/azps-release). Se tiver versões anteriores dos módulos do Azure instaladas, o instalador remove-as automaticamente. O pacote MSI instala os módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`, mas não cria pastas específicas da versão.

## <a name="run-in-a-docker-container"></a>Executar num contentor do Docker

Mantemos um conjunto de imagens do Docker pré-configuradas com o Azure PowerShell. Existem dois tipos de contentor disponíveis: contentores com o PowerShell tradicional em execução no Windows e um contentor com o PowerShell Core em execução no Windows ou Linux.

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