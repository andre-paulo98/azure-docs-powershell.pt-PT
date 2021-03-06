---
title: Instalar e configurar o Azure PowerShell | Microsoft Docs
description: Como instalar e configurar o Azure PowerShell para uma primeira utilização.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/27/2018
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 7c0ae849d276df103619bec3422cdc9b694d068f
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89238589"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a>Instalar o Azure PowerShell no Windows com o PowerShellGet

[!INCLUDE [migrate-to-az-banner](../../includes/migrate-to-az-banner.md)]

Este artigo explica os passos para instalar os módulos do Azure PowerShell para o PowerShell 5.x para Windows com o PowerShellGet. O PowerShellGet e a gestão do módulo constituem a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).

O modelo de implementação clássica do Azure não é suportado por esta versão do Azure PowerShell. Para obter suporte para implementações clássicas, siga as instruções indicadas em [Instalar o módulo de Gestão de Serviço do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).

> [!IMPORTANT]
> O módulo AzureRM não é suportado para macOS ou Linux. Para utilizar cmdlets do Azure PowerShell nestas plataformas, [Instale o módulo Az](/powershell/azure/install-az-ps).

## <a name="step-1-install-powershellget"></a>Passo 1: Instalar o PowerShellGet

A instalação de itens a partir da Galeria do PowerShell requer o módulo PowerShellGet. Certifique-se de que tem a versão adequada do PowerShellGet e outros requisitos de sistema. Execute o seguinte comando para ver se tem o PowerShellGet instalado no sistema.


```powershell-interactive
Get-InstalledModule -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

Deverá ver algo semelhante à saída seguinte:

```Output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

Precisa da versão 1.1.2.0 ou superior do PowerShellGet. Para atualizar o PowerShellGet, utilize o seguinte comando:

```powershell-interactive
Install-Module PowerShellGet -Force
```

Se não tiver o PowerShellGet instalado, veja a secção [Como obter o PowerShellGet](#how-to-get-powershellget) deste artigo.

> [!NOTE]
> A utilização do PowerShellGet requer uma Política de Execução que lhe permita executar scripts. Para obter mais informações sobre a Política de Execução do PowerShell, veja [About Execution Policies (Sobre as Políticas de Execução)](/powershell/module/microsoft.powershell.core/about/about_execution_policies).
>
> [!IMPORTANT]
> O módulo descrito neste documento, o AzureRM, utiliza o .NET Framework. Isto torna-o incompatível com o PowerShell 6.0, que utiliza o .NET Core. Se estiver a utilizar o PowerShell 6.0, siga as [instruções de instalação para macOS e Linux](/powershell/azure/install-az-ps).

## <a name="step-2-install-azure-powershell"></a>Passo 2: Instalar o Azure PowerShell

Instalar o Azure PowerShell a partir da Galeria do PowerShell requer privilégios elevados. Execute o seguinte comando a partir de uma sessão do PowerShell elevada:

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

Por predefinição, a galeria do PowerShell não está configurada como um repositório Fidedigno para PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

Responder "Sim" ou "Sim a Todos" para continuar com a instalação.

> [!NOTE]
> Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.

O módulo de AzureRM é um módulo de rollup para os cmdlets do Azure Resource Manager. Quando instala o módulo AzureRM, qualquer outro módulo do Azure PowerShell que não tenha sido anteriormente instalado será transferido a partir da Galeria do PowerShell.

Se tiver uma versão anterior do Azure PowerShell instalado poderá receber um erro. Para resolver este problema, veja a secção [Updating to a new version of Azure PowerShell](#update-azps)(Atualizar para uma versão nova do Azure PowerShell) deste artigo.

## <a name="step-3-load-the-azurerm-module"></a>Passo 3: Carregar o módulo de AzureRM

Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell. Deve fazê-lo numa sessão normal (não avaliada) do PowerShell. Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:

```powershell-interactive
Import-Module -Name AzureRM
```

## <a name="next-steps"></a>Passos Seguintes

Para mais informações sobre como utilizar o Azure PowerShell, consulte os artigos seguintes:

* [Introdução ao Azure PowerShell](get-started-azureps.md)

## <a name="reporting-issues-and-feedback"></a>Comunicar problemas e comentários

Se encontrar quaisquer erros com a ferramenta, comunique o assunto na secção [Problemas](https://github.com/Azure/azure-powershell/issues) do nosso repositório do GitHub. Para enviar comentários a partir da linha de comandos, experimente o cmdlet `Send-Feedback`.

## <a name="frequently-asked-questions"></a>Perguntas mais frequentes

### <a name="how-to-get-powershellget"></a>Como obter o PowerShellGet

|Versão do SO|Instruções de instalação|
|---|---|
|Tenho o Windows 10 ou o Windows Server 2016|Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO|
|Quero atualizar para o PowerShell 5|[Instalar a versão mais recente do WMF](https://www.microsoft.com/download/details.aspx?id=54616)|
|Estou a executar uma versão do Windows com o PowerShell 3 ou o PowerShell 4|[Obter os módulos PackageManagement](https://go.microsoft.com/fwlink/?LinkID=746217)|

### <a name="div-idhelpmechoosechecking-the-version-of-azure-powershell"></a><div id="helpmechoose"/>A verificar a versão do Azure PowerShell

Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell. Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-InstalledModule AzureRM` a partir da linha de comandos.

```powershell-interactive
Get-InstalledModule AzureRM -AllVersions | Select-Object -Property Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a>Suporte para os métodos de implementação clássicos

Se tiver implementações que utilizam o modelo de implementação clássico, pode instalar a versão de Gestão de Serviço do Azure PowerShell. Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps). Os módulos Azure e AzureRM partilham dependências comuns. Se utilizar os módulos do Azure e do AzureRM, deve instalar a mesma versão de cada pacote.

### <a name="div-idupdate-azpsupdating-to-a-new-version-of-azure-powershell"></a><div id="update-azps"/>A atualizar para uma nova versão do Azure PowerShell

Se tiver uma versão anterior do Azure PowerShell instalada, que inclui o módulo de Gestão de Serviço, poderá receber o erro seguinte:

```Output
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

Como a mensagem de erro indica, tem de utilizar o parâmetro -AllowClobber para instalar o módulo. Utilize o seguinte comando:

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

Para mais informações, veja o tópico de ajuda para [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).

### <a name="installing-module-versions-side-by-side"></a>Instalar as versões do módulo lado a lado

O método de instalação do PowerShellGet é o único método que suporta a instalação de várias versões. Por exemplo, poderá ter scripts escritos utilizando uma versão anterior do Azure PowerShell Azure que não têm o tempo ou recursos atualizados. Os comandos seguintes ilustram como instalar várias versões do Azure PowerShell:

```powershell-interactive
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

Apenas uma versão do módulo pode ser carregada numa sessão do PowerShell. Tem de abrir uma nova janela do PowerShell e utilizar `Import-Module` para importar uma versão específica dos cmdlets do AzureRM:

```powershell-interactive
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

> [!NOTE]
> A versão 2.1.0 e a versão 1.2.6 são as primeiras versões do módulo concebidas para serem instaladas e utilizadas lado a lado. Ao carregar uma versão anterior do Azure PowerShell, as versões incompatíveis do módulo **AzureRM.Profile** são carregadas. Isto dá origem a que os cmdlets solicitem que inicie sessão sempre executar um cmdlet.

### <a name="other-installation-methods"></a>Outros métodos de instalação

Para obter informações sobre a instalação com o Instalador de Plataforma Web ou o Pacote MSI, veja [Outros métodos de instalação](other-install.md)
