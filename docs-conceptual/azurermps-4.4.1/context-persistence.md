---
title: Manter credenciais do utilizador nas sessões do PowerShell
description: Saiba como reutilizar as credenciais do Azure e outras informações entre várias sessões do PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/31/2017
ms.openlocfilehash: 442dfed6175f2f5e2f386df3cb2bcea4871bcc01
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "65854174"
---
# <a name="persisting-user-credentials-across-powershell-sessions"></a><span data-ttu-id="b2972-103">Manter credenciais do utilizador nas sessões do PowerShell</span><span class="sxs-lookup"><span data-stu-id="b2972-103">Persisting user credentials across PowerShell sessions</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="b2972-104">O Azure PowerShell oferece uma funcionalidade chamada **Gravação Automática de Contexto do Azure**, que lhe oferece as seguintes funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="b2972-104">Azure PowerShell offers a feature called **Azure Context Autosave**, which gives the following features:</span></span>

- <span data-ttu-id="b2972-105">Retenção de informações de início de sessão para serem reutilizadas em novas sessões do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-105">Retention of sign in information for reuse in new PowerShell sessions.</span></span>
- <span data-ttu-id="b2972-106">Utilização mais fácil de tarefas em segundo plano para executar os cmdlets de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b2972-106">Easier use of background tasks for executing long-running cmdlets.</span></span>
- <span data-ttu-id="b2972-107">Alternar entre contas, subscrições e ambientes sem um início de sessão separado.</span><span class="sxs-lookup"><span data-stu-id="b2972-107">Switch between accounts, subscriptions, and environments without a separate sign in.</span></span>
- <span data-ttu-id="b2972-108">Execução de tarefas com credenciais e subscrições diferentes, em simultâneo, a partir da mesma sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-108">Execution of tasks using different credentials and subscriptions, simultaneously, from the same PowerShell session.</span></span>

## <a name="azure-contexts-defined"></a><span data-ttu-id="b2972-109">Contextos do Azure definidos</span><span class="sxs-lookup"><span data-stu-id="b2972-109">Azure contexts defined</span></span>

<span data-ttu-id="b2972-110">Um *contexto do Azure* é um conjunto de informações que define o destino dos cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-110">An *Azure context* is a set of information that defines the target of Azure PowerShell cmdlets.</span></span> <span data-ttu-id="b2972-111">O contexto é composto por cinco partes:</span><span class="sxs-lookup"><span data-stu-id="b2972-111">The context consists of five parts:</span></span>

- <span data-ttu-id="b2972-112">Uma *Conta* - o Nome de Utilizador ou Principal de serviço utilizado para autenticar as comunicações com o Azure</span><span class="sxs-lookup"><span data-stu-id="b2972-112">An *Account* - the UserName or Service Principal used to authenticate communications with Azure</span></span>
- <span data-ttu-id="b2972-113">Uma *Subscrição* - a subscrição do Azure que contém os recursos que estão a ser alterados.</span><span class="sxs-lookup"><span data-stu-id="b2972-113">A *Subscription* - The Azure Subscription containing the Resources being acted upon.</span></span>
- <span data-ttu-id="b2972-114">Um *Inquilino* - o inquilino do Azure Active Directory que contém a sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="b2972-114">A *Tenant* - The Azure Active Directory tenant that contains your subscription.</span></span> <span data-ttu-id="b2972-115">Os inquilinos são mais importantes para a autenticação do Principal de Serviço.</span><span class="sxs-lookup"><span data-stu-id="b2972-115">Tenants are more important to ServicePrincipal authentication.</span></span>
- <span data-ttu-id="b2972-116">Um *Ambiente* - a cloud de destino específica do Azure, normalmente, a Cloud global do Azure.</span><span class="sxs-lookup"><span data-stu-id="b2972-116">An *Environment* - The particular Azure Cloud being targeted, usually the Azure global Cloud.</span></span>
  <span data-ttu-id="b2972-117">No entanto, a definição do ambiente permite-lhe visar também uma cloud Nacional, do Government e no local (Azure Stack).</span><span class="sxs-lookup"><span data-stu-id="b2972-117">However, the environment setting allows you to target National, Government, and on-premises (Azure Stack) clouds as well.</span></span>
- <span data-ttu-id="b2972-118">*Credenciais* - as informações utilizadas pelo Azure para verificar a sua identidade e garantir a sua autorização para aceder a recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="b2972-118">*Credentials* - The information used by Azure to verify your identity and ensure your authorization to access resources in Azure</span></span>

