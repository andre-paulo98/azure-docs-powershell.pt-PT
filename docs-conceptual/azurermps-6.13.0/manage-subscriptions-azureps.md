---
title: Gerir subscrições do Azure com o Azure PowerShell
description: Gerir subscrições do Azure com o Azure PowerShell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 9721baff069d2255481a3c993e82db49ba36d9ac
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83387909"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="d49ca-103">Gerir várias subscrições do Azure</span><span class="sxs-lookup"><span data-stu-id="d49ca-103">Manage multiple Azure subscriptions</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="d49ca-104">Se só agora começou a utilizar o Azure, é provável que só tenha uma subscrição individual.</span><span class="sxs-lookup"><span data-stu-id="d49ca-104">If you're brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="d49ca-105">Mas se já o utilizar há algum tempo, poderá ter criado várias subscrições do Azure.</span><span class="sxs-lookup"><span data-stu-id="d49ca-105">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="d49ca-106">Pode configurar Azure PowerShell para executar comandos numa determinada subscrição.</span><span class="sxs-lookup"><span data-stu-id="d49ca-106">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="d49ca-107">Obtenha uma lista de todas as subscrições da sua conta.</span><span class="sxs-lookup"><span data-stu-id="d49ca-107">Get a list of all subscriptions in your account.</span></span>

    ```azurepowershell-interactive
    Get-AzureRmSubscription
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My DevTest Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

2. <span data-ttu-id="d49ca-108">Defina a predefinida.</span><span class="sxs-lookup"><span data-stu-id="d49ca-108">Set the default.</span></span>

    ```azurepowershell-interactive
    Select-AzureRmSubscription -Subscription "My Demos"
    ```

3. <span data-ttu-id="d49ca-109">Verifique a alteração executando o cmdlet `Get-AzureRmContext`.</span><span class="sxs-lookup"><span data-stu-id="d49ca-109">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

    ```azurepowershell-interactive
    Get-AzureRmContext
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

<span data-ttu-id="d49ca-110">Depois de definir a subscrição predefinida, todos os comandos do Azure PowerShell são executados no âmbito dessa subscrição.</span><span class="sxs-lookup"><span data-stu-id="d49ca-110">Once you set your default subscription, all Azure PowerShell commands run against this subscription.</span></span>
