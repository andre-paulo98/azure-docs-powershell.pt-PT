---
title: Contextos e credenciais de início de sessão do Azure
description: Saiba como reutilizar as credenciais do Azure e outras informações entre várias sessões do PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: b75382d09e01dc242acf37a1652ec265266eaf7f
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243009"
---
# <a name="azure-powershell-context-objects"></a><span data-ttu-id="f5906-103">Objetos de contexto do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f5906-103">Azure PowerShell context objects</span></span>

<span data-ttu-id="f5906-104">O Azure PowerShell utiliza _objetos de contexto do Azure PowerShell_  (contextos do Azure) para manter as informações de subscrição e autenticação.</span><span class="sxs-lookup"><span data-stu-id="f5906-104">Azure PowerShell uses _Azure PowerShell context objects_ (Azure contexts) to hold subscription and authentication information.</span></span> <span data-ttu-id="f5906-105">Se tiver mais do que uma subscrição, os contextos do Azure permitem-lhe selecionar a subscrição na qual executar os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5906-105">If you have more than one subscription, Azure contexts let you select the subscription to run Azure PowerShell cmdlets on.</span></span> <span data-ttu-id="f5906-106">Os contextos do Azure também servem para armazenar informações de início de sessão em várias sessões do PowerShell e executar tarefas em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="f5906-106">Azure contexts are also used to store sign-in information across multiple PowerShell sessions and run background tasks.</span></span>

<span data-ttu-id="f5906-107">Este artigo aborda a gestão de contextos do Azure, não a gestão de subscrições ou contas.</span><span class="sxs-lookup"><span data-stu-id="f5906-107">This article covers managing Azure contexts, not the management of subscriptions or accounts.</span></span> <span data-ttu-id="f5906-108">Se está à procura de informações sobre a gestão de utilizadores, subscrições, inquilinos ou outras informações sobre contas, veja a documentação do [Azure Active Directory](/azure/active-directory).</span><span class="sxs-lookup"><span data-stu-id="f5906-108">If you're looking to manage users, subscriptions, tenants, or other account information, see the [Azure Active Directory](/azure/active-directory) documentation.</span></span> <span data-ttu-id="f5906-109">Para obter informações sobre a utilização de contextos para executar tarefas em segundo plano ou em paralelo, veja [Executar cmdlets do Azure PowerShell em tarefas do PowerShell ](using-psjobs.md) depois de se familiarizar com os contextos do Azure.</span><span class="sxs-lookup"><span data-stu-id="f5906-109">To learn about using contexts for running background or parallel tasks, see [Use Azure PowerShell cmdlets in PowerShell jobs](using-psjobs.md) after becoming familiar with Azure contexts.</span></span>

## <a name="overview-of-azure-context-objects"></a><span data-ttu-id="f5906-110">Descrição geral dos objetos de contexto do Azure</span><span class="sxs-lookup"><span data-stu-id="f5906-110">Overview of Azure context objects</span></span>

<span data-ttu-id="f5906-111">Os contextos do Azure são objetos do PowerShell que representam a sua subscrição ativa na qual executar comandos e as informações de autenticação necessárias para se ligar a uma cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="f5906-111">Azure contexts are PowerShell objects representing your active subscription to run commands against, and the authentication information needed to connect to an Azure cloud.</span></span> <span data-ttu-id="f5906-112">Com os contextos do Azure, o Azure PowerShell não precisa de reautenticar a sua conta sempre que muda de subscrição.</span><span class="sxs-lookup"><span data-stu-id="f5906-112">With Azure contexts, Azure PowerShell doesn't need to reauthenticate your account each time you switch subscriptions.</span></span> <span data-ttu-id="f5906-113">Um contexto do Azure é composto por:</span><span class="sxs-lookup"><span data-stu-id="f5906-113">An Azure context consists of:</span></span>

