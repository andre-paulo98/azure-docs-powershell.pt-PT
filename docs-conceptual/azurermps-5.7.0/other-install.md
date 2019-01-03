---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell sem o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 30f7a01b941bb2861b1652fa30ea002d40c80a80
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594578"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a>Instalar o Azure PowerShell no Windows com o MSI ou o Instalador de Plataforma Web

Este artigo explica como instalar o Azure PowerShell no Windows com um pacote MSI ou o Instalador de Plataforma Web (WebPI).  
Utilize estes métodos de instalação apenas se forem necessários para o seu sistema. A forma recomendada para instalar o Azure PowerShell no Windows é com o PowerShellGet. Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

## <a name="install-or-update-on-windows-using-the-msi-package"></a>Instalar ou atualizar no Windows com o Pacote MSI

O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018). Se tiver instalado as versões anteriores dos módulos do Azure como um MSI, o instalador remove-as automaticamente. O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`. Ambos os módulos `AzureRM` e `Azure` são instalados.

> [!NOTE]
> Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.

Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).
Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>Instalar ou atualizar no Windows com o Instalador de Plataforma Web

Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação. Se tiver versões anteriores dos módulos do Azure instaladas a partir de um MSI ou com o WebPI, o instalador remove-as automaticamente. Os módulos são instalados no `${env:ProgramFiles}\WindowsPowerShell\Modules`. Os módulos `AzureRM` e `Azure` estão instalados.

> [!NOTE]
> Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.

Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).
Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).