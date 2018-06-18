---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com o MSI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: e2eb6767d16dd15529b35b7a4134f4dcdd257d60
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323344"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="0fd18-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="0fd18-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="0fd18-104">O Azure PowerShell suporta vários métodos de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="0fd18-104">Azure PowerShell supports multiple login methods.</span></span> <span data-ttu-id="0fd18-105">A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="0fd18-105">The simplest way to get started is to log in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="0fd18-106">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="0fd18-106">Sign in interactively</span></span>

<span data-ttu-id="0fd18-107">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount).</span><span class="sxs-lookup"><span data-stu-id="0fd18-107">To sign in interactively, use the [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) cmdlet.</span></span>

```azurepowershell
Connect-AzureRmAccount
```

<span data-ttu-id="0fd18-108">Quando é executado, este cmdlet apresenta uma caixa de diálogo que lhe pede para indicar o endereço de e-mail e a palavra-passe associados à sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="0fd18-108">When run, this cmdlet will bring up a dialog box prompting you for your email address and password associated with your Azure account.</span></span> <span data-ttu-id="0fd18-109">Quando efetuar a autenticação, essas informações são guardadas para a sessão atual do PowerShell, a caixa de diálogo é fechada e tem acesso a todos os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0fd18-109">When you authenticate, that information is saved for the current PowerShell session, the dialog is closed, and you have access to all of the Azure PowerShell cmdlets.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0fd18-110">Este início de sessão reporta à sessão atual do PowerShell _apenas_.</span><span class="sxs-lookup"><span data-stu-id="0fd18-110">This sign in is for the current PowerShell session _only_.</span></span> <span data-ttu-id="0fd18-111">Para manter o início de sessão em várias sessões, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="0fd18-111">To persist the login across multiple sessions, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="0fd18-112">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="0fd18-112">Sign in with a service principal</span></span>

<span data-ttu-id="0fd18-113">Os principais de serviço proporcionam uma forma de criar contas não interativas que pode ser utilizar para manipular recursos.</span><span class="sxs-lookup"><span data-stu-id="0fd18-113">Service principals provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="0fd18-114">Os principais de serviço são como contas de utilizador às quais pode aplicar regras com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fd18-114">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span> <span data-ttu-id="0fd18-115">Ao conceder as permissões mínimas necessárias para um principal de serviço, pode garantir que os seus scripts de automatização estão ainda mais protegidos.</span><span class="sxs-lookup"><span data-stu-id="0fd18-115">By granting the minimum permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

<span data-ttu-id="0fd18-116">Se precisar de criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="0fd18-116">If you need to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="0fd18-117">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="0fd18-117">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzureRmAccount` cmdlet.</span></span> <span data-ttu-id="0fd18-118">Também irá precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="0fd18-118">You will also need the service princpal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="0fd18-119">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="0fd18-119">In order to get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="0fd18-120">Este cmdlet irá apresentar uma caixa de diálogo para introduzir o ID de utilizador e a palavra-passe do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="0fd18-120">This cmdlet will display a dialog box to enter the service principal user ID and password into.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-vm-managed-service-identity"></a><span data-ttu-id="0fd18-121">Iniciar sessão com uma Identidade de Serviço Gerida de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="0fd18-121">Sign in using an Azure VM Managed Service Identity</span></span>

<span data-ttu-id="0fd18-122">Identidade do Serviço Gerido (MSI) é uma funcionalidade de pré-visualização do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fd18-122">Managed Service Identity (MSI) is a preview feature of Azure Active Directory.</span></span> <span data-ttu-id="0fd18-123">Pode utilizar um principal de serviço do MSI para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="0fd18-123">You can use an MSI service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="0fd18-124">O MSI só está disponível em máquinas virtuais em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="0fd18-124">MSI is only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="0fd18-125">Para obter mais informações sobre o MSI, veja [Como utilizar uma Identidade do Serviço Gerido de VM (MSI) do Azure para início de sessão e aquisição de token](/azure/active-directory/msi-how-to-get-access-token-using-msi).</span><span class="sxs-lookup"><span data-stu-id="0fd18-125">For more information about MSI, see [How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition](/azure/active-directory/msi-how-to-get-access-token-using-msi).</span></span>

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="0fd18-126">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="0fd18-126">Sign in to another Cloud</span></span>

<span data-ttu-id="0fd18-127">Os serviços cloud do Azure fornecem diferentes ambientes que cumprem os regulamentos de processamento de dados de várias regiões.</span><span class="sxs-lookup"><span data-stu-id="0fd18-127">Azure cloud services provide different environments that adhere to the data-handling regulations of various regions.</span></span> <span data-ttu-id="0fd18-128">Se a sua conta do Azure estiver numa cloud associada a uma destas regiões, terá de especificar o ambiente quando iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="0fd18-128">If your Azure account is in a cloud associated with one of these regions, you need to specify the environment when you sign in.</span></span> <span data-ttu-id="0fd18-129">Por exemplo, se a sua conta está na cloud da China, inicia sessão com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="0fd18-129">For example, if you account is in the China cloud you sign on using the following command:</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

<span data-ttu-id="0fd18-130">Utilize o seguinte comando para obter uma lista de ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="0fd18-130">Use the following command to get a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="0fd18-131">Saiba mais sobre como gerir o acesso baseado em funções do Azure</span><span class="sxs-lookup"><span data-stu-id="0fd18-131">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="0fd18-132">Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).</span><span class="sxs-lookup"><span data-stu-id="0fd18-132">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="0fd18-133">Cmdlets do Azure PowerShell para a gestão de funções:</span><span class="sxs-lookup"><span data-stu-id="0fd18-133">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="0fd18-134">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0fd18-134">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="0fd18-135">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0fd18-135">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="0fd18-136">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0fd18-136">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="0fd18-137">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0fd18-137">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="0fd18-138">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0fd18-138">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="0fd18-139">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0fd18-139">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="0fd18-140">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0fd18-140">Set-AzureRmRoleDefinition</span></span>](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
