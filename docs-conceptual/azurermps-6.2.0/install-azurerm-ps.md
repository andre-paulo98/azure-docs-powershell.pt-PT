---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323106"
---
# <a name="install-azure-powershell-with-powershellget"></a>Instalar o Azure PowerShell com o PowerShellGet

Este artigo explica os passos para instalar os módulos do Azure PowerShell num ambiente do Windows com o PowerShellGet.  Esta é a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).

Se quiser utilizar o Azure PowerShell no macOS ou Linux, veja o seguinte artigo: [Instalar e configurar o Azure PowerShell no macOS e Linux](install-azurermps-maclinux.md).

## <a name="system-requirements"></a>Requisitos de sistema

A versão 6.1.0 do Azure PowerShell exige a versão 5.0 (ou superior) do PowerShell. Para obter informações sobre a atualização para o PowerShell 5.0, veja [Atualizar o Windows PowerShell existente](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).

O PowerShellGet está automaticamente incluído no PowerShell 5.0.

## <a name="install-or-update-the-azure-powershell-module"></a>Instalar ou atualizar o módulo Azure PowerShell

Instalar o Azure PowerShell a partir da Galeria do PowerShell requer privilégios elevados. Execute o seguinte comando a partir de uma sessão do PowerShell elevada:

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> Este comando irá atualizar qualquer instalação existente do Azure PowerShell no seu sistema. Se precisar de ter mais do que uma versão instalada, veja a resposta das FAQ a [Posso instalar várias versões do Azure PowerShell?](#multiple-versions)

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responder "Sim" ou "Sim a Todos" para continuar com a instalação.

> [!NOTE]
> Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.

O módulo de AzureRM é um módulo de rollup para os cmdlets do Azure Resource Manager. Quando instala o módulo AzureRM, qualquer outro módulo do Azure PowerShell que não tenha sido instalado anteriormente é transferido a partir da Galeria do PowerShell.

## <a name="load-the-azure-powershell-module"></a>Carregar o módulo Azure PowerShell

Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell. Deve fazê-lo numa sessão normal (não avaliada) do PowerShell. Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a>Comunicar problemas e comentários

Se detetar erros na ferramenta, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues). Para enviar comentários a partir da linha de comandos, experimente o cmdlet `Send-Feedback`.

## <a name="next-steps"></a>Passos Seguintes

Para mais informações sobre como utilizar o Azure PowerShell, consulte os artigos seguintes:

* [Introdução ao Azure PowerShell](get-started-azureps.md)

## <a name="frequently-asked-questions"></a>Perguntas mais frequentes

### <a id="helpmechoose"></a>Como posso verificar a versão do Azure PowerShell?

Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell. Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-Module AzureRM` a partir da linha de comandos.

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a>Posso utilizar o Azure PowerShell para implementações clássicas do Azure?

Se tiver implementações que utilizam o modelo de implementação clássico, pode instalar a versão de Gestão de Serviço do Azure PowerShell. Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps). Os módulos Azure e AzureRM partilham dependências comuns. Se utilizar os módulos do Azure e do AzureRM, deve instalar a mesma versão de cada pacote.

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><a name="multiple-versions"/>Posso instalar várias versões do Azure PowerShell?

O PowerShellGet é o único método de instalação que suporta várias versões. Para instalar várias versões, pode adicionar o parâmetro `-RequiredVersion` ao cmdlet `Install-Module`. Por exemplo, para instalar as versões 6.1.0 e 1.2.9:

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

Apenas uma versão do módulo pode ser carregada numa sessão do PowerShell. Tem de abrir uma nova janela do PowerShell e utilizar `Import-Module` para importar uma versão específica do módulo Azure PowerShell.

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> A versão 2.1.0 e a versão 1.2.6 são as primeiras versões do módulo concebidas para serem instaladas e utilizadas lado a lado. Ao carregar uma versão anterior do Azure PowerShell, as versões incompatíveis do módulo **AzureRM.Profile** são carregadas. Isto resulta nos cmdlets solicitando que inicie sessão sempre executar um cmdlet.
