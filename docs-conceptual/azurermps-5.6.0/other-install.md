---
title: "Outros modos de instalação do Azure PowerShell | Microsoft Docs"
description: "Como instalar o Azure PowerShell através do pacote MSI ou do Instalador de Plataforma Web."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 8a88cce312b4cca002c342c04e1f97b966ae3d2f
ms.sourcegitcommit: 20af779cd523c758d40e23d60eb989a4ef982d5c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/15/2018
---
# <a name="other-installation-methods"></a>Outros métodos de instalação

O Azure PowerShell tem múltiplos métodos de instalação. A utilização do PowerShellGet com a Galeria do PowerShell é o método preferencial. O Azure PowerShell pode ser instalado no Windows através do Instalador de Plataforma Web (WebPI) ou do ficheiro MSI disponível a partir do GitHub. O Azure PowerShell também pode ser instalado num contentor do Docker.

## <a name="install-on-windows-using-the-web-platform-installer"></a>Instalar no Windows através do Instalador de Plataforma Web

Instalar o Azure PowerShell mais recente a partir do WebPI é o mesmo que para versões anteriores.
Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.

> [!NOTE]
> Se tiver instalado anteriormente os módulos do Azure a partir da Galeria do PowerShell, o instalador irá removê-los automaticamente. Isto simplifica o seu ambiente ao assegurar que está instalada apenas uma versão do Azure PowerShell. No entanto, existem cenários onde poderá precisar de múltiplas versões instaladas ao mesmo tempo.
>
> Os módulos da Galeria do PowerShell instalam módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`. Em contrapartida, o instalador WebPI instalará os módulos do Azure em `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.
>
> Se ocorrer um erro durante a instalação, pode remover manualmente as pastas Azure* na pasta `$env:ProgramFiles\WindowsPowerShell\Modules` e tentar efetuar novamente a instalação.

Depois de concluída a instalação, a definição `$env:PSModulePath` deve incluir os diretórios que contêm os cmdlets do Azure PowerShell. Pode ser utilizado o comando seguinte para verificar se o Azure PowerShell está instalado corretamente.

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> Existe um problema conhecido que pode ocorrer ao instalar a partir do WebPI. Se o seu computador tiver de ser reiniciado devido a atualizações do sistema ou outras instalações, isto poderá provocar a falha das atualizações em `$env:PSModulePath` para incluir o caminho onde o Azure PowerShell está instalado.

Ao tentar carregar ou executar os cmdlets após a instalação, pode receber a seguinte mensagem de erro:

```
PS C:\> Login-AzureRmAccount
Login-AzureRmAccount : The term 'Login-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Login-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Login-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

Este erro pode ser corrigido ao reiniciar o computador ou ao importar o módulo através do caminho totalmente qualificado. Por exemplo:

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-on-windows-using-the-msi-package"></a>Instalar no Windows através do Pacote MSI

O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://aka.ms/azps-release). Se tiver versões anteriores dos módulos do Azure instaladas, o instalador remove-as automaticamente. O pacote MSI instala os módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`, mas não cria pastas específicas da versão.

## <a name="install-in-a-docker-container"></a>Instalar num contentor do Docker

Mantemos uma imagem do Docker pré-configurada com o Azure PowerShell.

Execute o contentor com `docker run`.

```powershell
docker run azuresdk/azure-powershell
```

Além disso, mantemos um subconjunto de cmdlets como contentor do PowerShell Core.

Para Mac/Linux, utilize a imagem `latest`.

```bash
docker run azuresdk/azure-powershell-core:latest
```

Para Windows, utilize a imagem `nanoserver`.

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

O Azure PowerShell está instalado na imagem através do `Install-Module` da [Galeria do PowerShell](https://www.powershellgallery.com/).
