---
title: Instalar o Azure PowerShell no Windows com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c287afa2fb34938cac7304028071afd7deedb263
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243791"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a>Instalar o Azure PowerShell no Windows com o PowerShellGet

[!INCLUDE [migrate-to-az-banner](../../includes/migrate-to-az-banner.md)]

Este artigo explica os passos para instalar os módulos do Azure PowerShell para o PowerShell 5.x para Windows com o PowerShellGet. O PowerShellGet e a gestão do módulo constituem a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).

O modelo de implementação clássica do Azure não é suportado por esta versão do Azure PowerShell. Para obter suporte para implementações clássicas, siga as instruções indicadas em [Instalar o módulo de Gestão de Serviço do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).

> [!IMPORTANT]
> O módulo AzureRM não é suportado para macOS ou Linux. Para utilizar cmdlets do Azure PowerShell nestas plataformas, [Instale o módulo Az](/powershell/azure/install-az-ps).

## <a name="requirements"></a>Requisitos

Para instalar o Azure PowerShell, precisa do PowerShellGet versão 1.1.2.0 ou superior. Para verificar se está disponível no seu sistema, execute o comando:

```powershell-interactive
Get-InstalledModule -Name PowerShellGet -AllVersions | Select-Object -Property Name,Version,Path
```

Deverá ver algo semelhante à saída seguinte:

```output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

Se precisa de atualizar a sua instalação do PowerShellGet, execute o seguinte comando:

```powershell-interactive
Install-Module PowerShellGet -Force
```

Se não tem o PowerShellGet instalado, siga as instruções na tabela abaixo do seu sistema.

|Cenário|Instruções de instalação|
|---|---|
|Windows 10<br/>Windows Server 2016|Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO|
|Atualizar para o PowerShell 5| <ol><li>[Instalar a versão mais recente do WMF](https://www.microsoft.com/download/details.aspx?id=54616)</li><li>Execute o seguinte comando:<br/>```Install-Module PowerShellGet -Force```</li></ol>|
|Windows com PowerShell 3 ou PowerShell 4|<ol><il>[Obter os módulos PackageManagement](https://go.microsoft.com/fwlink/?LinkID=746217)</il><li>Execute o seguinte comando:<br/>```Install-Module PowerShellGet -Force```</li></ol>|

> [!NOTE]
> A utilização do PowerShellGet requer uma Política de Execução que lhe permita executar scripts. Para obter mais informações sobre a Política de Execução do PowerShell, veja [About Execution Policies (Sobre as Políticas de Execução)](/powershell/module/microsoft.powershell.core/about/about_execution_policies).
>
> [!IMPORTANT]
> O módulo descrito neste documento, o AzureRM, utiliza o .NET Framework. Isto torna-o incompatível com o PowerShell 6.0, que utiliza o .NET Core. Se estiver a utilizar o PowerShell 6.0, siga as [instruções de instalação para macOS e Linux](/powershell/azure/install-az-ps).

## <a name="install-the-azure-powershell-module"></a>Instalar o módulo do Azure PowerShell

Precisa de privilégios elevados para instalar módulos da Galeria do PowerShell. Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada:

```powershell-interactive
Install-Module -Name AzureRM
```

> [!NOTE]
> Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responda `Yes` ou `Yes to All` para continuar com a instalação.

O módulo `AzureRM` é um módulo de rollup para os cmdlets do Azure PowerShell. A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.

## <a name="sign-in"></a>Iniciar sessão

Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).
Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="update-the-azure-powershell-module"></a>Atualizar o módulo do Azure PowerShell

Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module). Este comando __não__ desinstala as versões anteriores.

```powershell-interactive
Update-Module -Name AzureRM
```

Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).

## <a name="use-multiple-versions-of-azure-powershell"></a>Utilizar várias versões do Azure PowerShell

Pode instalar várias versões do Azure PowerShell. Poderá precisar de mais de uma versão se trabalhar com recursos do Azure Stack no local, executar uma versão mais antiga do Windows que não pode atualizar para o PowerShell 5.0 ou utilizar o modelo de implementação clássica do Azure. Para instalar uma versão anterior, apresente o argumento `-RequiredVersion` ao instalar.

```powershell-interactive
# Install version 2.3.0 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

Ao carregar o módulo do Azure PowerShell, a versão mais recente é carregada por predefinição. Para carregar uma versão diferente, apresente o argumento `-RequiredVersion`.

```powershell-interactive
# Load version 2.3.0 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

## <a name="provide-feedback"></a>Enviar comentários

Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).
Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).

## <a name="next-steps"></a>Passos Seguintes

Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.
