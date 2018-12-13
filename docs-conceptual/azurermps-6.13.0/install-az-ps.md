---
title: Instalar o módulo "Az" do Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet no Windows, macOS e Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/26/2018
ms.openlocfilehash: 3d52b18750341f220dc8e10d6bf89796457c5a10
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217002"
---
# <a name="install-the-azure-powershell-az-module"></a>Instalar o módulo "Az" do Azure PowerShell

Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet. Estas instruções funcionam nas plataformas Windows, macOS e Linux. Para a versão de pré-visualização do Az, não são suportados outros métodos de instalação. 

## <a name="requirements"></a>Requisitos

O Azure PowerShell funciona com o PowerShell 5.x no Windows ou no PowerShell 6.x em qualquer plataforma. Para verificar a versão do PowerShell em execução na sua máquina, execute o seguinte comando:

```powershell-interactive
$PSVersionTable.PSVersion
```

Se tiver uma versão desatualizada ou precisar de instalar o PowerShell, veja [Instalar várias versões do PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6). As informações sobre a instalação da sua plataforma estão associadas a essa página.

## <a name="install-the-azure-powershell-module"></a>Instalar o módulo do Azure PowerShell

> [!IMPORTANT]
>
> Pode ter ambos os módulos `AzureRM` e `Az` instalados em simultâneo. Se tiver ambos os módulos instalados, __não ative os aliases__.
> Ativar os aliases causa conflitos entre os cmdlets `AzureRM` e os aliases de comando `Az`, o que pode causar comportamentos inesperados.
> É recomendado que antes de instalar o módulo `Az`, desinstale `AzureRM`. Pode sempre desinstalar `AzureRM` ou ativar aliases a qualquer momento. Para instruções de desinstalação, veja [Desinstalar o módulo do Azure PowerShell (AzureRM)](uninstall-azurerm-ps.md). 

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

O módulo `Az` é um módulo de rollup para os cmdlets do Azure PowerShell. A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.

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

Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module). Este comando __não__ desinstala as versões anteriores.

```powershell-interactive
Update-Module -Name Az
```

Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).

## <a name="use-multiple-versions-of-azure-powershell"></a>Utilizar várias versões do Azure PowerShell

Pode instalar mais de uma versão do Azure PowerShell. Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).

Pode carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion` com `Install-Module` e `Import-Module`:

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

Se tiver mais do que uma versão do módulo instalada, a versão mais recente é carregada por predefinição.

## <a name="provide-feedback"></a>Enviar comentários

Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).
Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.profile/send-feedback).

## <a name="next-steps"></a>Passos Seguintes

Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.
