---
title: Contextos e credenciais de início de sessão do Azure
description: Saiba como reutilizar as credenciais do Azure e outras informações entre várias sessões do PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.openlocfilehash: c79d1d634d5b76b2c6ab6b6ab309c2d49f9f7678
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386090"
---
# <a name="azure-powershell-context-objects"></a>Objetos de contexto do Azure PowerShell

O Azure PowerShell utiliza _objetos de contexto do Azure PowerShell_  (contextos do Azure) para manter as informações de subscrição e autenticação. Se tiver mais do que uma subscrição, os contextos do Azure permitem-lhe selecionar a subscrição na qual executar os cmdlets do Azure PowerShell. Os contextos do Azure também servem para armazenar informações de início de sessão em várias sessões do PowerShell e executar tarefas em segundo plano.

Este artigo aborda a gestão de contextos do Azure, não a gestão de subscrições ou contas. Se está à procura de informações sobre a gestão de utilizadores, subscrições, inquilinos ou outras informações sobre contas, veja a documentação do [Azure Active Directory](/azure/active-directory). Para obter informações sobre a utilização de contextos para executar tarefas em segundo plano ou em paralelo, veja [Executar cmdlets do Azure PowerShell em tarefas do PowerShell ](using-psjobs.md) depois de se familiarizar com os contextos do Azure.

## <a name="overview-of-azure-context-objects"></a>Descrição geral dos objetos de contexto do Azure

Os contextos do Azure são objetos do PowerShell que representam a sua subscrição ativa na qual executar comandos e as informações de autenticação necessárias para se ligar a uma cloud do Azure. Com os contextos do Azure, o Azure PowerShell não precisa de reautenticar a sua conta sempre que muda de subscrição. Um contexto do Azure é composto por:

