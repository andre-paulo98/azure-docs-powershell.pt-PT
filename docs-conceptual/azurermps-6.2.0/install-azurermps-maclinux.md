---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323174"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Instalar o Azure PowerShell no macOS ou Linux

Em plataformas não Windows, é possível executar o Azure PowerShell por cima do PowerShell Core v6. Em vez do Azure PowerShell padrão baseado no .NET Framework para Windows, este produto foi concebido para o .NET Core e pode ser executado em qualquer plataforma que suporte o .Net Core runtime.

> [!NOTE]
> Atualmente, tanto o PowerShell Core v6 como o Azure PowerShell para .NET Core ainda se encontram em fase beta.
> O suporte para estes produtos é limitado. Se se deparar com problemas ou detetar erros, registe um problema no GitHub.
>
> * [Problemas do PowerShell Core v6](https://github.com/PowerShell/PowerShell/issues)
> * [Problemas do Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a>Instalar o PowerShell Core v6

A instalação do PowerShell Core v6 no Linux ou macOS varia consoante a distribuição do Linux e a versão do SO.
Pode encontrar instruções detalhadas nos seguintes artigos:

- [Instalar o PowerShell Core no macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [Instalar o PowerShell Core no Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Instalar o Azure PowerShell para o .NET Core

O PowerShell Core v6 é fornecido com o módulo PowerShellGet já instalado. o que facilita a instalação de qualquer módulo que seja publicado na Galeria do PowerShell. Para instalar o Azure PowerShell, abra uma nova sessão do PowerShell e execute o seguinte comando:

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a>Carregar o módulo AzureRM.Netcore

Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell. Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

Quando a importação terminar, pode testar o módulo que acabou de instalar ao tentar iniciar sessão no Azure através do seguinte comando:

```powershell
Connect-AzureRmAccount
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
