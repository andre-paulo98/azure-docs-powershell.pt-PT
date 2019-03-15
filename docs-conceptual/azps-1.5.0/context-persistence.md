---
title: Manter credenciais do utilizador nas sessões do PowerShell
description: Saiba como reutilizar as credenciais do Azure e outras informações entre várias sessões do PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 8702de48429482748939fb1a43ff911bed15f6c0
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882532"
---
# <a name="persist-user-credentials-across-powershell-sessions"></a><span data-ttu-id="28ed5-103">Manter credenciais do utilizador nas sessões do PowerShell</span><span class="sxs-lookup"><span data-stu-id="28ed5-103">Persist user credentials across PowerShell sessions</span></span>

<span data-ttu-id="28ed5-104">O Azure PowerShell oferece uma funcionalidade chamada **Gravação Automática de Contexto do Azure**, que lhe oferece as seguintes funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="28ed5-104">Azure PowerShell offers a feature called **Azure Context Autosave**, which gives the following features:</span></span>

- <span data-ttu-id="28ed5-105">Retenção de informações de início de sessão para serem reutilizadas em novas sessões do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28ed5-105">Retention of sign-in information for reuse in new PowerShell sessions.</span></span>
- <span data-ttu-id="28ed5-106">Utilização mais fácil de tarefas em segundo plano para executar os cmdlets de execução longa.</span><span class="sxs-lookup"><span data-stu-id="28ed5-106">Easier use of background tasks for executing long-running cmdlets.</span></span>
- <span data-ttu-id="28ed5-107">Alternar entre contas, subscrições e ambientes sem um início de sessão separado.</span><span class="sxs-lookup"><span data-stu-id="28ed5-107">Switch between accounts, subscriptions, and environments without a separate sign-in.</span></span>
- <span data-ttu-id="28ed5-108">Execução de tarefas com credenciais e subscrições diferentes, em simultâneo, a partir da mesma sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28ed5-108">Execution of tasks using different credentials and subscriptions, simultaneously, from the same PowerShell session.</span></span>

## <a name="azure-contexts-defined"></a><span data-ttu-id="28ed5-109">Contextos do Azure definidos</span><span class="sxs-lookup"><span data-stu-id="28ed5-109">Azure contexts defined</span></span>

<span data-ttu-id="28ed5-110">Um *contexto do Azure* é um conjunto de informações que define o destino dos cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28ed5-110">An *Azure context* is a set of information that defines the target of Azure PowerShell cmdlets.</span></span> <span data-ttu-id="28ed5-111">O contexto é composto por cinco partes:</span><span class="sxs-lookup"><span data-stu-id="28ed5-111">The context consists of five parts:</span></span>

- <span data-ttu-id="28ed5-112">Uma *Conta* - o Nome de Utilizador ou Principal de serviço utilizado para autenticar as comunicações com o Azure</span><span class="sxs-lookup"><span data-stu-id="28ed5-112">An *Account* - the UserName or Service Principal used to authenticate communications with Azure</span></span>
- <span data-ttu-id="28ed5-113">Uma *Subscrição* - a subscrição do Azure com os Recursos que estão a ser alterados.</span><span class="sxs-lookup"><span data-stu-id="28ed5-113">A *Subscription* - The Azure Subscription with the Resources being acted upon.</span></span>
- <span data-ttu-id="28ed5-114">Um *Inquilino* - o inquilino do Azure Active Directory que contém a sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="28ed5-114">A *Tenant* - The Azure Active Directory tenant that contains your subscription.</span></span> <span data-ttu-id="28ed5-115">Os inquilinos são mais importantes para a autenticação do Principal de Serviço.</span><span class="sxs-lookup"><span data-stu-id="28ed5-115">Tenants are more important to ServicePrincipal authentication.</span></span>
- <span data-ttu-id="28ed5-116">Um *Ambiente* - a cloud de destino específica do Azure, normalmente, a Cloud global do Azure.</span><span class="sxs-lookup"><span data-stu-id="28ed5-116">An *Environment* - The particular Azure Cloud being targeted, usually the Azure global Cloud.</span></span>
  <span data-ttu-id="28ed5-117">No entanto, a definição do ambiente permite-lhe visar também uma cloud Nacional, do Government e no local (Azure Stack).</span><span class="sxs-lookup"><span data-stu-id="28ed5-117">However, the environment setting allows you to target National, Government, and on-premises (Azure Stack) clouds as well.</span></span>
