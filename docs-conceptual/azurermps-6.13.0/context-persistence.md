---
title: Manter credenciais do utilizador nas sessões do PowerShell
description: Saiba como reutilizar as credenciais do Azure e outras informações entre várias sessões do PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: edae36941312471df52946cdd752a3c1eca643ad
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243349"
---
# <a name="persist-user-credentials-across-powershell-sessions"></a>Manter credenciais do utilizador nas sessões do PowerShell

[!INCLUDE [migrate-to-az-banner](../../includes/migrate-to-az-banner.md)]

O Azure PowerShell oferece uma funcionalidade chamada **Gravação Automática de Contexto do Azure**, que lhe oferece as seguintes funcionalidades:

- Retenção de informações de início de sessão para serem reutilizadas em novas sessões do PowerShell.
- Utilização mais fácil de tarefas em segundo plano para executar os cmdlets de execução longa.
- Alternar entre contas, subscrições e ambientes sem um início de sessão separado.
- Execução de tarefas com credenciais e subscrições diferentes, em simultâneo, a partir da mesma sessão do PowerShell.

## <a name="azure-contexts-defined"></a>Contextos do Azure definidos

Um *contexto do Azure* é um conjunto de informações que define o destino dos cmdlets do Azure PowerShell. O contexto é composto por cinco partes:

- Uma *Conta* - o Nome de Utilizador ou Principal de serviço utilizado para autenticar as comunicações com o Azure
- Uma *Subscrição* - a subscrição do Azure com os Recursos que estão a ser alterados.
- Um *Inquilino* - o inquilino do Azure Active Directory que contém a sua subscrição. Os inquilinos são mais importantes para a autenticação do Principal de Serviço.
- Um *Ambiente* - a cloud de destino específica do Azure, normalmente, a Cloud global do Azure.
  No entanto, a definição do ambiente permite-lhe visar também uma cloud Nacional, do Government e no local (Azure Stack).
- *Credenciais* - as informações utilizadas pelo Azure para verificar a sua identidade e confirmar a sua autorização para aceder a recursos no Azure

Em versões anteriores, um Contexto do Azure tinha de ser criado sempre que abria uma nova sessão do PowerShell. A partir do Azure PowerShell v4.4.0, os contextos do Azure podem ser guardados automaticamente sempre que abrir uma nova sessão do PowerShell.

## <a name="automatically-save-the-context-for-the-next-sign-in"></a>Guardar automaticamente o contexto para o próximo início de sessão

Nas versões 6.3.0 e posteriores, o Azure PowerShell mantém as informações de contexto automaticamente entre sessões. Para definir o PowerShell para que esqueça o contexto e as credenciais, utilize `Disable-AzureRmContextAutoSave`. Terá de iniciar sessão no Azure sempre que abrir uma sessão do PowerShell.

Para permitir que o Azure PowerShell se lembre do contexto depois de fechar a sessão do PowerShell, utilize `Enable-AzureRmContextAutosave`. As informações de contexto e as credenciais são guardadas automaticamente numa pasta oculta especial no seu diretório de utilizador (`%AppData%\Roaming\Windows Azure PowerShell`).
Cada nova sessão do PowerShell visa o contexto utilizado na sua última sessão.