<span data-ttu-id="b2972-119">Em versões anteriores, o Contexto do Azure tinha de ser criado sempre que abria uma nova sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-119">In previous releases, your Azure Context had to be created each time you opened a new PowerShell session.</span></span> <span data-ttu-id="b2972-120">A partir do Azure PowerShell v4.4.0, pode ativar a gravação e reutilização automáticas de Contextos do Azure sempre que abrir uma nova sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-120">Beginning with Azure PowerShell v4.4.0, you can enable the automatic saving and reuse of Azure Contexts whenever you open a new PowerShell session.</span></span>

## <a name="automatically-saving-the-context-for-the-next-sign-in"></a><span data-ttu-id="b2972-121">Guardar automaticamente o contexto para o próximo início de sessão</span><span class="sxs-lookup"><span data-stu-id="b2972-121">Automatically saving the context for the next sign in</span></span>

<span data-ttu-id="b2972-122">Por predefinição, o Azure PowerShell elimina as informações de contexto sempre que fecha a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-122">By default, Azure PowerShell discards your context information whenever you close the PowerShell session.</span></span>

<span data-ttu-id="b2972-123">Para permitir que o Azure PowerShell se lembre do contexto depois de fechar a sessão do PowerShell, utilize `Enable-AzureRmContextAutosave`.</span><span class="sxs-lookup"><span data-stu-id="b2972-123">To allow Azure PowerShell to remember your context after the PowerShell session is closed, use `Enable-AzureRmContextAutosave`.</span></span> <span data-ttu-id="b2972-124">As informações de contexto e as credenciais são guardadas automaticamente numa pasta oculta especial no seu diretório de utilizador (`%AppData%\Roaming\Windows Azure PowerShell`).</span><span class="sxs-lookup"><span data-stu-id="b2972-124">Context and credential information are automatically saved in a special hidden folder in your user directory (`%AppData%\Roaming\Windows Azure PowerShell`).</span></span>
<span data-ttu-id="b2972-125">Posteriormente, cada nova sessão do PowerShell visa o contexto utilizado na sua última sessão.</span><span class="sxs-lookup"><span data-stu-id="b2972-125">Subsequently, each new PowerShell session targets the context used in your last session.</span></span>

<span data-ttu-id="b2972-126">Para definir o PowerShell para que esqueça o contexto e as credenciais, utilize `Disable-AzureRmContextAutoSave`.</span><span class="sxs-lookup"><span data-stu-id="b2972-126">To set PowerShell to forget your context and credentials, use `Disable-AzureRmContextAutoSave`.</span></span> <span data-ttu-id="b2972-127">Terá de iniciar sessão no Azure sempre que abrir uma sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2972-127">You will need to sign in to Azure every time you open a PowerShell session.</span></span>