- <span data-ttu-id="28ed5-118">*Credenciais* - as informações utilizadas pelo Azure para verificar a sua identidade e confirmar a sua autorização para aceder a recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="28ed5-118">*Credentials* - The information used by Azure to verify your identity and confirm your authorization to access resources in Azure</span></span>

<span data-ttu-id="28ed5-119">Com a versão mais recente do Azure PowerShell, é possível guardar automaticamente os contextos do Azure sempre que for aberta uma nova sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28ed5-119">With the latest version of Azure PowerShell, Azure Contexts can automatically be saved whenever opening a new PowerShell session.</span></span>

## <a name="automatically-save-the-context-for-the-next-sign-in"></a><span data-ttu-id="28ed5-120">Guardar automaticamente o contexto para o próximo início de sessão</span><span class="sxs-lookup"><span data-stu-id="28ed5-120">Automatically save the context for the next sign-in</span></span>

<span data-ttu-id="28ed5-121">O Azure PowerShell mantém as informações de contexto automaticamente entre sessões.</span><span class="sxs-lookup"><span data-stu-id="28ed5-121">Azure PowerShell retains your context information automatically between sessions.</span></span> <span data-ttu-id="28ed5-122">Para definir o PowerShell para que esqueça o contexto e as credenciais, utilize `Disable-AzContextAutoSave`.</span><span class="sxs-lookup"><span data-stu-id="28ed5-122">To set PowerShell to forget your context and credentials, use `Disable-AzContextAutoSave`.</span></span> <span data-ttu-id="28ed5-123">Se a gravação do contexto estiver desativada, terá de iniciar sessão no Azure sempre que abrir uma sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28ed5-123">With context saving disabled, you'll need to sign in to Azure every time you open a PowerShell session.</span></span>

<span data-ttu-id="28ed5-124">Para permitir que o Azure PowerShell se lembre do contexto depois de fechar a sessão do PowerShell, utilize `Enable-AzContextAutosave`.</span><span class="sxs-lookup"><span data-stu-id="28ed5-124">To allow Azure PowerShell to remember your context after the PowerShell session is closed, use `Enable-AzContextAutosave`.</span></span> <span data-ttu-id="28ed5-125">As informações de contexto e de credenciais são guardadas automaticamente numa pasta oculta especial no seu diretório de utilizador (`$env:USERPROFILE\.Azure` no Windows e `$HOME/.Azure` noutras plataformas).</span><span class="sxs-lookup"><span data-stu-id="28ed5-125">Context and credential information are automatically saved in a special hidden folder in your user directory (`$env:USERPROFILE\.Azure` on Windows, and `$HOME/.Azure` on other platforms).</span></span> <span data-ttu-id="28ed5-126">Cada nova sessão do PowerShell visa o contexto utilizado na sua última sessão.</span><span class="sxs-lookup"><span data-stu-id="28ed5-126">Each new PowerShell session targets the context used in your last session.</span></span>