Os cmdlets que lhe permitem gerir contextos do Azure também permitem o controlo detalhado. Se pretender que as alterações sejam aplicadas apenas à sessão atual do PowerShell (âmbito `Process`) ou a cada sessão do PowerShell (âmbito `CurrentUser`). Estas opções são abordadas detalhadamente em [Utilizar Âmbitos de Contexto](#using-context-scopes).

## <a name="running-azure-powershell-cmdlets-as-background-jobs"></a>Executar os cmdlets do Azure PowerShell como tarefas em segundo plano

A funcionalidade **Gravação Automática de Contexto do Azure** permite-lhe também partilhar o contexto com tarefas do PowerShell em segundo plano. O PowerShell permite-lhe iniciar e monitorizar tarefas de execução longa como tarefas em segundo plano, sem ter de aguardar a conclusão das tarefas. Pode partilhar as credenciais com tarefas em segundo plano de duas formas diferentes:

- Passar o contexto como um argumento

  A maioria dos cmdlets do AzureRM permitem-lhe passar o contexto como um parâmetro para o cmdlet. Pode passar um contexto para uma tarefa em segundo plano, conforme mostrado no exemplo seguinte:

  ```powershell-interactive
  PS C:\> $job = Start-Job { param ($ctx) New-AzureRmVm -AzureRmContext $ctx [... Additional parameters ...]} -ArgumentList (Get-AzureRmContext)
  ```

- Utilizar o contexto predefinido com a Gravação Automática ativada

  Se tiver ativado a **Gravação Automática de Contexto**, as tarefas em segundo plano utilizam automaticamente o contexto predefinido guardado.

  ```powershell-interactive
  PS C:\> $job = Start-Job { New-AzureRmVm [... Additional parameters ...]}
  ```

Quando precisar de saber o resultado da tarefa em segundo plano, utilize `Get-Job` para verificar o estado da tarefa e `Wait-Job` para aguardar a conclusão da tarefa. Utilize `Receive-Job` para capturar ou apresentar o resultado da tarefa em segundo plano. Para obter mais informações, veja [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).

## <a name="creating-selecting-renaming-and-removing-contexts"></a>Criar, selecionar, mudar o nome e remover contextos

Para criar um contexto, tem de ter sessão iniciada no Azure. O cmdlet `Connect-AzureRmAccount` (ou o respetivo alias, `Login-AzureRmAccount`) define o contexto predefinido utilizado por cmdlets do Azure PowerShell e permite-lhe aceder a quaisquer inquilinos ou subscrições permitidos pelas suas credenciais.

Para adicionar um novo contexto após o início de sessão, utilize `Set-AzureRmContext` (ou o respetivo alias, `Select-AzureRmSubscription`).

```azurepowershell-interactive
PS C:\> Set-AzureRMContext -Subscription "Contoso Subscription 1" -Name "Contoso1"
```

O exemplo anterior adiciona um novo contexto que visa “Contoso Subscription 1”, com as suas credenciais atuais. O novo contexto tem o nome “Contoso1”. Se não indicar um nome para o contexto, é utilizado um nome predefinido, com o ID da conta e o ID da subscrição.

Para mudar o nome de um contexto existente, utilize o cmdlet `Rename-AzureRmContext`. Por exemplo:

```azurepowershell-interactive
PS C:\> Rename-AzureRmContext '[user1@contoso.org; 123456-7890-1234-564321]` 'Contoso2'
```

Este exemplo muda o nome do contexto com o nome automático `[user1@contoso.org; 123456-7890-1234-564321]` para o nome simples “Contoso2”. Os cmdlets que gerem contextos também utilizam a conclusão de tabulação, permitindo-lhe selecionar rapidamente o contexto.

Por último, para remover um contexto, utilize o cmdlet `Remove-AzureRmContext`.  Por exemplo:

```azurepowershell-interactive
PS C:\> Remove-AzureRmContext Contoso2
```

Esquece o contexto ao qual foi dado o nome “Contoso2”. Pode recriar este contexto com `Set-AzureRmContext`

## <a name="removing-credentials"></a>Remover credenciais

Pode remover todas as credenciais e os contextos associados de um utilizador ou principal de serviço, com `Disconnect-AzureRmAccount` (também conhecido como `Logout-AzureRmAccount`). Quando executado sem parâmetros, o cmdlet `Disconnect-AzureRmAccount` remove todas as credenciais e os contextos associados ao Utilizador ou Principal de Serviço no contexto atual. Pode passar um Nome de Utilizador, Nome do Principal de Serviço ou contexto para visar um determinado principal.

```azurepowershell-interactive
Disconnect-AzureRmAccount user1@contoso.org
```

## <a name="using-context-scopes"></a>Utilizar âmbitos de contexto

Ocasionalmente, poderá querer selecionar, alterar ou remover um contexto de uma sessão do PowerShell sem afetar outras sessões. Para alterar o comportamento predefinido de cmdlets de contexto, utilize o parâmetro `Scope`. O âmbito `Process` substitui o comportamento predefinido, fazendo-o aplicar-se só à sessão atual. Por outro lado, o âmbito `CurrentUser` altera o contexto em todas as sessões, em vez de apenas na sessão atual.

Por exemplo, para alterar o contexto predefinido na sessão atual do PowerShell sem causar impacto noutras janelas ou no contexto utilizado da próxima vez que abrir uma sessão, utilize:

```azurepowershell-interactive
PS C:\> Select-AzureRmContext Contoso1 -Scope Process
```

## <a name="how-the-context-autosave-setting-is-remembered"></a>Como a definição de gravação automática do contexto é memorizada

A definição de Gravação Automática do contexto é guardada no diretório do Azure PowerShell do utilizador (`%AppData%\Roaming\Windows Azure PowerShell`). Alguns tipos de contas de computador podem não ter acesso a este diretório. Para estes cenários, pode utilizar a variável de ambiente

```azurepowershell-interactive
$env:AzureRmContextAutoSave="true" | "false"
```

Quando definido para "true", o contexto é guardado automaticamente. Se definido para "false", o contexto não é guardado.

## <a name="changes-to-the-azurermprofile-module"></a>Alterações ao módulo AzureRM.Profile

Novos cmdlets para gerir o contexto

- [Enable-AzureRmContextAutosave][enable] - permite guardar o contexto entre sessões do Powershell.
  Quaisquer alterações alteram o contexto global.
- [Disable-AzureRmContextAutosave][disable] - desativa a gravação automática do contexto. Em cada nova sessão do PowerShell, é pedido ao utilizador que inicie sessão novamente.
- [Select-AzureRmContext][select] - seleciona um contexto como predefinição. Todos os cmdlets utilizam as credenciais neste contexto para a autenticação.
- [Disconnect-AzureRmAccount][remove-cred] - remove todas as credenciais e os contextos associados a uma conta.
- [Remove-AzureRmContext][remove-context] - remove um contexto nomeado.
- [Rename-AzureRmContext][rename] - muda o nome de um contexto existente.

Alterações aos cmdlets do perfil existente

- [Add-AzureRmAccount][login] - permite o controlo do âmbito do início de sessão para o processo ou utilizador atual.
  Permitir nomear o contexto predefinido após a autenticação.
- [Import-AzureRmContext][import] - permite o controlo do âmbito do início de sessão para o processo ou utilizador atual.
- [Set-AzureRmContext][set-context] - permite a seleção de contextos nomeados existentes e alterações de âmbito no processo ou utilizador atual.

<!-- Hyperlinks -->
[enable]: /powershell/module/azurerm.profile/Enable-AzureRmContextAutosave
[disable]: /powershell/module/azurerm.profile/Disable-AzureRmContextAutosave
[select]: /powershell/module/azurerm.profile/Select-AzureRmContext
[remove-cred]: /powershell/module/azurerm.profile/Disconnect-AzureRmAccount
[remove-context]: /powershell/module/azurerm.profile/Remove-AzureRmContext
[rename]: /powershell/module/azurerm.profile/Rename-AzureRmContext

<!-- Updated cmdlets -->
[login]: /powershell/module/azurerm.profile/Connect-AzureRmAccount
[import]:  /powershell/module/azurerm.profile/Import-AzureRmContext
[set-context]: /powershell/module/azurerm.profile/Set-AzureRmContext
