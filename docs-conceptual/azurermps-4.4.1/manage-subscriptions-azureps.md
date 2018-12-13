---
title: Gerir subscrições do Azure com o Azure PowerShell | Microsoft Docs
description: Gerir subscrições do Azure com o Azure PowerShell
keywords: Azure PowerShell, subscrição
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 12e304f32f585c1af40d20579cd46999e0a12395
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217189"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="46569-104">Gerir várias subscrições do Azure</span><span class="sxs-lookup"><span data-stu-id="46569-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="46569-105">Se só agora começou a utilizar o Azure, é provável que só tenha uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="46569-105">If you are brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="46569-106">Mas se já o utilizar há algum tempo, poderá ter criado várias subscrições do Azure.</span><span class="sxs-lookup"><span data-stu-id="46569-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="46569-107">Pode configurar Azure PowerShell para executar comandos numa determinada subscrição.</span><span class="sxs-lookup"><span data-stu-id="46569-107">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="46569-108">Obtenha uma lista de todas as subscrições da sua conta.</span><span class="sxs-lookup"><span data-stu-id="46569-108">Get a list of all subscriptions in your account.</span></span>

    ```powershell-interactive
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

2. <span data-ttu-id="46569-109">Defina a predefinida.</span><span class="sxs-lookup"><span data-stu-id="46569-109">Set the default.</span></span>

    ```powershell-interactive
    Select-AzureRmSubscription -SubscriptionName "My Demos"
    ```

3. <span data-ttu-id="46569-110">Verifique a alteração executando o cmdlet `Get-AzureRmContext`.</span><span class="sxs-lookup"><span data-stu-id="46569-110">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

    ```powershell-interactive
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

<span data-ttu-id="46569-111">Depois de definir a subscrição predefinida, todos os comandos do Azure PowerShell subsequentes são executados no âmbito dessa subscrição.</span><span class="sxs-lookup"><span data-stu-id="46569-111">Once you set your default subscription, all subsequent Azure PowerShell commands run against this subscription.</span></span>
