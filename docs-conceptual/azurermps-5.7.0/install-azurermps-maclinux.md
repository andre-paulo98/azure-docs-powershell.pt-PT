---
title: Instalar e configurar o Azure PowerShell no macOS e Linux | Microsoft Docs
description: Como instalar e configurar o Azure PowerShell para uma primeira utilização no macOS e Linux.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/12/2018
ms.openlocfilehash: e68ef0ac6aebda9e5249c2f6882400ee3a4f2e02
ms.sourcegitcommit: 5f0013981fcea1d689649b9a2b2ffe84ae842e56
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/16/2018
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a>Instalar e configurar o Azure PowerShell no macOS e Linux

Agora, é possível instalar o PowerShell Core v6 e o Azure PowerShell em plataformas não Windows.
O processo de instalação do Azure PowerShell no macOS e Linux não difere muito do do Windows. No entanto, primeiro tem de instalar o PowerShell Core v6.

> [!NOTE]

> Atualmente, tanto o PowerShell Core v6 como o Azure PowerShell para .NET Core ainda se encontram em fase beta.
> O suporte para estes produtos é limitado. Se tiver problemas ou detetar erros, envie um relatório para Problemas no GitHub.
>
> * [Problemas do PowerShell Core v6](https://github.com/PowerShell/PowerShell/issues)
> * [Problemas do Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-core-v6"></a>Passo 1: Instalar o PowerShell Core v6

O processo de instalação do PowerShell Core v6 varia consoante o sistema operativo de destino.
Embora seja possível instalar o PowerShell Core v6 no Windows, este artigo incide sobre o macOS e Linux. Se quiser utilizar o Azure PowerShell no Windows, veja o artigo [instalar](./install-azurerm-ps.md) para o Windows.

A instalação do **PowerShell Core v6** no Linux ou macOS varia consoante a distribuição do Linux e a versão do SO.
Pode encontrar instruções detalhadas no seguinte artigo:

- [Instalar o PowerShell Core no macOS e no Linux](/powershell/scripting/setup/installing-powershell-core-on-macos-and-linux)

## <a name="step-2-install-azure-powershell-for-net-core"></a>Passo 2: Instalar o Azure PowerShell para .NET Core

O PowerShell Core v6 é fornecido com o módulo PowerShellGet já instalado. o que facilita a instalação de qualquer módulo que seja publicado na Galeria do PowerShell. Para instalar o Azure PowerShell, abra uma nova sessão do PowerShell e execute o seguinte comando:

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a>Passo 3: Carregar o módulo AzureRM.Netcore

Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell. Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

Quando a importação terminar, pode testar o módulo que acabou de instalar ao tentar iniciar sessão no Azure através do seguinte comando:

```powershell
Login-AzureRmAccount
```

O comando acima deve pedir-lhe para aceder a `https://aka.ms/devicelogin` e introduzir o código fornecido.

## <a name="available-cmdlets"></a>Cmdlets disponíveis

Os módulos do Azure PowerShell para .NET Standard ainda estão em desenvolvimento. Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos. As seguintes funções estão implementadas nos módulos AzureRM.Netcore:

* Gestão de contas
  - Inicie sessão com a conta Microsoft, a conta Organizacional ou o Principal de Serviço através do Microsoft Azure Active Directory
  - Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext
* Ambiente
  - Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar
  - Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)
* Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.
  - Máquina Virtual
  - Serviço de Aplicações (Sites)
  - SQL Database
  - Armazenamento
  - Rede

## <a name="next-steps"></a>Passos Seguintes

Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).