* A _conta_ que foi utilizada para iniciar sessão no Azure com [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount). Os contextos do Azure tratam os utilizadores, IDs de aplicação e principais de serviço da mesma forma de uma perspetiva de conta.
* A _subscrição_ ativa, um contrato de serviço com a Microsoft para criar e executar recursos do Azure, que estão associados a um _inquilino_. Os inquilinos são frequentemente designados por _organizações_ na documentação ou ao trabalhar com o Active Directory.
* Uma referência a uma _cache de tokens_, um token de autenticação armazenado para aceder a uma cloud do Azure. As [definições de gravação automática do contexto](#save-azure-contexts-across-powershell-sessions) determinam o local onde este token é armazenado e o tempo durante o qual persiste.

Para obter mais informações sobre estes termos, veja a [Terminologia do Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis#terminology). Os tokens de autenticação utilizados pelos contextos do Azure são os mesmos que outros tokens armazenados que fazem parte de uma sessão persistente. 

Quando inicia sessão com `Connect-AzAccount`, pelo menos um contexto do Azure é criado para a sua subscrição predefinida. O objeto devolvido por `Connect-AzAccount` é o contexto predefinido do Azure utilizado durante o resto da sessão do PowerShell.

## <a name="get-azure-contexts"></a>Obter contextos do Azure

Os contextos disponíveis do Azure são obtidos com o cmdlet [Get-AzContext](/powershell/module/az.accounts/get-azcontext). Liste todos os contextos disponíveis com `-ListAvailable`:

```azurepowershell-interactive
Get-AzContext -ListAvailable
```

Ou obtenha um contexto por nome:

```azurepowershell-interactive
$context = Get-AzContext -Name "mycontext"
```

Os nomes dos contextos podem ser diferentes do nome da subscrição associada.

> [!IMPORTANT]
> Os contextos do Azure disponíveis __não são__ sempre as suas subscrições disponíveis. Os contextos do Azure representam apenas informações armazenadas localmente. Pode obter as suas subscrições com o cmdlet [Get-AzSubscription](/powershell/module/Az.Accounts/Get-AzSubscription?view=azps-1.8.0).

## <a name="create-a-new-azure-context-from-subscription-information"></a>Criar um novo contexto do Azure a partir de informações de subscrição

O cmdlet [Set-AzContext](/powershell/module/Az.Accounts/Set-AzContext) serve para criar novos contextos do Azure e para defini-los como o contexto ativo.
A forma mais fácil de criar um novo contexto do Azure é utilizar as informações de subscrição existentes. O cmdlet destina-se a retirar o objeto de saída de `Get-AzSubscription` como um valor encaminhado e configurar um novo contexto do Azure:

```azurepowershell-interactive
Get-AzSubscription -SubscriptionName 'MySubscriptionName' | Set-AzContext -Name 'MyContextName'
```

Ou indique o ID ou nome da subscrição e o ID do inquilino, se necessário:

```azurepowershell-interactive
Set-AzContext -Name 'MyContextName' -Subscription 'MySubscriptionName' -Tenant '.......'
```

Se o argumento `-Name` for omitido, o nome e o ID da subscrição são utilizados como o nome do contexto no formato `Subscription Name (subscription-id)`.

## <a name="change-the-active-azure-context"></a>Alterar o contexto ativo do Azure

Tanto `Set-AzContext` como [Select-AzContext](/powershell/module/az.accounts/set-azcontext) podem ser utilizados para alterar o contexto ativo do Azure. Conforme descrito em [Criar um novo contexto do Azure ](#create-a-new-azure-context-from-subscription-information), `Set-AzContext` cria um novo contexto do Azure para uma subscrição, caso não exista um, e, em seguida, passa a utilizar esse contexto como o contexto ativo.

`Select-AzContext` destina-se a ser utilizado apenas com contextos existentes do Azure e funciona de forma semelhante a `Set-AzContext -Context`, mas foi projetado para ser utilizado com encaminhamento:

```azurepowershell-interactive
Set-AzContext -Context $(Get-AzContext -Name "mycontext") # Set a context with an inline Azure context object
Get-AzContext -Name "mycontext" | Select-AzContext # Set a context with a piped Azure context object
```

Tal como muitos outros comandos de gestão de contas e contextos no Azure PowerShell, `Set-AzContext` e `Select-AzContext` suportam o argumento `-Scope`, para que possa controlar durante quanto tempo o contexto está ativo. `-Scope` permite-lhe alterar o contexto ativo de uma única sessão sem alterar a predefinição:

```azurepowershell-interactive
Get-AzContext -Name "mycontext" | Select-AzContext -Scope Process
```

Para evitar a mudança de contexto durante a totalidade de uma sessão do PowerShell, todos os comandos do Azure PowerShell podem ser executados num determinado contexto com o argumento `-AzContext`:

```azurepowershell-interactive
$context = Get-AzContext -Name "mycontext"
New-AzVM -Name ExampleVM -AzContext $context
```

A outra principal utilização dos contextos com os cmdlets do Azure PowerShell é para executar comandos em segundo plano. Para obter mais informações sobre a execução de Tarefas do PowerShell com o Azure PowerShell, veja [Executar cmdlets do Azure PowerShell em Tarefas do PowerShell](using-psjobs.md).

## <a name="save-azure-contexts-across-powershell-sessions"></a>Guardar contextos do Azure entre sessões do PowerShell

Por predefinição, os contextos do Azure são guardados para serem utilizados entre as sessões do PowerShell. Pode alterar este comportamento das seguintes formas:

* Iniciar sessão com `-Scope Process` com `Connect-AzAccount`.

  ```azurepowershell
  Connect-AzAccount -Scope Process
  ```

  O contexto do Azure devolvido como parte deste início de sessão é válido _apenas_ para a sessão atual e não será automaticamente guardado, independentemente da definição de gravação automática do contexto do Azure PowerShell.
* Desative a gravação automática do contexto do Azure Powershell com o cmdlet [Disable-AzContextAutosave](/powershell/module/az.accounts/disable-azcontextautosave).
  A desativação da gravação automática do contexto __não__ limpa os tokens armazenados. Para saber como limpar as informações de contexto do Azure armazenadas, veja [Remover as credenciais e os contextos do Azure](#remove-azure-contexts-and-stored-credentials).
* Pode ativar explicitamente a gravação automática do contexto do Azure com o cmdlet [Enable-AzContextAutosave](/powershell/module/az.accounts/enable-azcontextautosave). Com a gravação automática ativada, todos os contextos de um utilizador são armazenados localmente para sessões posteriores do PowerShell.
* Guarde manualmente os contextos com [Save-AzContext](/powershell/module/az.accounts/save-azcontext) para serem utilizados em sessões futuras do PowerShell, onde podem ser carregados com [Import-AzContext](/powershell/module/az.accounts/import-azcontext):

  ```azurepowershell
  Save-AzContext -Path current-context.json # Save the current context
  Save-AzContext -Profile $profileObject -Path other-context.json # Save a context object
  Import-AzContext -Path other-context.json # Load the context from a file and set it to the current context
  ```

> [!WARNING]
> Desativar a gravação automática do contexto __não__ limpa as informações de contexto armazenadas que foram guardadas. Para remover as informações armazenadas, utilize o cmdlet [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext). Para obter mais informações sobre como remover contextos guardados, veja [Remover credenciais e contextos](#remove-azure-contexts-and-stored-credentials).

Cada um destes comandos suporta o parâmetro `-Scope`, que pode retirar um valor de `Process` para aplicar apenas ao processo que está em execução. Por exemplo, para garantir que os contextos recém-criados não são guardados depois de sair de uma sessão do PowerShell:

```azurepowershell-interactive
Disable-AzContextAutosave -Scope Process
$context2 = Set-AzContext -Subscription "sub-id" -Tenant "other-tenant"
```

As informações de contexto e os tokens são armazenados no diretório `$env:USERPROFILE\.Azure` no Windows e em `$HOME/.Azure` noutras plataformas. As informações confidenciais, como os IDs de subscrição e os IDs de inquilino, ainda podem ser expostas nas informações armazenadas através de registos ou contextos guardados. Para saber como limpar as informações armazenadas, veja a secção [Remover credenciais e contextos](#remove-azure-contexts-and-stored-credentials).

## <a name="remove-azure-contexts-and-stored-credentials"></a>Remover credenciais armazenadas e contextos do Azure

Para limpar as credenciais e os contextos do Azure:

* Termine sessão de uma conta com [Disconnect-AzAccount](/powershell/module/az.accounts/disconnect-azaccount).
  Pode terminar sessão de qualquer conta através da conta ou do contexto:

  ```azurepowershell-interactive
  Disconnect-AzAccount # Disconnect active account 
  Disconnect-AzAccount -Username "user@contoso.com" # Disconnect by account name

  Disconnect-AzAccount -ContextName "subscription2" # Disconnect by context name
  Disconnect-AzAccount -AzureContext $contextObject # Disconnect using context object information
  ```

  Desligar remove sempre os tokens de autenticação armazenados e limpa os contextos guardados associados ao contexto ou utilizador desligado.
* Utilize [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext). Este cmdlet garante que os tokens de autenticação e os contextos armazenados são sempre removidos, e também termina a sua sessão.
* Remova um contexto com [Remove-AzContext](/powershell/module/az.accounts/remove-azcontext):
  
  ```azurepowershell-interactive
  Remove-AzContext -Name "mycontext" # Remove by name
  Get-AzContext -Name "mycontext" | Remove-AzContext # Remove by piping Azure context object
  ```

  Se remover o contexto ativo, será desligado do Azure e terá de se autenticar novamente com `Connect-AzAccount`.

## <a name="see-also"></a>Consulte também

* [Executar cmdlets do Azure PowerShell em Tarefas do PowerShell](using-psjobs.md)
* [Terminologia do Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis#terminology)
* [Referência de Az.Accounts](/powershell/module/az.accounts)