<span data-ttu-id="b2972-128">Os cmdlets que lhe permitem gerir contextos do Azure também permitem o controlo detalhado.</span><span class="sxs-lookup"><span data-stu-id="b2972-128">The cmdlets that allow you to manage Azure contexts also allow you fine grained control.</span></span> <span data-ttu-id="b2972-129">Se pretender que as alterações sejam aplicadas apenas à sessão atual do PowerShell (âmbito `Process`) ou a cada sessão do PowerShell (âmbito `CurrentUser`).</span><span class="sxs-lookup"><span data-stu-id="b2972-129">If you want changes to apply only to the current PowerShell session (`Process` scope) or every PowerShell session (`CurrentUser` scope).</span></span> <span data-ttu-id="b2972-130">Estas opções são abordadas detalhadamente em [Utilizar Âmbitos de Contexto](#using-context-scopes).</span><span class="sxs-lookup"><span data-stu-id="b2972-130">These options are discussed in mode detail in [Using Context Scopes](#using-context-scopes).</span></span>

## <a name="running-azure-powershell-cmdlets-as-background-jobs"></a><span data-ttu-id="b2972-131">Executar os cmdlets do Azure PowerShell como tarefas em segundo plano</span><span class="sxs-lookup"><span data-stu-id="b2972-131">Running Azure PowerShell cmdlets as background jobs</span></span>

<span data-ttu-id="b2972-132">A funcionalidade **Gravação Automática de Contexto do Azure** permite-lhe também partilhar o contexto com tarefas do PowerShell em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="b2972-132">The **Azure Context Autosave** feature also allows you to share you context with PowerShell background jobs.</span></span> <span data-ttu-id="b2972-133">O PowerShell permite-lhe iniciar e monitorizar tarefas de execução longa como tarefas em segundo plano, sem ter de aguardar a conclusão das tarefas.</span><span class="sxs-lookup"><span data-stu-id="b2972-133">PowerShell allows you to start and monitor long-executing tasks as background jobs without having to wait for the tasks to complete.</span></span> <span data-ttu-id="b2972-134">Pode partilhar as credenciais com tarefas em segundo plano de duas formas diferentes:</span><span class="sxs-lookup"><span data-stu-id="b2972-134">You can share credentials with background jobs in two different ways:</span></span>

- <span data-ttu-id="b2972-135">Passar o contexto como um argumento</span><span class="sxs-lookup"><span data-stu-id="b2972-135">Passing the context as an argument</span></span>

  <span data-ttu-id="b2972-136">A maioria dos cmdlets do AzureRM permitem-lhe passar o contexto como um parâmetro para o cmdlet.</span><span class="sxs-lookup"><span data-stu-id="b2972-136">Most AzureRM cmdlets allow you to pass the context as a parameter to the cmdlet.</span></span> <span data-ttu-id="b2972-137">Pode passar um contexto para uma tarefa em segundo plano, conforme mostrado no exemplo seguinte:</span><span class="sxs-lookup"><span data-stu-id="b2972-137">You can pass a context to a background job as shown in the following example:</span></span>

  ```powershell-interactive
  PS C:\> $job = Start-Job { param ($ctx) New-AzureRmVm -AzureRmContext $ctx [... Additional parameters ...]} -ArgumentList (Get-AzureRmContext)
  ```

- <span data-ttu-id="b2972-138">Utilizar o contexto predefinido com a Gravação Automática ativada</span><span class="sxs-lookup"><span data-stu-id="b2972-138">Using the default context with Autosave enabled</span></span>

  <span data-ttu-id="b2972-139">Se tiver ativado a **Gravação Automática de Contexto**, as tarefas em segundo plano utilizam automaticamente o contexto predefinido guardado.</span><span class="sxs-lookup"><span data-stu-id="b2972-139">If you have enabled **Context Autosave**, background jobs automatically use the default saved context.</span></span>

  ```powershell-interactive
  PS C:\> $job = Start-Job { New-AzureRmVm [... Additional parameters ...]}
  ```

<span data-ttu-id="b2972-140">Quando precisar de saber o resultado da tarefa em segundo plano, utilize `Get-Job` para verificar o estado da tarefa e `Wait-Job` para aguardar a conclusão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="b2972-140">When you need to know the outcome of the background task, use `Get-Job` to check the job status and `Wait-Job` to wait for the Job to complete.</span></span> <span data-ttu-id="b2972-141">Utilize `Receive-Job` para capturar ou apresentar o resultado da tarefa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="b2972-141">Use `Receive-Job` to capture or display the output of the background job.</span></span> <span data-ttu-id="b2972-142">Para obter mais informações, veja [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span><span class="sxs-lookup"><span data-stu-id="b2972-142">For more information, see [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="creating-selecting-renaming-and-removing-contexts"></a><span data-ttu-id="b2972-143">Criar, selecionar, mudar o nome e remover contextos</span><span class="sxs-lookup"><span data-stu-id="b2972-143">Creating, selecting, renaming, and removing contexts</span></span>

<span data-ttu-id="b2972-144">Para criar um contexto, tem de ter sessão iniciada no Azure.</span><span class="sxs-lookup"><span data-stu-id="b2972-144">To create a context, you must be signed in to Azure.</span></span> <span data-ttu-id="b2972-145">O cmdlet `Add-AzureRmAccount` (ou o respetivo alias, `Login-AzureRmAccount`) define o contexto predefinido utilizado por cmdlets subsequentes do Azure PowerShell e permite-lhe aceder a quaisquer inquilinos ou subscrições permitidos pelas suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="b2972-145">The `Add-AzureRmAccount` cmdlet (or its alias, `Login-AzureRmAccount`) sets the default context used by subsequent Azure PowerShell cmdlets, and allows you to access any tenants or subscriptions allowed by your credentials.</span></span>

<span data-ttu-id="b2972-146">Para adicionar um novo contexto após o início de sessão, utilize `Set-AzureRmContext` (ou o respetivo alias, `Select-AzureRmSubscription`).</span><span class="sxs-lookup"><span data-stu-id="b2972-146">To add a new context after sign in, use `Set-AzureRmContext` (or its alias, `Select-AzureRmSubscription`).</span></span>

```azurepowershell-interactive
PS C:\> Set-AzureRMContext -Subscription "Contoso Subscription 1" -Name "Contoso1"
```

<span data-ttu-id="b2972-147">O exemplo anterior adiciona um novo contexto que visa “Contoso Subscription 1”, com as suas credenciais atuais.</span><span class="sxs-lookup"><span data-stu-id="b2972-147">The previous example adds a new context targeting 'Contoso Subscription 1' using your current credentials.</span></span> <span data-ttu-id="b2972-148">O novo contexto tem o nome “Contoso1”.</span><span class="sxs-lookup"><span data-stu-id="b2972-148">The new context is named 'Contoso1'.</span></span> <span data-ttu-id="b2972-149">Se não fornecer um nome para o contexto, é utilizado um nome predefinido, com o ID da conta e o ID da subscrição.</span><span class="sxs-lookup"><span data-stu-id="b2972-149">If you do not provide a name for the context, a default name, using the account ID and subscription ID is used.</span></span>

<span data-ttu-id="b2972-150">Para mudar o nome de um contexto existente, utilize o cmdlet `Rename-AzureRmContext`.</span><span class="sxs-lookup"><span data-stu-id="b2972-150">To rename an existing context, use the `Rename-AzureRmContext` cmdlet.</span></span> <span data-ttu-id="b2972-151">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b2972-151">For example:</span></span>

```azurepowershell-interactive
PS C:\> Rename-AzureRmContext '[user1@contoso.org; 123456-7890-1234-564321]` 'Contoso2'
```

<span data-ttu-id="b2972-152">Este exemplo muda o nome do contexto com o nome automático `[user1@contoso.org; 123456-7890-1234-564321]` para o nome simples “Contoso2”.</span><span class="sxs-lookup"><span data-stu-id="b2972-152">This example renames the context with automatic name `[user1@contoso.org; 123456-7890-1234-564321]` to the simple name 'Contoso2'.</span></span> <span data-ttu-id="b2972-153">Os cmdlets que gerem contextos também utilizam a conclusão de tabulação, permitindo-lhe selecionar rapidamente o contexto.</span><span class="sxs-lookup"><span data-stu-id="b2972-153">Cmdlets that manage contexts also use tab completion, allowing you to quickly select the context.</span></span>

<span data-ttu-id="b2972-154">Por último, para remover um contexto, utilize o cmdlet `Remove-AzureRmContext`.</span><span class="sxs-lookup"><span data-stu-id="b2972-154">Finally, to remove a context, use the `Remove-AzureRmContext` cmdlet.</span></span>  <span data-ttu-id="b2972-155">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b2972-155">For example:</span></span>

```azurepowershell-interactive
PS C:\> Remove-AzureRmContext Contoso2
```

<span data-ttu-id="b2972-156">Esquece o contexto ao qual foi dado o nome “Contoso2”.</span><span class="sxs-lookup"><span data-stu-id="b2972-156">Forgets the context that was named 'Contoso2'.</span></span> <span data-ttu-id="b2972-157">Pode recriar este contexto posteriormente, com `Set-AzureRmContext`</span><span class="sxs-lookup"><span data-stu-id="b2972-157">You can recreate this context subsequently using `Set-AzureRmContext`</span></span>

## <a name="removing-credentials"></a><span data-ttu-id="b2972-158">Remover credenciais</span><span class="sxs-lookup"><span data-stu-id="b2972-158">Removing credentials</span></span>

<span data-ttu-id="b2972-159">Pode remover todas as credenciais e os contextos associados de um utilizador ou principal de serviço, com `Remove-AzureRmAccount` (também conhecido como `Logout-AzureRmAccount`).</span><span class="sxs-lookup"><span data-stu-id="b2972-159">You can remove all credentials and associated contexts for a user or service principal using `Remove-AzureRmAccount` (also known as `Logout-AzureRmAccount`).</span></span> <span data-ttu-id="b2972-160">Quando executado sem parâmetros, o cmdlet `Remove-AzureRmAccount` remove todas as credenciais e os contextos associados ao Utilizador ou Principal de Serviço no contexto atual.</span><span class="sxs-lookup"><span data-stu-id="b2972-160">When executed without parameters, the `Remove-AzureRmAccount` cmdlet removes all credentials and contexts associated with the User or Service Principal in the current context.</span></span> <span data-ttu-id="b2972-161">Pode passar um Nome de Utilizador, Nome do Principal de Serviço ou contexto para visar um determinado principal.</span><span class="sxs-lookup"><span data-stu-id="b2972-161">You may pass in a Username, Service Principal Name, or context to target a particular principal.</span></span>

```azurepowershell-interactive
Remove-AzureRmAccount user1@contoso.org
```

## <a name="using-context-scopes"></a><span data-ttu-id="b2972-162">Utilizar âmbitos de contexto</span><span class="sxs-lookup"><span data-stu-id="b2972-162">Using context scopes</span></span>

<span data-ttu-id="b2972-163">Ocasionalmente, poderá querer selecionar, alterar ou remover um contexto de uma sessão do PowerShell sem afetar outras sessões.</span><span class="sxs-lookup"><span data-stu-id="b2972-163">Occasionally, you may want to select, change, or remove a context in a PowerShell session without impacting other sessions.</span></span> <span data-ttu-id="b2972-164">Para alterar o comportamento predefinido de cmdlets de contexto, utilize o parâmetro `Scope`.</span><span class="sxs-lookup"><span data-stu-id="b2972-164">To change the default behavior of context cmdlets, use the `Scope` parameter.</span></span> <span data-ttu-id="b2972-165">O âmbito `Process` substitui o comportamento predefinido, fazendo-o aplicar-se só à sessão atual.</span><span class="sxs-lookup"><span data-stu-id="b2972-165">The `Process` scope overrides the default behavior by making it apply only for the current session.</span></span> <span data-ttu-id="b2972-166">Por outro lado, o âmbito `CurrentUser` altera o contexto em todas as sessões, em vez de apenas na sessão atual.</span><span class="sxs-lookup"><span data-stu-id="b2972-166">Conversely `CurrentUser` scope changes the context in all sessions, instead of just the current session.</span></span>

<span data-ttu-id="b2972-167">Por exemplo, para alterar o contexto predefinido na sessão atual do PowerShell sem causar impacto noutras janelas ou no contexto utilizado da próxima vez que abrir uma sessão, utilize:</span><span class="sxs-lookup"><span data-stu-id="b2972-167">As an example, to change the default context in the current PowerShell session without impacting other windows, or the context used the next time a session is opened, use:</span></span>

```azurepowershell-interactive
PS C:\> Select-AzureRmContext Contoso1 -Scope Process
```

## <a name="how-the-context-autosave-setting-is-remembered"></a><span data-ttu-id="b2972-168">Como a definição de gravação automática do contexto é memorizada</span><span class="sxs-lookup"><span data-stu-id="b2972-168">How the context autosave setting is remembered</span></span>

<span data-ttu-id="b2972-169">A definição de Gravação Automática do contexto é guardada no diretório do Azure PowerShell do utilizador (`%AppData%\Roaming\Windows Azure PowerShell`).</span><span class="sxs-lookup"><span data-stu-id="b2972-169">The context AutoSave setting is saved to the user Azure PowerShell directory (`%AppData%\Roaming\Windows Azure PowerShell`).</span></span> <span data-ttu-id="b2972-170">Alguns tipos de contas de computador podem não ter acesso a este diretório.</span><span class="sxs-lookup"><span data-stu-id="b2972-170">Some kinds of computer accounts may not have access to this directory.</span></span> <span data-ttu-id="b2972-171">Para estes cenários, pode utilizar a variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="b2972-171">For such scenarios, you can use the environment variable</span></span>

```azurepowershell-interactive
$env:AzureRmContextAutoSave="true" | "false"
```

<span data-ttu-id="b2972-172">Se definido para “true”, o contexto é guardado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b2972-172">If set to 'true', the context is automatically saved.</span></span> <span data-ttu-id="b2972-173">Se definido para “false”, o contexto não é guardado.</span><span class="sxs-lookup"><span data-stu-id="b2972-173">If set to 'false', the context is not saved.</span></span>

## <a name="changes-to-the-azurermprofile-module"></a><span data-ttu-id="b2972-174">Alterações ao módulo AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="b2972-174">Changes to the AzureRM.Profile module</span></span>

<span data-ttu-id="b2972-175">Novos cmdlets para gerir o contexto</span><span class="sxs-lookup"><span data-stu-id="b2972-175">New cmdlets for managing context</span></span>

- <span data-ttu-id="b2972-176">[Enable-AzureRmContextAutosave][enable] - permite guardar o contexto entre sessões do Powershell.</span><span class="sxs-lookup"><span data-stu-id="b2972-176">[Enable-AzureRmContextAutosave][enable] - Allow saving the context between powershell sessions.</span></span>
  <span data-ttu-id="b2972-177">Quaisquer alterações alteram o contexto global.</span><span class="sxs-lookup"><span data-stu-id="b2972-177">Any changes alter the global context.</span></span>
- <span data-ttu-id="b2972-178">[Disable-AzureRmContextAutosave][disable] - desativa a gravação automática do contexto.</span><span class="sxs-lookup"><span data-stu-id="b2972-178">[Disable-AzureRmContextAutosave][disable] - Turn off autosaving the context.</span></span> <span data-ttu-id="b2972-179">Em cada nova sessão do PowerShell, é pedido ao utilizador que inicie sessão novamente.</span><span class="sxs-lookup"><span data-stu-id="b2972-179">Each new PowerShell session is required to sign in again.</span></span>
- <span data-ttu-id="b2972-180">[Select-AzureRmContext][select] - seleciona um contexto como predefinição.</span><span class="sxs-lookup"><span data-stu-id="b2972-180">[Select-AzureRmContext][select] - Select a context as the default.</span></span> <span data-ttu-id="b2972-181">Todos os cmdlets subsequentes utilizam as credenciais neste contexto para a autenticação.</span><span class="sxs-lookup"><span data-stu-id="b2972-181">All subsequent cmdlets use the credentials in this context for authentication.</span></span>
- <span data-ttu-id="b2972-182">[Remove-AzureRmAccount][remove-cred] - remove todas as credenciais e os contextos associados a uma conta.</span><span class="sxs-lookup"><span data-stu-id="b2972-182">[Remove-AzureRmAccount][remove-cred] - Remove all credentials and contexts associated with an account.</span></span>
- <span data-ttu-id="b2972-183">[Remove-AzureRmContext][remove-context] - remove um contexto nomeado.</span><span class="sxs-lookup"><span data-stu-id="b2972-183">[Remove-AzureRmContext][remove-context] - Remove a named context.</span></span>
- <span data-ttu-id="b2972-184">[Rename-AzureRmContext][rename] - muda o nome de um contexto existente.</span><span class="sxs-lookup"><span data-stu-id="b2972-184">[Rename-AzureRmContext][rename] - Rename an existing context.</span></span>

<span data-ttu-id="b2972-185">Alterações aos cmdlets do perfil existente</span><span class="sxs-lookup"><span data-stu-id="b2972-185">Changes to existing profile cmdlets</span></span>

- <span data-ttu-id="b2972-186">[Add-AzureRmAccount][login] - permite o controlo do âmbito do início de sessão para o processo ou utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="b2972-186">[Add-AzureRmAccount][login] - Allow scoping of the sign in to the process or the current user.</span></span>
  <span data-ttu-id="b2972-187">Permitir nomear o contexto predefinido após a autenticação.</span><span class="sxs-lookup"><span data-stu-id="b2972-187">Allow naming the default context after authentication.</span></span>
- <span data-ttu-id="b2972-188">[Import-AzureRmContext][import] - permite o controlo do âmbito do início de sessão para o processo ou utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="b2972-188">[Import-AzureRmContext][import] - Allow scoping of the sign in to the process or the current user.</span></span>
- <span data-ttu-id="b2972-189">[Set-AzureRmContext][set-context] - permite a seleção de contextos nomeados existentes e alterações de âmbito no processo ou utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="b2972-189">[Set-AzureRmContext][set-context] - Allow selection of existing named contexts, and scope changes to the process or current user.</span></span>

<!-- Hyperlinks -->
[enable]: /powershell/module/azurerm.profile/Enable-AzureRmContextAutosave
[disable]: /powershell/module/azurerm.profile/Disable-AzureRmContextAutosave
[select]: /powershell/module/azurerm.profile/Select-AzureRmContext
[remove-cred]: /powershell/module/azurerm.profile/Remove-AzureRmAccount
[remove-context]: /powershell/module/azurerm.profile/Remove-AzureRmContext
[rename]: /powershell/module/azurerm.profile/Rename-AzureRmContext

<!-- Updated cmdlets -->
[login]: /powershell/module/azurerm.profile/Add-AzureRmAccount
[import]: /powershell/module/azurerm.profile/Import-AzureRmAccount
[set-context]: /powershell/module/azurerm.profile/Import-AzureRmContext