<span data-ttu-id="28ed5-127">Os cmdlets que lhe permitem gerir contextos do Azure também permitem o controlo detalhado.</span><span class="sxs-lookup"><span data-stu-id="28ed5-127">The cmdlets that allow you to manage Azure contexts also allow you fine grained control.</span></span> <span data-ttu-id="28ed5-128">Se pretender que as alterações sejam aplicadas apenas à sessão atual do PowerShell (âmbito `Process`) ou a cada sessão do PowerShell (âmbito `CurrentUser`).</span><span class="sxs-lookup"><span data-stu-id="28ed5-128">If you want changes to apply only to the current PowerShell session (`Process` scope) or every PowerShell session (`CurrentUser` scope).</span></span> <span data-ttu-id="28ed5-129">Estas opções são abordadas mais detalhadamente em [Utilizar Âmbitos de Contexto](#Using-Context-Scopes).</span><span class="sxs-lookup"><span data-stu-id="28ed5-129">These options are discussed in more detail in [Using Context Scopes](#Using-Context-Scopes).</span></span>

## <a name="running-azure-powershell-cmdlets-as-background-jobs"></a><span data-ttu-id="28ed5-130">Executar os cmdlets do Azure PowerShell como tarefas em segundo plano</span><span class="sxs-lookup"><span data-stu-id="28ed5-130">Running Azure PowerShell cmdlets as background jobs</span></span>

<span data-ttu-id="28ed5-131">A funcionalidade **Gravação Automática de Contexto do Azure** permite-lhe também partilhar o contexto com tarefas do PowerShell em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="28ed5-131">The **Azure Context Autosave** feature also allows you to share you context with PowerShell background jobs.</span></span> <span data-ttu-id="28ed5-132">O PowerShell permite-lhe iniciar e monitorizar tarefas de execução longa como tarefas em segundo plano, sem ter de aguardar a conclusão das tarefas.</span><span class="sxs-lookup"><span data-stu-id="28ed5-132">PowerShell allows you to start and monitor long-executing tasks as background jobs without having to wait for the tasks to complete.</span></span> <span data-ttu-id="28ed5-133">Pode partilhar as credenciais com tarefas em segundo plano de duas formas diferentes:</span><span class="sxs-lookup"><span data-stu-id="28ed5-133">You can share credentials with background jobs in two different ways:</span></span>

- <span data-ttu-id="28ed5-134">Passar o contexto como um argumento</span><span class="sxs-lookup"><span data-stu-id="28ed5-134">Passing the context as an argument</span></span>

  <span data-ttu-id="28ed5-135">A maioria dos cmdlets do AzureRM permitem-lhe passar o contexto como um parâmetro para o cmdlet.</span><span class="sxs-lookup"><span data-stu-id="28ed5-135">Most AzureRM cmdlets allow you to pass the context as a parameter to the cmdlet.</span></span> <span data-ttu-id="28ed5-136">Pode passar um contexto para uma tarefa em segundo plano, conforme mostrado no exemplo seguinte:</span><span class="sxs-lookup"><span data-stu-id="28ed5-136">You can pass a context to a background job as shown in the following example:</span></span>

  ```powershell-interactive
  PS C:\> $job = Start-Job { param ($ctx) New-AzVm -AzureRmContext $ctx [... Additional parameters ...]} -ArgumentList (Get-AzContext)
  ```

- <span data-ttu-id="28ed5-137">Utilizar o contexto predefinido com a Gravação Automática ativada</span><span class="sxs-lookup"><span data-stu-id="28ed5-137">Using the default context with Autosave enabled</span></span>

  <span data-ttu-id="28ed5-138">Se tiver ativado a **Gravação Automática de Contexto**, as tarefas em segundo plano utilizam automaticamente o contexto predefinido guardado.</span><span class="sxs-lookup"><span data-stu-id="28ed5-138">If you have enabled **Context Autosave**, background jobs automatically use the default saved context.</span></span>

  ```powershell-interactive
  PS C:\> $job = Start-Job { New-AzVm [... Additional parameters ...]}
  ```

<span data-ttu-id="28ed5-139">Quando precisar de saber o resultado da tarefa em segundo plano, utilize `Get-Job` para verificar o estado da tarefa e `Wait-Job` para aguardar a conclusão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="28ed5-139">When you need to know the outcome of the background task, use `Get-Job` to check the job status and `Wait-Job` to wait for the Job to complete.</span></span> <span data-ttu-id="28ed5-140">Utilize `Receive-Job` para capturar ou apresentar o resultado da tarefa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="28ed5-140">Use `Receive-Job` to capture or display the output of the background job.</span></span> <span data-ttu-id="28ed5-141">Para obter mais informações, veja [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span><span class="sxs-lookup"><span data-stu-id="28ed5-141">For more information, see [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="creating-selecting-renaming-and-removing-contexts"></a><span data-ttu-id="28ed5-142">Criar, selecionar, mudar o nome e remover contextos</span><span class="sxs-lookup"><span data-stu-id="28ed5-142">Creating, selecting, renaming, and removing contexts</span></span>

<span data-ttu-id="28ed5-143">Para criar um contexto, tem de ter sessão iniciada no Azure.</span><span class="sxs-lookup"><span data-stu-id="28ed5-143">To create a context, you must be signed in to Azure.</span></span> <span data-ttu-id="28ed5-144">O cmdlet `Connect-AzAccount` (ou o respetivo alias, `Login-AzAccount`) define o contexto predefinido utilizado por cmdlets do Azure PowerShell e permite-lhe aceder a quaisquer inquilinos ou subscrições permitidos pelas suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="28ed5-144">The `Connect-AzAccount` cmdlet (or its alias, `Login-AzAccount`) sets the default context used by Azure PowerShell cmdlets, and allows you to access any tenants or subscriptions allowed by your credentials.</span></span>

<span data-ttu-id="28ed5-145">Para adicionar um novo contexto após o início de sessão, utilize `Set-AzContext` (ou o respetivo alias, `Select-AzSubscription`).</span><span class="sxs-lookup"><span data-stu-id="28ed5-145">To add a new context after sign-in, use `Set-AzContext` (or its alias, `Select-AzSubscription`).</span></span>

```azurepowershell-interactive
PS C:\> Set-AzContext -Subscription "Contoso Subscription 1" -Name "Contoso1"
```

<span data-ttu-id="28ed5-146">O exemplo anterior adiciona um novo contexto que visa “Contoso Subscription 1”, com as suas credenciais atuais.</span><span class="sxs-lookup"><span data-stu-id="28ed5-146">The previous example adds a new context targeting 'Contoso Subscription 1' using your current credentials.</span></span> <span data-ttu-id="28ed5-147">O novo contexto tem o nome “Contoso1”.</span><span class="sxs-lookup"><span data-stu-id="28ed5-147">The new context is named 'Contoso1'.</span></span> <span data-ttu-id="28ed5-148">Se não indicar um nome para o contexto, é utilizado um nome predefinido, com o ID da conta e o ID da subscrição.</span><span class="sxs-lookup"><span data-stu-id="28ed5-148">If you don't provide a name for the context, a default name, using the account ID and subscription ID is used.</span></span>

<span data-ttu-id="28ed5-149">Para mudar o nome de um contexto existente, utilize o cmdlet `Rename-AzContext`.</span><span class="sxs-lookup"><span data-stu-id="28ed5-149">To rename an existing context, use the `Rename-AzContext` cmdlet.</span></span> <span data-ttu-id="28ed5-150">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="28ed5-150">For example:</span></span>

```azurepowershell-interactive
PS C:\> Rename-AzContext '[user1@contoso.org; 123456-7890-1234-564321]` 'Contoso2'
```

<span data-ttu-id="28ed5-151">Este exemplo muda o nome do contexto com o nome automático `[user1@contoso.org; 123456-7890-1234-564321]` para o nome simples “Contoso2”.</span><span class="sxs-lookup"><span data-stu-id="28ed5-151">This example renames the context with automatic name `[user1@contoso.org; 123456-7890-1234-564321]` to the simple name 'Contoso2'.</span></span> <span data-ttu-id="28ed5-152">Os cmdlets que gerem contextos também utilizam a conclusão de tabulação, permitindo-lhe selecionar rapidamente o contexto.</span><span class="sxs-lookup"><span data-stu-id="28ed5-152">Cmdlets that manage contexts also use tab completion, allowing you to quickly select the context.</span></span>

<span data-ttu-id="28ed5-153">Por último, para remover um contexto, utilize o cmdlet `Remove-AzContext`.</span><span class="sxs-lookup"><span data-stu-id="28ed5-153">Finally, to remove a context, use the `Remove-AzContext` cmdlet.</span></span>  <span data-ttu-id="28ed5-154">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="28ed5-154">For example:</span></span>

```azurepowershell-interactive
PS C:\> Remove-AzContext Contoso2
```

<span data-ttu-id="28ed5-155">Esquece o contexto ao qual foi dado o nome “Contoso2”.</span><span class="sxs-lookup"><span data-stu-id="28ed5-155">Forgets the context that was named 'Contoso2'.</span></span> <span data-ttu-id="28ed5-156">Pode recriar este contexto com `Set-AzContext`</span><span class="sxs-lookup"><span data-stu-id="28ed5-156">You can recreate this context using `Set-AzContext`</span></span>

## <a name="removing-credentials"></a><span data-ttu-id="28ed5-157">Remover credenciais</span><span class="sxs-lookup"><span data-stu-id="28ed5-157">Removing credentials</span></span>

<span data-ttu-id="28ed5-158">Pode remover todas as credenciais e os contextos associados de um utilizador ou principal de serviço, com `Disconnect-AzAccount` (também conhecido como `Logout-AzAccount`).</span><span class="sxs-lookup"><span data-stu-id="28ed5-158">You can remove all credentials and associated contexts for a user or service principal using `Disconnect-AzAccount` (also known as `Logout-AzAccount`).</span></span> <span data-ttu-id="28ed5-159">Quando executado sem parâmetros, o cmdlet `Disconnect-AzAccount` remove todas as credenciais e os contextos associados ao Utilizador ou Principal de Serviço no contexto atual.</span><span class="sxs-lookup"><span data-stu-id="28ed5-159">When executed without parameters, the `Disconnect-AzAccount` cmdlet removes all credentials and contexts associated with the User or Service Principal in the current context.</span></span> <span data-ttu-id="28ed5-160">Pode passar um Nome de Utilizador, Nome do Principal de Serviço ou contexto para visar um determinado principal.</span><span class="sxs-lookup"><span data-stu-id="28ed5-160">You may pass in a Username, Service Principal Name, or context to target a particular principal.</span></span>

```azurepowershell-interactive
Disconnect-AzAccount user1@contoso.org
```

## <a name="using-context-scopes"></a><span data-ttu-id="28ed5-161">Utilizar âmbitos de contexto</span><span class="sxs-lookup"><span data-stu-id="28ed5-161">Using context scopes</span></span>

<span data-ttu-id="28ed5-162">Ocasionalmente, poderá querer selecionar, alterar ou remover um contexto de uma sessão do PowerShell sem afetar outras sessões.</span><span class="sxs-lookup"><span data-stu-id="28ed5-162">Occasionally, you may want to select, change, or remove a context in a PowerShell session without impacting other sessions.</span></span> <span data-ttu-id="28ed5-163">Para alterar o comportamento predefinido de cmdlets de contexto, utilize o parâmetro `Scope`.</span><span class="sxs-lookup"><span data-stu-id="28ed5-163">To change the default behavior of context cmdlets, use the `Scope` parameter.</span></span> <span data-ttu-id="28ed5-164">O âmbito `Process` substitui o comportamento predefinido, fazendo-o aplicar-se só à sessão atual.</span><span class="sxs-lookup"><span data-stu-id="28ed5-164">The `Process` scope overrides the default behavior by making it apply only for the current session.</span></span> <span data-ttu-id="28ed5-165">Por outro lado, o âmbito `CurrentUser` altera o contexto em todas as sessões, em vez de apenas na sessão atual.</span><span class="sxs-lookup"><span data-stu-id="28ed5-165">Conversely `CurrentUser` scope changes the context in all sessions, instead of just the current session.</span></span>

<span data-ttu-id="28ed5-166">Por exemplo, para alterar o contexto predefinido na sessão atual do PowerShell sem causar impacto noutras janelas ou no contexto utilizado da próxima vez que abrir uma sessão, utilize:</span><span class="sxs-lookup"><span data-stu-id="28ed5-166">As an example, to change the default context in the current PowerShell session without impacting other windows, or the context used the next time a session is opened, use:</span></span>

```azurepowershell-interactive
PS C:\> Select-AzContext Contoso1 -Scope Process
```

## <a name="how-the-context-autosave-setting-is-remembered"></a><span data-ttu-id="28ed5-167">Como a definição de gravação automática do contexto é memorizada</span><span class="sxs-lookup"><span data-stu-id="28ed5-167">How the context autosave setting is remembered</span></span>

<span data-ttu-id="28ed5-168">A definição de Gravação Automática do contexto é guardada no diretório do Azure PowerShell do utilizador (`$env:USERPROFILE\.Azure` no Windows e `$HOME/.Azure` noutras plataformas).</span><span class="sxs-lookup"><span data-stu-id="28ed5-168">The context AutoSave setting is saved to the user Azure PowerShell directory (`$env:USERPROFILE\.Azure` on Windows, and `$HOME/.Azure` on other platforms).</span></span> <span data-ttu-id="28ed5-169">Alguns tipos de contas de computador podem não ter acesso a este diretório.</span><span class="sxs-lookup"><span data-stu-id="28ed5-169">Some kinds of computer accounts may not have access to this directory.</span></span> <span data-ttu-id="28ed5-170">Para estes cenários, pode utilizar a variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="28ed5-170">For such scenarios, you can use the environment variable</span></span>

```azurepowershell-interactive
$env:AzureRmContextAutoSave="true" | "false"
```

<span data-ttu-id="28ed5-171">Quando definido para "true", o contexto é guardado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="28ed5-171">When set to 'true', the context is automatically saved.</span></span> <span data-ttu-id="28ed5-172">Se definido para "false", o contexto não é guardado.</span><span class="sxs-lookup"><span data-stu-id="28ed5-172">If set to 'false', the context isn't saved.</span></span>

## <a name="context-management-cmdlets"></a><span data-ttu-id="28ed5-173">Cmdlets de gestão do contexto</span><span class="sxs-lookup"><span data-stu-id="28ed5-173">Context management cmdlets</span></span>

- <span data-ttu-id="28ed5-174">[Enable-AzContextAutosave][enable]: permitir a gravação do contexto entre sessões do Powershell.</span><span class="sxs-lookup"><span data-stu-id="28ed5-174">[Enable-AzContextAutosave][enable] - Allow saving the context between powershell sessions.</span></span>
  <span data-ttu-id="28ed5-175">Quaisquer alterações alteram o contexto global.</span><span class="sxs-lookup"><span data-stu-id="28ed5-175">Any changes alter the global context.</span></span>
- <span data-ttu-id="28ed5-176">[Disable-AzContextAutosave][disable]: desativar a gravação automática do contexto.</span><span class="sxs-lookup"><span data-stu-id="28ed5-176">[Disable-AzContextAutosave][disable] - Turn off autosaving the context.</span></span> <span data-ttu-id="28ed5-177">Em cada nova sessão do PowerShell, é pedido ao utilizador que inicie sessão novamente.</span><span class="sxs-lookup"><span data-stu-id="28ed5-177">Each new PowerShell session is required to sign in again.</span></span>
- <span data-ttu-id="28ed5-178">[Select-AzContext][select]: selecionar um contexto como predefinição.</span><span class="sxs-lookup"><span data-stu-id="28ed5-178">[Select-AzContext][select] - Select a context as the default.</span></span> <span data-ttu-id="28ed5-179">Todos os cmdlets utilizam as credenciais neste contexto para a autenticação.</span><span class="sxs-lookup"><span data-stu-id="28ed5-179">All cmdlets use the credentials in this context for authentication.</span></span>
- <span data-ttu-id="28ed5-180">[Disconnect-AzAccount][remove-cred]: remover todas as credenciais e os contextos associados a uma conta.</span><span class="sxs-lookup"><span data-stu-id="28ed5-180">[Disconnect-AzAccount][remove-cred] - Remove all credentials and contexts associated with an account.</span></span>
- <span data-ttu-id="28ed5-181">[Remove-AzContext][remove-context]: remover um contexto nomeado.</span><span class="sxs-lookup"><span data-stu-id="28ed5-181">[Remove-AzContext][remove-context] - Remove a named context.</span></span>
- <span data-ttu-id="28ed5-182">[Rename-AzContext][rename]: mudar o nome de um contexto existente.</span><span class="sxs-lookup"><span data-stu-id="28ed5-182">[Rename-AzContext][rename] - Rename an existing context.</span></span>
- <span data-ttu-id="28ed5-183">[Add-AzAccount][login]: permitir o controlo do âmbito do início de sessão para o processo ou utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="28ed5-183">[Add-AzAccount][login] - Allow scoping of the sign-in to the process or the current user.</span></span>
  <span data-ttu-id="28ed5-184">Permitir nomear o contexto predefinido após a autenticação.</span><span class="sxs-lookup"><span data-stu-id="28ed5-184">Allow naming the default context after authentication.</span></span>
- <span data-ttu-id="28ed5-185">[Import-AzContext][import]: permitir o controlo do âmbito do início de sessão para o processo ou utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="28ed5-185">[Import-AzContext][import] - Allow scoping of the sign-in to the process or the current user.</span></span>
- <span data-ttu-id="28ed5-186">[Set-AzContext][set-context]: permitir a seleção de contextos nomeados existentes e alterações de âmbito no processo ou utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="28ed5-186">[Set-AzContext][set-context] - Allow selection of existing named contexts, and scope changes to the process or current user.</span></span>

<!-- Hyperlinks -->
[enable]: /powershell/module/az.accounts/Enable-AzureRmContextAutosave
[disable]: /powershell/module/az.accounts/Disable-AzContextAutosave
[select]: /powershell/module/az.accounts/Select-AzContext
[remove-cred]: /powershell/module/az.accounts/Disconnect-AzAccount
[remove-context]: /powershell/module/az.accounts/Remove-AzContext
[rename]: /powershell/module/az.accounts/Rename-AzContext

<!-- Updated cmdlets -->
[login]: /powershell/module/az.accounts/Connect-AzAccount
[import]:  /powershell/module/az.accounts/Import-AzContext
[set-context]: /powershell/module/az.accounts/Set-AzContext
