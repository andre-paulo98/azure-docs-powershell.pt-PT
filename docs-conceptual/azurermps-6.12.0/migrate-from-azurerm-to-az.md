---
title: Migrar scripts do Azure PowerShell do AzureRM para o Az
description: Conheça os passos e as ferramentas para migrar scripts do módulo do AzureRM para o novo módulo do Az.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 0c73e7ac1d47a2a97b6136fa481d0adce8de33db
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574418"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="9bdfe-103">Migrar do AzureRM para o Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="9bdfe-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="9bdfe-104">O módulo do Az tem paridade de funcionalidades com o AzureRM, mas utiliza nomes de cmdlet mais curtos e mais consistentes.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="9bdfe-105">Os scripts escritos para os cmdlets do AzureRM não irão funcionar automaticamente com o módulo novo.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="9bdfe-106">Para facilitar a transição, o Az oferece ferramentas para permitir a execução dos seus scripts existentes com o AzureRM.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="9bdfe-107">Uma migração para um novo conjunto de comandos nunca é conveniente, mas este artigo ajuda-o a fazer a transição para o novo módulo.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="9bdfe-108">Certifique-se de que os seus scripts existentes funcionam com a versão mais recente do AzureRM</span><span class="sxs-lookup"><span data-stu-id="9bdfe-108">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="9bdfe-109">Este é o passo mais importante!</span><span class="sxs-lookup"><span data-stu-id="9bdfe-109">This is the most important step!</span></span> <span data-ttu-id="9bdfe-110">Execute os seus scripts existentes e certifique-se de que funcionam com a versão _mais recente_ do AzureRM (__6.12.0__).</span><span class="sxs-lookup"><span data-stu-id="9bdfe-110">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.12.0__).</span></span> <span data-ttu-id="9bdfe-111">Se os scripts não funcionarem, certifique-se de que lê o [guia de migração do AzureRM](migration-guide.6.0.0.md).</span><span class="sxs-lookup"><span data-stu-id="9bdfe-111">If your scripts don't work, make sure to read the [AzureRM migration guide](migration-guide.6.0.0.md).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="9bdfe-112">Instalar o módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="9bdfe-112">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="9bdfe-113">O primeiro passo é instalar o módulo do Az na sua plataforma.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-113">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="9bdfe-114">Para instalar o Az, precisa de desinstalar o AzureRM.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-114">To install Az, you need to uninstall AzureRM.</span></span>
<span data-ttu-id="9bdfe-115">Nos passos seguintes, irá aprender como continuar a executar os scripts existentes e permitir a compatibilidade dos nomes de cmdlet antigos.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-115">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="9bdfe-116">Para instalar o módulo do Azure PowerShell Az, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="9bdfe-116">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="9bdfe-117">[Desinstalar o módulo do AzureRM](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="9bdfe-117">[Uninstall the AzureRM module](uninstall-azurerm-ps.md).</span></span> <span data-ttu-id="9bdfe-118">Certifique-se de que remove _todas_ as versões instaladas do AzureRM, e não apenas a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-118">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="9bdfe-119">Instalar o módulo do Az</span><span class="sxs-lookup"><span data-stu-id="9bdfe-119">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><span data-ttu-id="9bdfe-120"><a name="aliases"/>Ativar o modo de alias do AzureRM</span><span class="sxs-lookup"><span data-stu-id="9bdfe-120"><a name="aliases"/>Enable AzureRM alias mode</span></span>

<span data-ttu-id="9bdfe-121">Com o AzureRM desinstalado e os seus scripts a funcionarem com a versão mais recente do AzureRM, chegou o momento de ativar o modo de compatibilidade para o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-121">With AzureRM uninstalled and your scripts working with the latest AzureRM version, now is the time to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="9bdfe-122">A compatibilidade é ativada com o comando:</span><span class="sxs-lookup"><span data-stu-id="9bdfe-122">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="9bdfe-123">Os aliases ativam a capacidade de utilizar nomes de cmdlet antigos com o módulo `Az` instalado.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-123">Aliases enable the ability to use old cmdlet names with the `Az` module installed.</span></span> <span data-ttu-id="9bdfe-124">Estes aliases são escritos para o perfil de utilizador do âmbito selecionado.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-124">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="9bdfe-125">Se não existir um perfil de utilizador, é criado um.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-125">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="9bdfe-126">Pode utilizar um `-Scope` diferente para este comando, mas não é recomendado!</span><span class="sxs-lookup"><span data-stu-id="9bdfe-126">You can use a different `-Scope` for this command, but it's not recommended!</span></span> <span data-ttu-id="9bdfe-127">Os aliases são escritos para o perfil de utilizador para o âmbito selecionado, por isso continue a permitir que tenham um âmbito o mais limitado possível.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-127">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="9bdfe-128">Ativar aliases em todo o sistema também pode causar problemas para outros utilizadores que têm o `AzureRM` instalado no seu âmbito local.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-128">Enabling aliases system-wide could also cause issues for other users which have `AzureRM` installed in their local scope.</span></span>

<span data-ttu-id="9bdfe-129">Assim que o modo de alias estiver ativado, execute os seus scripts novamente para confirmar que ainda funcionam como esperado.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-129">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="9bdfe-130">Alterar importações de módulo e nomes de cmdlet</span><span class="sxs-lookup"><span data-stu-id="9bdfe-130">Change module imports and cmdlet names</span></span>

<span data-ttu-id="9bdfe-131">Em geral, os nomes dos módulos foram alterados para que `AzureRM` e `Azure` se tornassem `Az`, e o mesmo para os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-131">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="9bdfe-132">Por exemplo, o módulo `AzureRM.Compute` foi renomeado para `Az.Compute`.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-132">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="9bdfe-133">`New-AzureRmVM` tornou-se `New-AzVM`, e `Get-AzureStorageBlob` é agora `Get-AzStorageBlob`.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-133">`New-AzureRmVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="9bdfe-134">Existem exceções a esta alteração de nomenclatura que deve ter conhecimento antes de fazer qualquer mudança de nome:</span><span class="sxs-lookup"><span data-stu-id="9bdfe-134">There are exceptions to this naming change that you should be aware of before doing any renaming:</span></span>

| <span data-ttu-id="9bdfe-135">Módulo do AzureRM</span><span class="sxs-lookup"><span data-stu-id="9bdfe-135">AzureRM module</span></span> | <span data-ttu-id="9bdfe-136">Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="9bdfe-136">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="9bdfe-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="9bdfe-137">AzureRM.DataFactories</span></span> | <span data-ttu-id="9bdfe-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9bdfe-138">Az.DataFactory</span></span> |
| <span data-ttu-id="9bdfe-139">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9bdfe-139">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="9bdfe-140">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9bdfe-140">Az.DataFactory</span></span> |
| <span data-ttu-id="9bdfe-141">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9bdfe-141">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="9bdfe-142">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bdfe-142">Az.RecoveryServices</span></span> |
| <span data-ttu-id="9bdfe-143">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9bdfe-143">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="9bdfe-144">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bdfe-144">Az.RecoveryServices</span></span> |

## <a name="summary"></a><span data-ttu-id="9bdfe-145">Resumo</span><span class="sxs-lookup"><span data-stu-id="9bdfe-145">Summary</span></span>

<span data-ttu-id="9bdfe-146">Ao seguir estes passos, pode atualizar todos os scripts existentes para utilizarem o módulo novo.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-146">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="9bdfe-147">Se tiver dúvidas ou problemas com estes passos que dificultaram a sua migração, comente este artigo para que possamos melhorar as instruções.</span><span class="sxs-lookup"><span data-stu-id="9bdfe-147">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>