* <span data-ttu-id="f5906-114">A _conta_ que foi utilizada para iniciar sessão no Azure com [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="f5906-114">The _account_ that was used to sign in to Azure with [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span></span> <span data-ttu-id="f5906-115">Os contextos do Azure tratam os utilizadores, IDs de aplicação e principais de serviço da mesma forma de uma perspetiva de conta.</span><span class="sxs-lookup"><span data-stu-id="f5906-115">Azure contexts treat users, application IDs, and service principals the same from an account perspective.</span></span>
* <span data-ttu-id="f5906-116">A _subscrição_ ativa, um contrato de serviço com a Microsoft para criar e executar recursos do Azure, que estão associados a um _inquilino_.</span><span class="sxs-lookup"><span data-stu-id="f5906-116">The active _subscription_, a service agreement with Microsoft to create and run Azure resources, which are associated with a _tenant_.</span></span> <span data-ttu-id="f5906-117">Os inquilinos são frequentemente designados por _organizações_ na documentação ou ao trabalhar com o Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f5906-117">Tenants are often referred to as _organizations_ in documentation or when working with Active Directory.</span></span>
* <span data-ttu-id="f5906-118">Uma referência a uma _cache de tokens_, um token de autenticação armazenado para aceder a uma cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="f5906-118">A reference to a _token cache_, a stored authentication token for accessing an Azure cloud.</span></span> <span data-ttu-id="f5906-119">As [definições de gravação automática do contexto](#save-azure-contexts-across-powershell-sessions) determinam o local onde este token é armazenado e o tempo durante o qual persiste.</span><span class="sxs-lookup"><span data-stu-id="f5906-119">Where this token is stored and how long it persists for is determined by the [context autosave settings](#save-azure-contexts-across-powershell-sessions).</span></span>

<span data-ttu-id="f5906-120">Para obter mais informações sobre estes termos, veja a [Terminologia do Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis#terminology).</span><span class="sxs-lookup"><span data-stu-id="f5906-120">For more information on these terms, see [Azure Active Directory Terminology](/azure/active-directory/fundamentals/active-directory-whatis#terminology).</span></span> <span data-ttu-id="f5906-121">Os tokens de autenticação utilizados pelos contextos do Azure são os mesmos que outros tokens armazenados que fazem parte de uma sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="f5906-121">Authentication tokens used by Azure contexts are the same as other stored tokens that are part of a persistent session.</span></span> 

<span data-ttu-id="f5906-122">Quando inicia sessão com `Connect-AzAccount`, pelo menos um contexto do Azure é criado para a sua subscrição predefinida.</span><span class="sxs-lookup"><span data-stu-id="f5906-122">When you sign in with `Connect-AzAccount`, at least one Azure context is created for your default subscription.</span></span> <span data-ttu-id="f5906-123">O objeto devolvido por `Connect-AzAccount` é o contexto predefinido do Azure utilizado durante o resto da sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5906-123">The object returned by `Connect-AzAccount` is the default Azure context used for the rest of the PowerShell session.</span></span>

## <a name="get-azure-contexts"></a><span data-ttu-id="f5906-124">Obter contextos do Azure</span><span class="sxs-lookup"><span data-stu-id="f5906-124">Get Azure contexts</span></span>

<span data-ttu-id="f5906-125">Os contextos disponíveis do Azure são obtidos com o cmdlet [Get-AzContext](/powershell/module/az.accounts/get-azcontext).</span><span class="sxs-lookup"><span data-stu-id="f5906-125">Available Azure contexts are retrieved with the [Get-AzContext](/powershell/module/az.accounts/get-azcontext) cmdlet.</span></span> <span data-ttu-id="f5906-126">Liste todos os contextos disponíveis com `-ListAvailable`:</span><span class="sxs-lookup"><span data-stu-id="f5906-126">List all of the available contexts with `-ListAvailable`:</span></span>

```azurepowershell-interactive
Get-AzContext -ListAvailable
```

<span data-ttu-id="f5906-127">Ou obtenha um contexto por nome:</span><span class="sxs-lookup"><span data-stu-id="f5906-127">Or get a context by name:</span></span>

```azurepowershell-interactive
$context = Get-Context -Name "mycontext"
```

<span data-ttu-id="f5906-128">Os nomes dos contextos podem ser diferentes do nome da subscrição associada.</span><span class="sxs-lookup"><span data-stu-id="f5906-128">Context names may be different from the name of the associated subscription.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f5906-129">Os contextos do Azure disponíveis __não são__ sempre as suas subscrições disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f5906-129">The available Azure contexts __aren't__ always your available subscriptions.</span></span> <span data-ttu-id="f5906-130">Os contextos do Azure representam apenas informações armazenadas localmente.</span><span class="sxs-lookup"><span data-stu-id="f5906-130">Azure contexts only represent locally-stored information.</span></span> <span data-ttu-id="f5906-131">Pode obter as suas subscrições com o cmdlet [Get-AzSubscription](/powershell/module/Az.Accounts/Get-AzSubscription?view=azps-1.8.0).</span><span class="sxs-lookup"><span data-stu-id="f5906-131">You can get your subscriptions with the [Get-AzSubscription](/powershell/module/Az.Accounts/Get-AzSubscription?view=azps-1.8.0) cmdlet.</span></span>

## <a name="create-a-new-azure-context-from-subscription-information"></a><span data-ttu-id="f5906-132">Criar um novo contexto do Azure a partir de informações de subscrição</span><span class="sxs-lookup"><span data-stu-id="f5906-132">Create a new Azure context from subscription information</span></span>

<span data-ttu-id="f5906-133">O cmdlet [Set-AzContext](/powershell/module/Az.Accounts/Set-AzContext?view=azps-1.8.0) serve para criar novos contextos do Azure e para defini-los como o contexto ativo.</span><span class="sxs-lookup"><span data-stu-id="f5906-133">The [Set-AzContext](/powershell/module/Az.Accounts/Set-AzContext?view=azps-1.8.0) cmdlet is used to both create new Azure contexts and set them as the active context.</span></span>
<span data-ttu-id="f5906-134">A forma mais fácil de criar um novo contexto do Azure é utilizar as informações de subscrição existentes.</span><span class="sxs-lookup"><span data-stu-id="f5906-134">The easiest way to create a new Azure context is to use existing subscription information.</span></span> <span data-ttu-id="f5906-135">O cmdlet destina-se a retirar o objeto de saída de `Get-AzSubscription` como um valor encaminhado e configurar um novo contexto do Azure:</span><span class="sxs-lookup"><span data-stu-id="f5906-135">The cmdlet is designed to take the output object from `Get-AzSubscription` as a piped value and configure a new Azure context:</span></span>

```azurepowershell-interactive
Get-AzSubscription -SubscriptionName 'MySubscriptionName' | Set-AzContext -Name 'MyContextName'
```

<span data-ttu-id="f5906-136">Ou indique o ID ou nome da subscrição e o ID do inquilino, se necessário:</span><span class="sxs-lookup"><span data-stu-id="f5906-136">Or give the subscription name or ID and the tenant ID if necessary:</span></span>

```azurepowershell-interactive
Set-AzContext -Name 'MyContextName' -Subscription 'MySubscriptionName' -Tenant '.......'
```

<span data-ttu-id="f5906-137">Se o argumento `-Name` for omitido, o nome e o ID da subscrição são utilizados como o nome do contexto no formato `Subscription Name (subscription-id)`.</span><span class="sxs-lookup"><span data-stu-id="f5906-137">If the `-Name` argument is omitted, then the subscription's name and ID are used as the context name in the format `Subscription Name (subscription-id)`.</span></span>

## <a name="change-the-active-azure-context"></a><span data-ttu-id="f5906-138">Alterar o contexto ativo do Azure</span><span class="sxs-lookup"><span data-stu-id="f5906-138">Change the active Azure context</span></span>

<span data-ttu-id="f5906-139">Tanto `Set-AzContext` como [Select-AzContext](/powershell/module/az.accounts/set-azcontext?view=azps-1.8.0) podem ser utilizados para alterar o contexto ativo do Azure.</span><span class="sxs-lookup"><span data-stu-id="f5906-139">Both `Set-AzContext` and [Select-AzContext](/powershell/module/az.accounts/set-azcontext?view=azps-1.8.0) can be used to change the active Azure context.</span></span> <span data-ttu-id="f5906-140">Conforme descrito em [Criar um novo contexto do Azure ](#create-a-new-azure-context-from-subscription-information), `Set-AzContext` cria um novo contexto do Azure para uma subscrição, caso não exista um, e, em seguida, passa a utilizar esse contexto como o contexto ativo.</span><span class="sxs-lookup"><span data-stu-id="f5906-140">As described in [Create a new Azure context](#create-a-new-azure-context-from-subscription-information), `Set-AzContext` creates a new Azure context for a subscription if one doesn't exist, and then switches to use that context as the active one.</span></span>

<span data-ttu-id="f5906-141">`Select-AzContext` destina-se a ser utilizado apenas com contextos existentes do Azure e funciona de forma semelhante a `Set-AzContext -Context`, mas foi projetado para ser utilizado com encaminhamento:</span><span class="sxs-lookup"><span data-stu-id="f5906-141">`Select-AzContext` is meant to be used with existing Azure contexts only and works similarly to using `Set-AzContext -Context`, but is designed for use with piping:</span></span>

```azurepowershell-interactive
Set-AzContext -Context $(Get-AzContext -Name "mycontext") # Set a context with an inline Azure context object
Get-AzContext -Name "mycontext" | Select-AzContext # Set a context with a piped Azure context object
```

<span data-ttu-id="f5906-142">Tal como muitos outros comandos de gestão de contas e contextos no Azure PowerShell, `Set-AzContext` e `Select-AzContext` suportam o argumento `-Scope`, para que possa controlar durante quanto tempo o contexto está ativo.</span><span class="sxs-lookup"><span data-stu-id="f5906-142">Like many other account and context management commands in Azure PowerShell, `Set-AzContext` and `Select-AzContext` support the `-Scope` argument so that you can control how long the context is active.</span></span> <span data-ttu-id="f5906-143">`-Scope` permite-lhe alterar o contexto ativo de uma única sessão sem alterar a predefinição:</span><span class="sxs-lookup"><span data-stu-id="f5906-143">`-Scope` lets you change a single session's active context without changing the default:</span></span>

```azurepowershell-interactive
Get-AzContext -Name "mycontext" | Select-AzContext -Scope Process
```

<span data-ttu-id="f5906-144">Para evitar a mudança de contexto durante a totalidade de uma sessão do PowerShell, todos os comandos do Azure PowerShell podem ser executados num determinado contexto com o argumento `-AzContext`:</span><span class="sxs-lookup"><span data-stu-id="f5906-144">To avoid switching contexts for a whole PowerShell session, all Azure PowerShell commands can be run against a given context with the `-AzContext` argument:</span></span>

```azurepowershell-interactive
$context = Get-AzContext -Name "mycontext"
New-AzVM -Name ExampleVM -AzContext $context
```

<span data-ttu-id="f5906-145">A outra principal utilização dos contextos com os cmdlets do Azure PowerShell é para executar comandos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="f5906-145">The other main use of contexts with Azure PowerShell cmdlets is to run background commands.</span></span> <span data-ttu-id="f5906-146">Para obter mais informações sobre a execução de Tarefas do PowerShell com o Azure PowerShell, veja [Executar cmdlets do Azure PowerShell em Tarefas do PowerShell](using-psjobs.md).</span><span class="sxs-lookup"><span data-stu-id="f5906-146">To learn more about running PowerShell Jobs using Azure PowerShell, see [Run Azure PowerShell cmdlets in PowerShell Jobs](using-psjobs.md).</span></span>

## <a name="save-azure-contexts-across-powershell-sessions"></a><span data-ttu-id="f5906-147">Guardar contextos do Azure entre sessões do PowerShell</span><span class="sxs-lookup"><span data-stu-id="f5906-147">Save Azure contexts across PowerShell sessions</span></span>

<span data-ttu-id="f5906-148">Por predefinição, os contextos do Azure são guardados para serem utilizados entre as sessões do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5906-148">By default, Azure contexts are saved for use between PowerShell sessions.</span></span> <span data-ttu-id="f5906-149">Pode alterar este comportamento das seguintes formas:</span><span class="sxs-lookup"><span data-stu-id="f5906-149">You change this behavior in the following ways:</span></span>

* <span data-ttu-id="f5906-150">Iniciar sessão com `-Scope Process` com `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="f5906-150">Sign in using `-Scope Process` with `Connect-AzAccount`.</span></span>

  ```azurepowershell
  Connect-AzAccount -Scope Process
  ```

  <span data-ttu-id="f5906-151">O contexto do Azure devolvido como parte deste início de sessão é válido _apenas_ para a sessão atual e não será automaticamente guardado, independentemente da definição de gravação automática do contexto do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5906-151">The Azure context returned as part of this sign in is valid for the current session _only_ and will not be automatically saved, regardless of the Azure PowerShell context autosave setting.</span></span>
* <span data-ttu-id="f5906-152">Desative a gravação automática do contexto do Azure Powershell com o cmdlet [Disable-AzContextAutosave](/powershell/module/az.accounts/disable-azcontextautosave).</span><span class="sxs-lookup"><span data-stu-id="f5906-152">Disable AzurePowershell's context autosave with the [Disable-AzContextAutosave](/powershell/module/az.accounts/disable-azcontextautosave) cmdlet.</span></span>
  <span data-ttu-id="f5906-153">A desativação da gravação automática do contexto __não__ limpa os tokens armazenados.</span><span class="sxs-lookup"><span data-stu-id="f5906-153">Disabling context autosave __doesn't__ clear any stored tokens.</span></span> <span data-ttu-id="f5906-154">Para saber como limpar as informações de contexto do Azure armazenadas, veja [Remover as credenciais e os contextos do Azure](#remove-azure-contexts-and-stored-credentials).</span><span class="sxs-lookup"><span data-stu-id="f5906-154">To learn how to clear stored Azure context information, see [Remove Azure contexts and credentials](#remove-azure-contexts-and-stored-credentials).</span></span>
* <span data-ttu-id="f5906-155">Pode ativar explicitamente a gravação automática do contexto do Azure com o cmdlet [Enable-AzContextAutosave](/powershell/module/az.accounts/enable-azcontextautosave).</span><span class="sxs-lookup"><span data-stu-id="f5906-155">Explicitly enable Azure context autosave can be enabled with the [Enable-AzContextAutosave](/powershell/module/az.accounts/enable-azcontextautosave) cmdlet.</span></span> <span data-ttu-id="f5906-156">Com a gravação automática ativada, todos os contextos de um utilizador são armazenados localmente para sessões posteriores do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5906-156">With autosave enabled, all of a user's contexts are stored locally for later PowerShell sessions.</span></span>
* <span data-ttu-id="f5906-157">Guarde manualmente os contextos com [Save-AzContext](/powershell/module/az.accounts/save-azcontext) para serem utilizados em sessões futuras do PowerShell, onde podem ser carregados com [Import-AzContext](/powershell/module/az.accounts/import-azcontext):</span><span class="sxs-lookup"><span data-stu-id="f5906-157">Manually save contexts with [Save-AzContext](/powershell/module/az.accounts/save-azcontext) to be used in future PowerShell sessions, where they can be loaded with [Import-AzContext](/powershell/module/az.accounts/import-azcontext):</span></span>

  ```azurepowershell
  Save-AzContext -Path current-context.json # Save the current context
  Save-AzContext -Profile $profileObject -Path other-context.json # Save a context object
  Import-AzContext -Path other-context.json # Load the context from a file and set it to the current context
  ```

> [!WARNING]
> <span data-ttu-id="f5906-158">Desativar a gravação automática do contexto __não__ limpa as informações de contexto armazenadas que foram guardadas.</span><span class="sxs-lookup"><span data-stu-id="f5906-158">Disabling context autosave __doesn't__ clear any stored context information that was saved.</span></span> <span data-ttu-id="f5906-159">Para remover as informações armazenadas, utilize o cmdlet [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext).</span><span class="sxs-lookup"><span data-stu-id="f5906-159">To remove stored information, use the [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext) cmdlet.</span></span> <span data-ttu-id="f5906-160">Para obter mais informações sobre como remover contextos guardados, veja [Remover credenciais e contextos](#remove-azure-contexts-and-stored-credentials).</span><span class="sxs-lookup"><span data-stu-id="f5906-160">For more on removing saved contexts, see [Remove contexts and credentials](#remove-azure-contexts-and-stored-credentials).</span></span>

<span data-ttu-id="f5906-161">Cada um destes comandos suporta o parâmetro `-Scope`, que pode retirar um valor de `Process` para aplicar apenas ao processo que está em execução.</span><span class="sxs-lookup"><span data-stu-id="f5906-161">Each of these commands supports the `-Scope` parameter, which can take a value of `Process` to only apply to the current running process.</span></span> <span data-ttu-id="f5906-162">Por exemplo, para garantir que os contextos recém-criados não são guardados depois de sair de uma sessão do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f5906-162">For example, to ensure that newly created contexts aren't saved after exiting a PowerShell session:</span></span>

```azurepowershell-interactive
Disable-AzContextAutosave -Scope Process
$context2 = Set-AzContext -Subscription "sub-id" -Tenant "other-tenant"
```

<span data-ttu-id="f5906-163">As informações de contexto e os tokens são armazenados no diretório `$env:USERPROFILE\.Azure` no Windows e em `$HOME/.Azure` noutras plataformas.</span><span class="sxs-lookup"><span data-stu-id="f5906-163">Context information and tokens are stored in the `$env:USERPROFILE\.Azure` directory on Windows, and on `$HOME/.Azure` on other platforms.</span></span> <span data-ttu-id="f5906-164">As informações confidenciais, como os IDs de subscrição e os IDs de inquilino, ainda podem ser expostas nas informações armazenadas através de registos ou contextos guardados.</span><span class="sxs-lookup"><span data-stu-id="f5906-164">Sensitive information such as subscription IDs and tenant IDs may still be exposed in stored information, through logs or saved contexts.</span></span> <span data-ttu-id="f5906-165">Para saber como limpar as informações armazenadas, veja a secção [Remover credenciais e contextos](#remove-azure-contexts-and-stored-credentials).</span><span class="sxs-lookup"><span data-stu-id="f5906-165">To learn how to clear stored information, see the [Remove contexts and credentials](#remove-azure-contexts-and-stored-credentials) section.</span></span>

## <a name="remove-azure-contexts-and-stored-credentials"></a><span data-ttu-id="f5906-166">Remover credenciais armazenadas e contextos do Azure</span><span class="sxs-lookup"><span data-stu-id="f5906-166">Remove Azure contexts and stored credentials</span></span>

<span data-ttu-id="f5906-167">Para limpar as credenciais e os contextos do Azure:</span><span class="sxs-lookup"><span data-stu-id="f5906-167">To clear Azure contexts and credentials:</span></span>

* <span data-ttu-id="f5906-168">Termine sessão de uma conta com [Disconnect-AzAccount](/powershell/module/az.accounts/disconnect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="f5906-168">Sign out of an account with [Disconnect-AzAccount](/powershell/module/az.accounts/disconnect-azaccount).</span></span>
  <span data-ttu-id="f5906-169">Pode terminar sessão de qualquer conta através da conta ou do contexto:</span><span class="sxs-lookup"><span data-stu-id="f5906-169">You can sign out of any account either by account or context:</span></span>

  ```azurepowershell-interactive
  Disconnect-AzAccount # Disconnect active account 
  Disconnect-AzAccount -Username "user@contoso.com" # Disconnect by account name

  Disconnect-AzAccount -ContextName "subscription2" # Disconnect by context name
  Disconnect-AzAccount -AzureContext $contextObject # Disconnect using context object information
  ```

  <span data-ttu-id="f5906-170">Desligar remove sempre os tokens de autenticação armazenados e limpa os contextos guardados associados ao contexto ou utilizador desligado.</span><span class="sxs-lookup"><span data-stu-id="f5906-170">Disconnecting always removes stored authentication tokens and clears saved contexts associated with the disconnected user or context.</span></span>
* <span data-ttu-id="f5906-171">Utilize [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext).</span><span class="sxs-lookup"><span data-stu-id="f5906-171">Use [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext).</span></span> <span data-ttu-id="f5906-172">Este cmdlet garante que os tokens de autenticação e os contextos armazenados são sempre removidos, e também termina a sua sessão.</span><span class="sxs-lookup"><span data-stu-id="f5906-172">This cmdlet is guaranteed to always remove stored contexts and authentication tokens, and will also sign you out.</span></span>
* <span data-ttu-id="f5906-173">Remova um contexto com [Remove-AzContext](/powershell/module/az.accounts/remove-azcontext):</span><span class="sxs-lookup"><span data-stu-id="f5906-173">Remove a context with [Remove-AzContext](/powershell/module/az.accounts/remove-azcontext):</span></span>
  
  ```azurepowershell-interactive
  Remove-AzContext -Name "mycontext" # Remove by name
  Get-AzContext -Name "mycontext" | Remove-AzContext # Remove by piping Azure context object
  ```

  <span data-ttu-id="f5906-174">Se remover o contexto ativo, será desligado do Azure e terá de se autenticar novamente com `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="f5906-174">If you remove the active context, you will be disconnected from Azure and need to reauthenticate with `Connect-AzAccount`.</span></span>

## <a name="see-also"></a><span data-ttu-id="f5906-175">Consulte também</span><span class="sxs-lookup"><span data-stu-id="f5906-175">See also</span></span>

* [<span data-ttu-id="f5906-176">Executar cmdlets do Azure PowerShell em Tarefas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="f5906-176">Run Azure PowerShell cmdlets in PowerShell Jobs</span></span>](using-psjobs.md)
* [<span data-ttu-id="f5906-177">Terminologia do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f5906-177">Azure Active Directory Terminology</span></span>](/azure/active-directory/fundamentals/active-directory-whatis#terminology)
* [<span data-ttu-id="f5906-178">Referência de Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f5906-178">Az.Accounts reference</span></span>](/powershell/module/az.accounts)
