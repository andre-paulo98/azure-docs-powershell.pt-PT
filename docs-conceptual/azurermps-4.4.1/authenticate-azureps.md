---
title: "Iniciar sessão com o Azure PowerShell"
description: "Iniciar sessão com o Azure PowerShell"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 1af5aeffb8e87e916df3e2440a84805935136c0f
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2017
---
# <a name="log-in-with-azure-powershell"></a><span data-ttu-id="5b946-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5b946-103">Log in with Azure PowerShell</span></span>

<span data-ttu-id="5b946-104">O Azure PowerShell suporta vários métodos de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="5b946-104">Azure PowerShell supports multiple login methods.</span></span> <span data-ttu-id="5b946-105">A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="5b946-105">The simplest way to get started is to log in interactively at the command line.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="5b946-106">Início de sessão interativo</span><span class="sxs-lookup"><span data-stu-id="5b946-106">Interactive log in</span></span>

1. <span data-ttu-id="5b946-107">Digite `Login-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="5b946-107">Type `Login-AzureRmAccount`.</span></span> <span data-ttu-id="5b946-108">Obterá uma caixa de diálogo a solicitar as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="5b946-108">You will get dialog box asking for your Azure credentials.</span></span>

2. <span data-ttu-id="5b946-109">Escreva o endereço de e-mail e a palavra-passe associados à sua conta.</span><span class="sxs-lookup"><span data-stu-id="5b946-109">Type the email address and password associated with your account.</span></span> <span data-ttu-id="5b946-110">O Azure autentica e guarda as informações das credenciais e, em seguida, fecha a janela.</span><span class="sxs-lookup"><span data-stu-id="5b946-110">Azure authenticates and saves the credential information, and then closes the window.</span></span>

## <a name="log-in-with-a-service-principal"></a><span data-ttu-id="5b946-111">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="5b946-111">Log in with a service principal</span></span>

<span data-ttu-id="5b946-112">Os principais de serviço proporcionam uma forma de criar contas não interativas que pode ser utilizar para manipular recursos.</span><span class="sxs-lookup"><span data-stu-id="5b946-112">Service principals provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="5b946-113">Os principais de serviço são como contas de utilizador às quais pode aplicar regras com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b946-113">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span> <span data-ttu-id="5b946-114">Ao conceder as permissões mínimas necessárias para um principal de serviço, pode garantir que os seus scripts de automatização estão ainda mais protegidos.</span><span class="sxs-lookup"><span data-stu-id="5b946-114">By granting the minimum permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

1. <span data-ttu-id="5b946-115">Se ainda não tiver um principal de serviço, [crie-o](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="5b946-115">If you don't already have a service principal, [create one](create-azure-service-principal-azureps.md).</span></span>

2. <span data-ttu-id="5b946-116">Inicie sessão com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="5b946-116">Log in with the service principal.</span></span>

    ```powershell
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    <span data-ttu-id="5b946-117">Para obter o seu T, inicie sessão interativamente e obtenha o TenantId da sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="5b946-117">To get your TenantId, log in interactively and then get the TenantId from your subscription.</span></span>

    ```powershell
    Get-AzureRmSubscription
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :
    ```

### <a name="log-in-using-an-azure-vm-managed-service-identity"></a><span data-ttu-id="5b946-118">Iniciar sessão com uma Identidade do Serviço Gerido de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="5b946-118">Log in using an Azure VM Managed Service Identity</span></span>

<span data-ttu-id="5b946-119">Identidade do Serviço Gerido (MSI) é uma funcionalidade de pré-visualização do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b946-119">Managed Service Identity (MSI) is a preview feature of Azure Active Directory.</span></span> <span data-ttu-id="5b946-120">Pode utilizar um principal de serviço do MSI para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="5b946-120">You can use an MSI service principal for sign-in, and acquire an app-only access token to access other resources.</span></span>

<span data-ttu-id="5b946-121">Para obter mais informações sobre o MSI, veja [Como utilizar uma Identidade do Serviço Gerido de VM (MSI) do Azure para início de sessão e aquisição de token](/azure/active-directory/msi-how-to-get-access-token-using-msi).</span><span class="sxs-lookup"><span data-stu-id="5b946-121">For more information about MSI, see [How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition](/azure/active-directory/msi-how-to-get-access-token-using-msi).</span></span>

## <a name="log-in-to-another-cloud"></a><span data-ttu-id="5b946-122">Inicie sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="5b946-122">Log in to another Cloud</span></span>

<span data-ttu-id="5b946-123">Os serviços cloud do Azure fornecem diferentes ambientes que aderem aos regulamentos de processamento de dados de várias administrações públicas.</span><span class="sxs-lookup"><span data-stu-id="5b946-123">Azure cloud services provide different environments that adhere to the data-handling regulations of various governments.</span></span> <span data-ttu-id="5b946-124">Se a sua conta do Azure é de uma das clouds de administração pública, tem de especificar o ambiente quando iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="5b946-124">If your Azure account is in one the government clouds, you need to specify the environment when you sign in.</span></span> <span data-ttu-id="5b946-125">Por exemplo, se a sua conta está na cloud da China, inicia sessão com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="5b946-125">For example, if you account is in the China cloud you sign on using the following command:</span></span>

```powershell
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

<span data-ttu-id="5b946-126">Utilize o seguinte comando para obter uma lista de ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="5b946-126">Use the following command to get a list of available environments:</span></span>

```powershell
Get-AzureRmEnvironment | Select-Object Name
```

```
Name
----
AzureCloud
AzureChinaCloud
AzureUSGovernment
AzureGermanCloud
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="5b946-127">Saiba mais sobre como gerir o acesso baseado em funções do Azure</span><span class="sxs-lookup"><span data-stu-id="5b946-127">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="5b946-128">Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).</span><span class="sxs-lookup"><span data-stu-id="5b946-128">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="5b946-129">Cmdlets do Azure PowerShell para gestão de funções</span><span class="sxs-lookup"><span data-stu-id="5b946-129">Azure PowerShell cmdlets for role management</span></span>

* [<span data-ttu-id="5b946-130">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5b946-130">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="5b946-131">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5b946-131">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="5b946-132">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5b946-132">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="5b946-133">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5b946-133">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="5b946-134">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5b946-134">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="5b946-135">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5b946-135">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="5b946-136">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5b946-136">Set-AzureRmRoleDefinition</span></span>](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
