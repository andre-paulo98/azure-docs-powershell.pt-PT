---
title: Introdução ao Azure PowerShell
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 01/17/2020
ms.openlocfilehash: 718f0dc0f1ef9b0c2aa3d0630ca099fa5cec7ec0
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477802"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="c0351-102">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0351-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="c0351-103">O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="c0351-103">Azure PowerShell is designed for managing and administering Azure resources from the command line.</span></span> <span data-ttu-id="c0351-104">Utilize o Azure PowerShell para criar ferramentas automatizadas que utilizem o modelo do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="c0351-104">Use Azure PowerShell when you want to build automated tools that use the Azure Resource Manager model.</span></span>
<span data-ttu-id="c0351-105">Experimente no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou instale-o no seu computador local.</span><span class="sxs-lookup"><span data-stu-id="c0351-105">Try it out in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or install on your local machine.</span></span>

<span data-ttu-id="c0351-106">Este artigo ajuda-o a começar a utilizar o Azure PowerShell e explica os principais conceitos que lhe estão subjacentes.</span><span class="sxs-lookup"><span data-stu-id="c0351-106">This article helps you get started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="c0351-107">Instalar ou executar no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c0351-107">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="c0351-108">A maneira mais fácil de começar a utilizar o Azure PowerShell é experimentá-lo num ambiente do Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c0351-108">The easiest way to get started with Azure PowerShell is by trying it out in an Azure Cloud Shell environment.</span></span>
<span data-ttu-id="c0351-109">Para ficar operacional com o Cloud Shell, veja [Início Rápido do PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="c0351-109">To get up and running with Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
<span data-ttu-id="c0351-110">O Cloud Shell executa o PowerShell 6 num contentor do Linux, pelo que a funcionalidade específica do Windows não está disponível.</span><span class="sxs-lookup"><span data-stu-id="c0351-110">Cloud Shell runs PowerShell 6 on a Linux container, so Windows-specific functionality isn't available.</span></span>

<span data-ttu-id="c0351-111">Quando estiver pronto para instalar o Azure PowerShell no seu computador local, siga as instruções em [Instalar o módulo do Azure PowerShell](install-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="c0351-111">When you're ready to install Azure PowerShell on your local machine, follow the instructions in [Install the Azure PowerShell module](install-az-ps.md).</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="c0351-112">Iniciar sessão no Azure</span><span class="sxs-lookup"><span data-stu-id="c0351-112">Sign in to Azure</span></span>

<span data-ttu-id="c0351-113">Inicie sessão interativamente com o cmdlet `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="c0351-113">Sign in interactively with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="c0351-114">Se utilizar o Cloud Shell, ignore este passo: a sua sessão do Azure Cloud Shell já foi autenticada para o ambiente, a subscrição e o inquilino que iniciou a sessão do Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c0351-114">Skip this step if you use Cloud Shell: Your Azure Cloud Shell session is already authenticated for the environment, subscription, and tenant that launched the Cloud Shell session.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="c0351-115">Se estiver numa região fora dos E.U.A., utilize o parâmetro `-Environment` para iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="c0351-115">If you're in a non-US region, use the `-Environment` parameter to sign in.</span></span> <span data-ttu-id="c0351-116">Obtenha o nome do ambiente para a sua região através do cmdlet [Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment).</span><span class="sxs-lookup"><span data-stu-id="c0351-116">Get the name of the environment for your region by using the [Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) cmdlet.</span></span> <span data-ttu-id="c0351-117">Por exemplo, para iniciar sessão no Azure China 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="c0351-117">For example, to sign in to Azure China 21Vianet:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="c0351-118">Nos ambientes do PowerShell 5.1, verá uma caixa de diálogo de início de sessão que lhe pedirá o nome de utilizador e a palavra-passe da sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0351-118">In PowerShell 5.1 environments, you'll get a sign-in dialog to provide a username and password for your Azure account.</span></span> <span data-ttu-id="c0351-119">Em todas as outras versões do PowerShell, obterá um token para utilizar em [https://microsoft.com/devicelogin ].</span><span class="sxs-lookup"><span data-stu-id="c0351-119">On every other version of PowerShell, you'll get a token to use on [https://microsoft.com/devicelogin].</span></span>
<span data-ttu-id="c0351-120">Abra esta página no seu browser e introduza o token, inicie sessão com as suas credenciais de conta do Azure e autorize o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c0351-120">Open this page in your browser and enter the token, then sign in with your Azure account credentials and authorize Azure PowerShell.</span></span>

<span data-ttu-id="c0351-121">Depois de iniciar sessão, são apresentadas informações que indicam qual das subscrições do Azure se encontra ativa.</span><span class="sxs-lookup"><span data-stu-id="c0351-121">After signing in, you'll see information indicating which of your Azure subscriptions is active.</span></span> <span data-ttu-id="c0351-122">Se tiver várias subscrições do Azure na sua conta e quiser selecionar uma diferente, obtenha as subscrições disponíveis com [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) e utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext) com o ID da subscrição.</span><span class="sxs-lookup"><span data-stu-id="c0351-122">If you have multiple Azure subscriptions in your account and want to select a different one, get your available subscriptions with [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) and use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet with your subscription ID.</span></span>
<span data-ttu-id="c0351-123">Para obter mais informações sobre como gerir as suas subscrições do Azure no Azure PowerShell, veja [Use multiple Azure subscriptions](manage-subscriptions-azureps.md) (Utilizar várias subscrições do Azure).</span><span class="sxs-lookup"><span data-stu-id="c0351-123">For more information about managing your Azure subscriptions in Azure PowerShell, see [Use multiple Azure subscriptions](manage-subscriptions-azureps.md).</span></span>

<span data-ttu-id="c0351-124">Assim que tiver iniciado sessão, utilize os cmdlets do Azure PowerShell para aceder e gerir recursos na sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="c0351-124">Once signed in, use the Azure PowerShell cmdlets to access and manage resources in your subscription.</span></span> <span data-ttu-id="c0351-125">Para saber mais sobre o processo de início de sessão e os métodos de autenticação, veja [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="c0351-125">To learn more about the sign-in process and authentication methods, see [Sign in with Azure PowerShell](authenticate-azureps.md).</span></span>

## <a name="find-commands"></a><span data-ttu-id="c0351-126">Encontrar comandos</span><span class="sxs-lookup"><span data-stu-id="c0351-126">Find commands</span></span>

<span data-ttu-id="c0351-127">Os cmdlets do Azure PowerShell seguem uma convenção de nomenclatura padrão para o PowerShell: `VERB-NOUN`.</span><span class="sxs-lookup"><span data-stu-id="c0351-127">Azure PowerShell cmdlets follow a standard naming convention for PowerShell, `VERB-NOUN`.</span></span> <span data-ttu-id="c0351-128">O verbo descreve a ação (os exemplos incluem `New`, `Get`, `Set`, `Remove`) e o substantivo descreve o tipo de recurso (os exemplos incluem `AzVM`, `AzKeyVaultCertificate`, `AzFirewall`, `AzVirtualNetworkGateway`).</span><span class="sxs-lookup"><span data-stu-id="c0351-128">The verb describes the action (examples include `New`, `Get`, `Set`, `Remove`) and the noun describes the resource type (examples include `AzVM`, `AzKeyVaultCertificate`, `AzFirewall`, `AzVirtualNetworkGateway`).</span></span> <span data-ttu-id="c0351-129">Os substantivos no Azure PowerShell começam sempre com o prefixo `Az`.</span><span class="sxs-lookup"><span data-stu-id="c0351-129">Nouns in Azure PowerShell always start with the prefix `Az`.</span></span> <span data-ttu-id="c0351-130">Para obter a lista completa dos verbos padrão, veja [Verbos aprovados para os Comandos do PowerShell](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands).</span><span class="sxs-lookup"><span data-stu-id="c0351-130">For the full list of standard verbs, see [Approved verbs for PowerShell Commands](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands).</span></span>

<span data-ttu-id="c0351-131">Saber os substantivos, verbos e módulos do Azure PowerShell disponíveis ajuda-o a encontrar os comandos com o cmdlet [Get-Command](/powershell/module/microsoft.powershell.core/get-command).</span><span class="sxs-lookup"><span data-stu-id="c0351-131">Knowing the nouns, verbs, and the Azure PowerShell modules available help you find commands with the [Get-Command](/powershell/module/microsoft.powershell.core/get-command) cmdlet.</span></span> <span data-ttu-id="c0351-132">Por exemplo, para encontrar todos os comandos relacionados com VMs que utilizem o verbo `Get`:</span><span class="sxs-lookup"><span data-stu-id="c0351-132">For example, to find all VM-related commands that use the `Get` verb:</span></span>

```powershell-interactive
Get-Command -Verb Get -Noun AzVM* -Module Az.Compute
```

<span data-ttu-id="c0351-133">Para o ajudar a encontrar os comandos comuns, esta tabela lista o tipo de recurso, o módulo correspondente do Azure PowerShell e o prefixo do substantivo a utilizar com `Get-Command`:</span><span class="sxs-lookup"><span data-stu-id="c0351-133">To help you find common commands, this table lists the resource type, corresponding Azure PowerShell module, and noun prefix to use with `Get-Command`:</span></span>

| <span data-ttu-id="c0351-134">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="c0351-134">Resource type</span></span> | <span data-ttu-id="c0351-135">Módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0351-135">Azure PowerShell module</span></span> | <span data-ttu-id="c0351-136">Prefixo do substantivo</span><span class="sxs-lookup"><span data-stu-id="c0351-136">Noun prefix</span></span> |
|---------------|-------------------------|----------------|
| [<span data-ttu-id="c0351-137">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="c0351-137">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="c0351-138">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0351-138">Az.Resources</span></span>](/powershell/module/az.resources#resources) | `AzResourceGroup` |
| [<span data-ttu-id="c0351-139">Máquinas virtuais</span><span class="sxs-lookup"><span data-stu-id="c0351-139">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="c0351-140">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0351-140">Az.Compute</span></span>](/powershell/module/az.compute#virtual_machines) | `AzVM` |
| [<span data-ttu-id="c0351-141">Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0351-141">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="c0351-142">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0351-142">Az.Storage</span></span>](/powershell/module/az.storage/) | `AzStorageAccount` |
| [<span data-ttu-id="c0351-143">Cofre de Chaves</span><span class="sxs-lookup"><span data-stu-id="c0351-143">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="c0351-144">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0351-144">Az.KeyVault</span></span>](/powershell/module/az.keyvault) | `AzKeyVault` |
| [<span data-ttu-id="c0351-145">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="c0351-145">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="c0351-146">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0351-146">Az.Websites</span></span>](/powershell/module/az.websites) | `AzWebApp` |
| [<span data-ttu-id="c0351-147">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="c0351-147">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="c0351-148">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0351-148">Az.Sql</span></span>](/powershell/module/az.sql) | `AzSqlDatabase` |

<span data-ttu-id="c0351-149">Para obter uma lista completa dos módulos no Azure PowerShell, veja a [lista de módulos do Azure PowerShell](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md) alojados no GitHub.</span><span class="sxs-lookup"><span data-stu-id="c0351-149">For a full list of the modules in Azure PowerShell, see the [Azure PowerShell modules list](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md) hosted on GitHub.</span></span>

## <a name="learn-azure-powershell-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="c0351-150">Aprender as noções básicas do Azure PowerShell com inícios rápidos e tutoriais</span><span class="sxs-lookup"><span data-stu-id="c0351-150">Learn Azure PowerShell basics with quickstarts and tutorials</span></span>

<span data-ttu-id="c0351-151">Para começar a utilizar o Azure PowerShell, experimente um tutorial aprofundado sobre como configurar máquinas virtuais e como as consultar.</span><span class="sxs-lookup"><span data-stu-id="c0351-151">To get started with Azure PowerShell, try an in-depth tutorial for setting up virtual machines and learning how to query them.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c0351-152">Criar máquinas virtuais com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0351-152">Create virtual machines with Azure PowerShell</span></span>](azureps-vm-tutorial.yml)

<span data-ttu-id="c0351-153">Também existem inícios rápidos do Azure PowerShell para outros serviços populares do Azure:</span><span class="sxs-lookup"><span data-stu-id="c0351-153">There are also Azure PowerShell quickstarts for other popular Azure services:</span></span>

* [<span data-ttu-id="c0351-154">Criar uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0351-154">Create a storage account</span></span>](/azure/storage/common/storage-quickstart-create-account?tabs=azure-powershell)
* [<span data-ttu-id="c0351-155">Transferir objetos de/para o armazenamento de Blobs do Azure</span><span class="sxs-lookup"><span data-stu-id="c0351-155">Transfer objects to/from Azure Blob storage</span></span>](/azure/storage/blobs/storage-quickstart-blobs-powershell)
* [<span data-ttu-id="c0351-156">Criar e obter segredos do Azure Key Vault</span><span class="sxs-lookup"><span data-stu-id="c0351-156">Create and retrieve secrets from Azure Key Vault</span></span>](/azure/key-vault/quick-create-powershell)
* [<span data-ttu-id="c0351-157">Criar uma firewall e base de dados SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="c0351-157">Create an Azure SQL database and firewall</span></span>](/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell)
* [<span data-ttu-id="c0351-158">Executar um contentor no Azure Container Instances</span><span class="sxs-lookup"><span data-stu-id="c0351-158">Run a container in Azure Container Instances</span></span>](/azure/container-instances/container-instances-quickstart-powershell)
* [<span data-ttu-id="c0351-159">Criar um Conjunto de Dimensionamento de Máquinas Virtuais (VMSS)</span><span class="sxs-lookup"><span data-stu-id="c0351-159">Create a Virtual Machine Scale Set (VMSS)</span></span>](/azure/virtual-machine-scale-sets/quick-create-powershell)
* [<span data-ttu-id="c0351-160">Criar um balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="c0351-160">Create a standard load balancer</span></span>](/azure/load-balancer/quickstart-create-standard-load-balancer-powershell)

## <a name="next-steps"></a><span data-ttu-id="c0351-161">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="c0351-161">Next steps</span></span>

* [<span data-ttu-id="c0351-162">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0351-162">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="c0351-163">Gerir subscrições do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0351-163">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="c0351-164">Criar principais de serviço com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0351-164">Create service principals with Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="c0351-165">Obter ajuda da comunidade:</span><span class="sxs-lookup"><span data-stu-id="c0351-165">Get help from the community:</span></span>
  * [<span data-ttu-id="c0351-166">Fórum do Azure no MSDN</span><span class="sxs-lookup"><span data-stu-id="c0351-166">Azure forum on MSDN</span></span>](https://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="c0351-167">Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="c0351-167">Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkId=320213)