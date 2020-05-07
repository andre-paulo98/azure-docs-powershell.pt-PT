---
title: Instalar e configurar o módulo Gestão do Serviço do Azure PowerShell | Microsoft Docs
description: Como instalar e configurar o Azure PowerShell para uma primeira utilização.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/06/2017
ms.openlocfilehash: a4911e72f687c07b31805c07fd23263a6b7f33b4
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "75718802"
---
# <a name="installing-the-azure-powershell-service-management-module"></a>Instalar o módulo Gestão do Serviço do Azure PowerShell

Instalar o Azure PowerShell a partir da [Galeria do PowerShell](https://www.powershellgallery.com/) é o método de instalação preferencial.

## <a name="step-1-install-powershellget"></a>Passo 1: Instalar o PowerShellGet

A instalação de itens a partir da Galeria do PowerShell requer o módulo PowerShellGet. Certifique-se de que tem a versão adequada do PowerShellGet e outros requisitos de sistema. Execute o seguinte comando para ver se tem o PowerShellGet instalado no sistema.

```powershell
Get-InstalledModule PowerShellGet -AllVersions | Select-Object Name,Version,Path
```

Deverá ver algo semelhante ao resultado seguinte:

```output
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

Se não tiver o PowerShellGet instalado, veja [Como obter o PowerShellGet](#how-to-get-powershellget).

## <a name="step-2-install-azure-powershell"></a>Passo 2: Instalar o Azure PowerShell

Execute o comando seguinte a partir da consola do Windows PowerShell em execução como Administrador:

```powershell
Install-Module Azure
```

O módulo Azure é um módulo de rollup para os cmdlets do Azure Resource Manager. Quando instala o módulo AzureRM, qualquer outro módulo do Azure que não tenha sido anteriormente instalado será transferido e instalado a partir da Galeria do PowerShell.

O módulo Gestão do Serviço do Azure partilha dependências com os módulos Azure PowerShell Resource Manager. Se tiver instalado os módulos Azure PowerShell Resource Manager, terá de adicionar o parâmetro `-AllowClobber` ao comando de instalação. Isto permite a atualização das dependências partilhadas. Sem este parâmetro, a instalação do módulo falha.

```powershell
Install-Module Azure -AllowClobber
```

Depois de instalar este módulo, pode importá-lo ao executar o seguinte comando:

```powershell
Import-Module Azure
```

## <a name="to-use-the-cmdlets"></a>Para utilizar os cmdlets

Para começar a trabalhar com os cmdlets da Gestão do Serviço do Azure, primeiro inicie sessão na sua conta do Azure. Para iniciar sessão na sua conta, execute o seguinte comando:

```powershell
Add-AzureAccount
```

Depois de iniciar sessão no Azure, o Azure PowerShell cria um contexto para a sessão fornecida. Esse contexto contém o ambiente, a conta, o inquilino e a subscrição do Azure PowerShell que serão utilizados para todos os cmdlets nessa sessão. Pode agora utilizar os módulos abaixo.

## <a name="azure-service-management-cmdlets"></a>Cmdlets da Gestão do Serviço do Azure

Os módulos do Azure PowerShell são atualizados com frequência. Se reparar que a ajuda do cmdlet online inclui cmdlets ou parâmetros que não estão no módulo, transfira e instale a versão mais recente do módulo. Para localizar a versão do seu módulo, escreva: `(Get-InstalledModule Azure).Version`.

Para obter scripts de exemplo que podem ajudá-lo a automatizar algumas das tarefas comuns no Azure, veja o [Centro de Scripts do Windows Azure](http://www.windowsazure.com/documentation/scripts/).

Para obter informações gerais sobre a instalação, formação, utilização e personalização do Windows PowerShell, veja [Scripting com o Windows PowerShell](https://go.microsoft.com/fwlink/p/?linkid=320210).

### <a name="how-to-get-powershellget"></a>Como obter o PowerShellGet

|Versão do SO|Instruções de instalação|
|---|---|
|Tenho o Windows 10 ou o Windows Server 2016|Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO|
|Quero atualizar para o PowerShell 5|[Instalar a versão mais recente do WMF](https://www.microsoft.com/download/details.aspx?id=54616)|
|Estou a executar uma versão do Windows com o PowerShell 3 ou o PowerShell 4|[Obter os módulos PackageManagement](https://go.microsoft.com/fwlink/?LinkID=746217)|

<div id="helpmechoose"/>

### <a name="checking-the-version-of-azure-powershell"></a>A verificar a versão do Azure PowerShell

Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell. Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-InstalledModule Azure` a partir da linha de comandos.

```powershell
Get-InstalledModule Azure -AllVersions | Select-Object Name,Version,Path
```
