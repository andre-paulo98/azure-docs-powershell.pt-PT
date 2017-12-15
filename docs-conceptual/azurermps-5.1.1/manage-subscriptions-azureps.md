---
title: "Gerir subscrições do Azure com o Azure PowerShell | Microsoft Docs"
description: "Gerir subscrições do Azure com o Azure PowerShell"
keywords: "Azure PowerShell, subscrição"
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 68d03ec8d1a86fb3b270d02a4697bbf9af847f2d
ms.sourcegitcommit: c42c7176276ec4e1cc3360a93e6b15d32083bf9f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/14/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="c786e-104">Gerir várias subscrições do Azure</span><span class="sxs-lookup"><span data-stu-id="c786e-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="c786e-105">Se só agora começou a utilizar o Azure, é provável que só tenha uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="c786e-105">If you are brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="c786e-106">Mas se já o utilizar há algum tempo, poderá ter criado várias subscrições do Azure.</span><span class="sxs-lookup"><span data-stu-id="c786e-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="c786e-107">Pode configurar Azure PowerShell para executar comandos numa determinada subscrição.</span><span class="sxs-lookup"><span data-stu-id="c786e-107">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="c786e-108">Obtenha uma lista de todas as subscrições da sua conta.</span><span class="sxs-lookup"><span data-stu-id="c786e-108">Get a list of all subscriptions in your account.</span></span>

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

2. <span data-ttu-id="c786e-109">Defina a predefinida.</span><span class="sxs-lookup"><span data-stu-id="c786e-109">Set the default.</span></span>

    ```powershell
    Select-AzureRmSubscription -SubscriptionName "My Demos"
    ```

3. <span data-ttu-id="c786e-110">Verifique a alteração executando o cmdlet `Get-AzureRmContext`.</span><span class="sxs-lookup"><span data-stu-id="c786e-110">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

    ```powershell
    Get-AzureRmContext
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

<span data-ttu-id="c786e-111">Depois de definir a subscrição predefinida, todos os comandos do Azure PowerShell subsequentes são executados no âmbito dessa subscrição.</span><span class="sxs-lookup"><span data-stu-id="c786e-111">Once you set your default subscription, all subsequent Azure PowerShell commands run against this subscription.</span></span>
