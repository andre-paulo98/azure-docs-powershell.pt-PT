---
title: Todas as alterações do AzureRM para o Azure PowerShell Az 1.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 1.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2019
ms.openlocfilehash: 04c520a3171d0b06ceaaa96f1c77bda6b03952ae
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365720"
---
# <a name="breaking-changes-for-az-100"></a><span data-ttu-id="9881c-103">Alterações interruptivas do Az 1.0.0</span><span class="sxs-lookup"><span data-stu-id="9881c-103">Breaking changes for Az 1.0.0</span></span>

<span data-ttu-id="9881c-104">Este documento fornece informações detalhadas sobre as alterações entre o AzureRM 6.x e o novo módulo do Az, versão 1.x e posterior.</span><span class="sxs-lookup"><span data-stu-id="9881c-104">This document provides detailed information on the changes between AzureRM 6.x and the new Az module, version 1.x and later.</span></span> <span data-ttu-id="9881c-105">O índice irá guiá-lo através de um caminho de migração completo, incluindo alterações específicas do módulo que podem afetar os scripts.</span><span class="sxs-lookup"><span data-stu-id="9881c-105">The table of contents will help guide you through a full migration path, including module-specific changes that may affect your scripts.</span></span>

<span data-ttu-id="9881c-106">Para obter orientação geral sobre como começar uma migração do AzureRM para o Az, veja [Iniciar a migração do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="9881c-106">For general advice on getting started with a migration from AzureRM to Az, see [Start migration from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="9881c-107">Índice</span><span class="sxs-lookup"><span data-stu-id="9881c-107">Table of Contents</span></span>

- [<span data-ttu-id="9881c-108">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="9881c-108">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="9881c-109">Alterações dos prefixo de nomes de cmdlets</span><span class="sxs-lookup"><span data-stu-id="9881c-109">Cmdlet noun prefix changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="9881c-110">Alterações de Nomes de Módulos</span><span class="sxs-lookup"><span data-stu-id="9881c-110">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="9881c-111">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="9881c-111">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="9881c-112">Windows PowerShell 5.1 e .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="9881c-112">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="9881c-113">Remoção temporária do início de sessão do utilizador através de PSCredential</span><span class="sxs-lookup"><span data-stu-id="9881c-113">Temporary removal of user login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="9881c-114">Início de sessão com o código de dispositivo predefinido em vez da linha de comandos do browser</span><span class="sxs-lookup"><span data-stu-id="9881c-114">Default device code login instead of web browser prompt</span></span>](#default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="9881c-115">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="9881c-115">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="9881c-116">Az.ApiManagement (anteriormente AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="9881c-116">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="9881c-117">Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="9881c-117">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="9881c-118">Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="9881c-118">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="9881c-119">Az.Compute (anteriormente AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="9881c-119">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="9881c-120">Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="9881c-120">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="9881c-121">Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="9881c-121">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="9881c-122">Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="9881c-122">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="9881c-123">Az.KeyVault (anteriormente AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="9881c-123">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="9881c-124">Az.Media (anteriormente AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="9881c-124">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="9881c-125">Az.Monitor (anteriormente AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="9881c-125">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="9881c-126">Az.Network (anteriormente AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="9881c-126">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="9881c-127">Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="9881c-127">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="9881c-128">Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="9881c-128">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="9881c-129">Az.Resources (anteriormente AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="9881c-129">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="9881c-130">Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="9881c-130">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="9881c-131">Az.Sql (anteriormente AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="9881c-131">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="9881c-132">Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="9881c-132">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="9881c-133">Az.Websites (anteriormente AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="9881c-133">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="9881c-134">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="9881c-134">General breaking changes</span></span>

<span data-ttu-id="9881c-135">Esta secção fornece detalhes sobre as alterações interruptivas gerais que fazem parte do novo design do módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="9881c-135">This section details the general breaking changes that are part of the redesign of the Az module.</span></span>

### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="9881c-136">Alterações do Prefixo de Nomes de Cmdlet</span><span class="sxs-lookup"><span data-stu-id="9881c-136">Cmdlet Noun Prefix Changes</span></span>

<span data-ttu-id="9881c-137">No módulo do AzureRM, os cmdlets utilizavam `AzureRM` ou `Azure` como prefixo de nome.</span><span class="sxs-lookup"><span data-stu-id="9881c-137">In the AzureRM module, cmdlets used either `AzureRM` or `Azure` as a noun prefix.</span></span>  <span data-ttu-id="9881c-138">O Az simplifica e normaliza os nomes de cmdlets, para que todos os cmdlets utilizem "Az" como prefixo de nome de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9881c-138">Az simplifies and normalizes cmdlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="9881c-139">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9881c-139">For example:</span></span>

```azurepowershell-interactive
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="9881c-140">Foi alterado para:</span><span class="sxs-lookup"><span data-stu-id="9881c-140">Has changed to:</span></span>

```azurepowershell-interactive
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="9881c-141">Para simplificar a transição para estes novos nomes de cmdlets, o Az apresenta dois novos cmdlets, [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) e [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span><span class="sxs-lookup"><span data-stu-id="9881c-141">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) and [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span></span>  <span data-ttu-id="9881c-142">`Enable-AzureRmAlias` cria aliases para os nomes de cmdlets mais antigos no AzureRM que os mapeia para os nomes de cmdlets do Az mais recentes.</span><span class="sxs-lookup"><span data-stu-id="9881c-142">`Enable-AzureRmAlias` creates aliases for the older cmdlet names in AzureRM that map to the newer Az cmdlet names.</span></span> <span data-ttu-id="9881c-143">A utilização do argumento `-Scope` com `Enable-AzureRmAlias` permite-lhe escolher onde os aliases estão ativados.</span><span class="sxs-lookup"><span data-stu-id="9881c-143">Using the `-Scope` argument with `Enable-AzureRmAlias` allows you to choose where aliases are enabled.</span></span>

<span data-ttu-id="9881c-144">Por exemplo, o seguinte script no AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9881c-144">For example, the following script in AzureRM:</span></span>

```azurepowershell-interactive
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9881c-145">Pode ser executado com alterações mínimas com `Enable-AzureRmAlias`:</span><span class="sxs-lookup"><span data-stu-id="9881c-145">Can be run with minimal changes using `Enable-AzureRmAlias`:</span></span>

```azurepowershell-interactive
#Requires -Modules Az.Storage
Enable-AzureRmAlias -Scope Process
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9881c-146">A utilização de `Enable-AzureRmAlias -Scope CurrentUser` permite atualizar os aliases em todas as sessões do PowerShell que forem abertas, para que, após a execução deste cmdlet, não seja necessário alterar um script deste tipo:</span><span class="sxs-lookup"><span data-stu-id="9881c-146">Running `Enable-AzureRmAlias -Scope CurrentUser` will enable the aliases for all PowerShell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>

```azurepowershell-interactive
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9881c-147">Para obter detalhes completos sobre a utilização de cmdlets de aliases,veja a [referência Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias).</span><span class="sxs-lookup"><span data-stu-id="9881c-147">For complete details on the usage of the alias cmdlets, see the [Enable-AzureRmAlias reference](/powershell/module/az.accounts/enable-azurermalias).</span></span>

<span data-ttu-id="9881c-148">Quando estiver pronto para desativar aliases, `Disable-AzureRmAlias` remove os aliases criados.</span><span class="sxs-lookup"><span data-stu-id="9881c-148">When you're ready to disable aliases, `Disable-AzureRmAlias` removes the created aliases.</span></span> <span data-ttu-id="9881c-149">Para obter detalhes completos, veja a [referência Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span><span class="sxs-lookup"><span data-stu-id="9881c-149">For complete details, see the [Disable-AzureRmAlias reference](/powershell/module/az.accounts/disable-azurermalias).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9881c-150">Quando desativar aliases, certifique-se de que estão desativados para _todos_ os âmbitos que tiveram aliases ativados.</span><span class="sxs-lookup"><span data-stu-id="9881c-150">When disabling aliases, make sure that they are disabled for _all_ scopes which had aliases enabled.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="9881c-151">Alterações de Nomes de Módulos</span><span class="sxs-lookup"><span data-stu-id="9881c-151">Module Name Changes</span></span>

<span data-ttu-id="9881c-152">Os nomes de módulos foram alterados de `AzureRM.*` para `Az.*`, exceto para os seguintes módulos:</span><span class="sxs-lookup"><span data-stu-id="9881c-152">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>

| <span data-ttu-id="9881c-153">Módulo do AzureRM</span><span class="sxs-lookup"><span data-stu-id="9881c-153">AzureRM module</span></span> | <span data-ttu-id="9881c-154">Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="9881c-154">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="9881c-155">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9881c-155">Azure.Storage</span></span> | <span data-ttu-id="9881c-156">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9881c-156">Az.Storage</span></span> |
| <span data-ttu-id="9881c-157">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9881c-157">Azure.AnalysisServices</span></span> | <span data-ttu-id="9881c-158">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9881c-158">Az.AnalysisServices</span></span> |
| <span data-ttu-id="9881c-159">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9881c-159">AzureRM.Profile</span></span> | <span data-ttu-id="9881c-160">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9881c-160">Az.Accounts</span></span> |
| <span data-ttu-id="9881c-161">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9881c-161">AzureRM.Insights</span></span> | <span data-ttu-id="9881c-162">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="9881c-162">Az.Monitor</span></span> |
| <span data-ttu-id="9881c-163">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="9881c-163">AzureRM.DataFactories</span></span> | <span data-ttu-id="9881c-164">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9881c-164">Az.DataFactory</span></span> |
| <span data-ttu-id="9881c-165">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9881c-165">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="9881c-166">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9881c-166">Az.DataFactory</span></span> |
| <span data-ttu-id="9881c-167">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9881c-167">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="9881c-168">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9881c-168">Az.RecoveryServices</span></span> |
| <span data-ttu-id="9881c-169">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9881c-169">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="9881c-170">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9881c-170">Az.RecoveryServices</span></span> |
| <span data-ttu-id="9881c-171">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9881c-171">AzureRM.Tags</span></span> | <span data-ttu-id="9881c-172">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9881c-172">Az.Resources</span></span> |
| <span data-ttu-id="9881c-173">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="9881c-173">AzureRM.MachineLearningCompute</span></span> | <span data-ttu-id="9881c-174">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="9881c-174">Az.MachineLearning</span></span> |
| <span data-ttu-id="9881c-175">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="9881c-175">AzureRM.UsageAggregates</span></span> | <span data-ttu-id="9881c-176">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="9881c-176">Az.Billing</span></span> |
| <span data-ttu-id="9881c-177">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9881c-177">AzureRM.Consumption</span></span> | <span data-ttu-id="9881c-178">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="9881c-178">Az.Billing</span></span> |

<span data-ttu-id="9881c-179">As alterações realizadas ao nível dos nomes de módulos significam que qualquer script que utilizar `#Requires` ou `Import-Module` para carregar módulos específicos terá de ser alterado de modo a utilizar o novo módulo.</span><span class="sxs-lookup"><span data-stu-id="9881c-179">The changes in module names mean that any script that uses `#Requires` or `Import-Module` to load specific modules will need to be changed to use the new module instead.</span></span> <span data-ttu-id="9881c-180">Para os módulos em que o sufixo de cmdlet não foi alterado, embora o nome do módulo tenha sido alterado, o sufixo que indica o espaço da operação _não foi alterado_.</span><span class="sxs-lookup"><span data-stu-id="9881c-180">For modules where the cmdlet suffix has not changed, this means that although the module name has changed, the suffix indicating the operation space has _not_.</span></span>

#### <a name="migrating-requires-and-import-module-statements"></a><span data-ttu-id="9881c-181">Migrar Declarações #Requires e Import-Module</span><span class="sxs-lookup"><span data-stu-id="9881c-181">Migrating #Requires and Import-Module Statements</span></span>

<span data-ttu-id="9881c-182">Os scripts que utilizam `#Requires` ou `Import-Module` para declarar uma dependência nos módulos do AzureRM devem ser atualizados de modo a utilizarem os novos nomes de módulos.</span><span class="sxs-lookup"><span data-stu-id="9881c-182">Scripts that use `#Requires` or `Import-Module` to declare a dependency on AzureRM modules must be updated to use the new module names.</span></span> <span data-ttu-id="9881c-183">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9881c-183">For example:</span></span>

```azurepowershell-interactive
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="9881c-184">Deve ser alterado para:</span><span class="sxs-lookup"><span data-stu-id="9881c-184">Should be changed to:</span></span>

```azurepowershell-interactive
#Requires -Module Az.Compute
```

<span data-ttu-id="9881c-185">Para `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="9881c-185">For `Import-Module`:</span></span>

```azurepowershell-interactive
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="9881c-186">Deve ser alterado para:</span><span class="sxs-lookup"><span data-stu-id="9881c-186">Should be changed to:</span></span>

```azurepowershell-interactive
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="9881c-187">Migrar Invocações de Cmdlets Completamente Qualificados</span><span class="sxs-lookup"><span data-stu-id="9881c-187">Migrating Fully-Qualified Cmdlet Invocations</span></span>

<span data-ttu-id="9881c-188">Os scripts que utilizam invocações de cmdlets qualificados por módulo, como:</span><span class="sxs-lookup"><span data-stu-id="9881c-188">Scripts that use module-qualified cmdlet invocations, such as:</span></span>

```azurepowershell-interactive
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="9881c-189">Têm de ser alterados de modo a utilizarem os novos nomes de módulos e cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9881c-189">Must be changed to use the new module and cmdlet names:</span></span>

```azurepowershell-interactive
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="9881c-190">Migrar dependências de manifestos de módulos</span><span class="sxs-lookup"><span data-stu-id="9881c-190">Migrating module manifest dependencies</span></span>

<span data-ttu-id="9881c-191">Os módulos que expressam dependências nos módulos do AzureRM através de um ficheiro (.psd1) de manifesto de módulo terão de atualizar os nomes de módulos na respetiva secção `RequiredModules`:</span><span class="sxs-lookup"><span data-stu-id="9881c-191">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their `RequiredModules` section:</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="9881c-192">Tem de ser alterado para:</span><span class="sxs-lookup"><span data-stu-id="9881c-192">Must be changed to:</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="9881c-193">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="9881c-193">Removed modules</span></span>

<span data-ttu-id="9881c-194">Os módulos seguintes foram removidos:</span><span class="sxs-lookup"><span data-stu-id="9881c-194">The following modules have been removed:</span></span>

- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="9881c-195">As ferramentas para estes serviços já não são suportadas ativamente.</span><span class="sxs-lookup"><span data-stu-id="9881c-195">The tools for these services are no longer actively supported.</span></span>  <span data-ttu-id="9881c-196">Os clientes são incentivados a mudar para serviços alternativos assim que for possível.</span><span class="sxs-lookup"><span data-stu-id="9881c-196">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="9881c-197">Windows PowerShell 5.1 e .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="9881c-197">Windows PowerShell 5.1 and .NET 4.7.2</span></span>

<span data-ttu-id="9881c-198">Para utilizar o Az com o PowerShell 5.1 para Windows, tem de instalar o .NET Framework 4.7.2.</span><span class="sxs-lookup"><span data-stu-id="9881c-198">Using Az with PowerShell 5.1 for Windows requires the installation of .NET Framework 4.7.2.</span></span> <span data-ttu-id="9881c-199">A utilização do PowerShell Core 6.x ou posterior não requer o .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="9881c-199">Using PowerShell Core 6.x or later does not require .NET Framework.</span></span>

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="9881c-200">Remoção temporária do Início de sessão do utilizador através de PSCredential</span><span class="sxs-lookup"><span data-stu-id="9881c-200">Temporary removal of User login using PSCredential</span></span>

<span data-ttu-id="9881c-201">Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a remover temporariamente o início de sessão do utilizador através de PSCredential.</span><span class="sxs-lookup"><span data-stu-id="9881c-201">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="9881c-202">Esta capacidade será introduzida novamente na versão de 15/01/2019 para o PowerShell 5.1 para Windows.</span><span class="sxs-lookup"><span data-stu-id="9881c-202">This capability will be re-introduced in the 1/15/2019 release for PowerShell 5.1 for Windows.</span></span> <span data-ttu-id="9881c-203">Este assunto é abordado em detalhe [neste debate sobre o problema no GitHub](https://github.com/Azure/azure-powershell/issues/7430).</span><span class="sxs-lookup"><span data-stu-id="9881c-203">This is discussed in detail in [this GitHub issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="9881c-204">Início de sessão com o código de dispositivo predefinido em vez da linha de comandos do browser</span><span class="sxs-lookup"><span data-stu-id="9881c-204">Default device code login instead of web browser prompt</span></span>

<span data-ttu-id="9881c-205">Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a utilizar o início de sessão de dispositivo como o fluxo de início de sessão predefinido durante o início de sessão interativo.</span><span class="sxs-lookup"><span data-stu-id="9881c-205">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="9881c-206">O início de sessão baseado no browser será introduzido novamente para o PowerShell 5.1 para Windows como a predefinição na versão de 15/01/2019.</span><span class="sxs-lookup"><span data-stu-id="9881c-206">Web browser based login will be re-introduced for PowerShell 5.1 for Windows as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="9881c-207">Nessa altura, os utilizadores poderão escolher o início de sessão de dispositivo através de um parâmetro de mudança (Switch).</span><span class="sxs-lookup"><span data-stu-id="9881c-207">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="9881c-208">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="9881c-208">Module breaking changes</span></span>

<span data-ttu-id="9881c-209">Esta secção fornece detalhes sobre alterações interruptivas específicas para cmdlets e módulos individuais.</span><span class="sxs-lookup"><span data-stu-id="9881c-209">This section details specific breaking changes for individual modules and cmdlets.</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="9881c-210">Az.ApiManagement (anteriormente AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="9881c-210">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>

- <span data-ttu-id="9881c-211">Foram removidos os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9881c-211">Removed the following cmdlets:</span></span>
  - <span data-ttu-id="9881c-212">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9881c-212">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="9881c-213">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9881c-213">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="9881c-214">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9881c-214">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="9881c-215">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9881c-215">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="9881c-216">Em alternativa, utilize o cmdlet **Set-AzApiManagement** para definir estas propriedades</span><span class="sxs-lookup"><span data-stu-id="9881c-216">Use **Set-AzApiManagement** cmdlet to set these properties instead</span></span>
- <span data-ttu-id="9881c-217">Foram removidas as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="9881c-217">Removed the following properties:</span></span>
  - <span data-ttu-id="9881c-218">As propriedades `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` e `ScmHostnameConfiguration` do tipo `PsApiManagementHostnameConfiguration` foram removidas de `PsApiManagementContext`.</span><span class="sxs-lookup"><span data-stu-id="9881c-218">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="9881c-219">Em vez disso, utilize `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` e `ScmCustomHostnameConfiguration` do tipo `PsApiManagementCustomHostNameConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="9881c-219">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="9881c-220">A propriedade `StaticIPs` foi removida de PsApiManagementContext.</span><span class="sxs-lookup"><span data-stu-id="9881c-220">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="9881c-221">A propriedade foi dividida em `PublicIPAddresses` e `PrivateIPAddresses`.</span><span class="sxs-lookup"><span data-stu-id="9881c-221">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="9881c-222">A propriedade necessária `Location` foi removida do cmdlet New-AzureApiManagementVirtualNetwork.</span><span class="sxs-lookup"><span data-stu-id="9881c-222">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="9881c-223">Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="9881c-223">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>

- <span data-ttu-id="9881c-224">O parâmetro `InvoiceName` foi removido do cmdlet `Get-AzConsumptionUsageDetail`.</span><span class="sxs-lookup"><span data-stu-id="9881c-224">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="9881c-225">Os scripts terão de utilizar outros parâmetros de identidade para a faturação.</span><span class="sxs-lookup"><span data-stu-id="9881c-225">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="9881c-226">Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="9881c-226">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>

- <span data-ttu-id="9881c-227">O conjunto de parâmetros `GetSkusWithAccountParamSetName` foi removido do cmdlet `Get-AzCognitiveServicesAccountSkus`.</span><span class="sxs-lookup"><span data-stu-id="9881c-227">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="9881c-228">Tem de obter os Skus através do Tipo de Conta e da Localização, em vez de utilizar ResourceGroupName e o Nome da Conta.</span><span class="sxs-lookup"><span data-stu-id="9881c-228">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="9881c-229">Az.Compute (anteriormente AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="9881c-229">Az.Compute (previously AzureRM.Compute)</span></span>

- <span data-ttu-id="9881c-230">Os `IdentityIds` foram removidos da propriedade `Identity` nos objetos `PSVirtualMachine` e `PSVirtualMachineScaleSet`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9881c-230">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="9881c-231">O tipo de propriedade `InstanceView` do objeto `PSVirtualMachineScaleSetVM` foi alterado de `VirtualMachineInstanceView` para `VirtualMachineScaleSetVMInstanceView`</span><span class="sxs-lookup"><span data-stu-id="9881c-231">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="9881c-232">As propriedades `AutoOSUpgradePolicy` e `AutomaticOSUpgrade` foram removidas da propriedade `UpgradePolicy`</span><span class="sxs-lookup"><span data-stu-id="9881c-232">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="9881c-233">O tipo de propriedade `Sku` no objeto `PSSnapshotUpdate` foi alterado de `DiskSku` para `SnapshotSku`</span><span class="sxs-lookup"><span data-stu-id="9881c-233">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="9881c-234">`VmScaleSetVMParameterSet` foi removido do cmdlet `Add-AzVMDataDisk`. Já não pode adicionar um disco de dados individualmente a uma VM de conjunto de dimensionamento (ScaleSet).</span><span class="sxs-lookup"><span data-stu-id="9881c-234">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you cna no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="9881c-235">Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="9881c-235">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>

- <span data-ttu-id="9881c-236">O parâmetro `GatewayName` tornou-se obrigatório no cmdlet `New-AzDataFactoryEncryptValue`</span><span class="sxs-lookup"><span data-stu-id="9881c-236">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="9881c-237">O cmdlet `New-AzDataFactoryGatewayKey` foi removido</span><span class="sxs-lookup"><span data-stu-id="9881c-237">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="9881c-238">O parâmetro `LinkedServiceName` foi removido do cmdlet `Get-AzDataFactoryV2ActivityRun`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9881c-238">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="9881c-239">Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="9881c-239">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>

- <span data-ttu-id="9881c-240">Os cmdlets preteridos que se seguem foram removidos: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret` e `Set-AzDataLakeAnalyticsCatalogSecret`</span><span class="sxs-lookup"><span data-stu-id="9881c-240">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="9881c-241">Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="9881c-241">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>

- <span data-ttu-id="9881c-242">O tipo do parâmetro `Encoding` foi alterado de `FileSystemCmdletProviderEncoding` para `System.Text.Encoding` nos cmdlets que se seguem.</span><span class="sxs-lookup"><span data-stu-id="9881c-242">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="9881c-243">Esta alteração remove os valores de codificação `String` e `Oem`.</span><span class="sxs-lookup"><span data-stu-id="9881c-243">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="9881c-244">Todos os outros valores de codificação anteriores permanecem.</span><span class="sxs-lookup"><span data-stu-id="9881c-244">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="9881c-245">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="9881c-245">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="9881c-246">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="9881c-246">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="9881c-247">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="9881c-247">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="9881c-248">O alias de propriedade preterido `Tags` foi removido dos cmdlets `New-AzDataLakeStoreAccount` e `Set-AzDataLakeStoreAccount`</span><span class="sxs-lookup"><span data-stu-id="9881c-248">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="9881c-249">Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9881c-249">Scripts using</span></span>
  ```azurepowershell-interactive
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="9881c-250">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9881c-250">Should be changed to</span></span>
  ```azurepowershell-interactive
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="9881c-251">As propriedades preteridas `Identity`, `EncryptionState`, `EncryptionProvisioningState`, `EncryptionConfig`, `FirewallState`, `FirewallRules`, `VirtualNetworkRules`, `TrustedIdProviderState`, `TrustedIdProviders`, `DefaultGroup`, `NewTier`, `CurrentTier` e `FirewallAllowAzureIps` foram removidas do objeto `PSDataLakeStoreAccountBasic`.</span><span class="sxs-lookup"><span data-stu-id="9881c-251">Removed deprecated properties `Identity`, `EncryptionState`, `EncryptionProvisioningState`, `EncryptionConfig`, `FirewallState`, `FirewallRules`, `VirtualNetworkRules`, `TrustedIdProviderState`, `TrustedIdProviders`, `DefaultGroup`, `NewTier`, `CurrentTier`, `FirewallAllowAzureIps` from `PSDataLakeStoreAccountBasic` object.</span></span>  <span data-ttu-id="9881c-252">Qualquer script que utilize `PSDatalakeStoreAccount` devolvido a partir de `Get-AzDataLakeStoreAccount` não deve fazer referência a essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9881c-252">Any script that uses the `PSDatalakeStoreAccount` returned from `Get-AzDataLakeStoreAccount` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="9881c-253">Az.KeyVault (anteriormente AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="9881c-253">Az.KeyVault (previously AzureRM.KeyVault)</span></span>

- <span data-ttu-id="9881c-254">A propriedade `PurgeDisabled` foi removida dos objetos `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` e `PSKeyVaultSecretAttributes`. Os scripts devem deixar de fazer referência à propriedade ```PurgeDisabled``` para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9881c-254">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts should no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="9881c-255">Az.Media (anteriormente AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="9881c-255">Az.Media (previously AzureRM.Media)</span></span>

- <span data-ttu-id="9881c-256">O alias de propriedade preterido `Tags` foi removido do cmdlet `New-AzMediaService`. Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9881c-256">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```azurepowershell-interactive
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="9881c-257">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9881c-257">Should be changed to</span></span>
  ```azurepowershell-interactive
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```

### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="9881c-258">Az.Monitor (anteriormente AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="9881c-258">Az.Monitor (previously AzureRM.Insights)</span></span>

- <span data-ttu-id="9881c-259">Os nomes de parâmetros no plural `Categories` e `Timegrains` foram removidos em prol de nomes de parâmetros no singular do cmdlet `Set-AzDiagnosticSetting`. Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9881c-259">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```azurepowershell-interactive
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="9881c-260">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9881c-260">Should be changed to</span></span>
  ```azurepowershell-interactive
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```

### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="9881c-261">Az.Network (anteriormente AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="9881c-261">Az.Network (previously AzureRM.Network)</span></span>

- <span data-ttu-id="9881c-262">O parâmetro preterido `ResourceId` foi removido do cmdlet `Get-AzServiceEndpointPolicyDefinition`</span><span class="sxs-lookup"><span data-stu-id="9881c-262">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="9881c-263">A propriedade preterida `EnableVmProtection` foi removida do objeto `PSVirtualNetwork`</span><span class="sxs-lookup"><span data-stu-id="9881c-263">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="9881c-264">O cmdlet preterido `Set-AzVirtualNetworkGatewayVpnClientConfig` foi removido</span><span class="sxs-lookup"><span data-stu-id="9881c-264">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>
  
<span data-ttu-id="9881c-265">Os scripts devem deixar de tomar decisões de processamento com base nos valores destes campos.</span><span class="sxs-lookup"><span data-stu-id="9881c-265">Scripts should no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="9881c-266">Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="9881c-266">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>

- <span data-ttu-id="9881c-267">O conjunto de parâmetros predefinido para `Get-AzOperationalInsightsDataSource` foi removido e `ByWorkspaceNameByKind` passou a ser o conjunto de parâmetros predefinido</span><span class="sxs-lookup"><span data-stu-id="9881c-267">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="9881c-268">Os scripts que listavam origens de dados com</span><span class="sxs-lookup"><span data-stu-id="9881c-268">Scripts that listed data sources using</span></span>
  ```azurepowershell-interactive
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="9881c-269">Devem ser alterados para especificar um tipo (Kind)</span><span class="sxs-lookup"><span data-stu-id="9881c-269">Should be changed to specify a Kind</span></span>
  ```azurepowershell-interactive
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9881c-270">Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="9881c-270">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>

- <span data-ttu-id="9881c-271">O parâmetro `Encryption` foi removido do cmdlet `New/Set-AzRecoveryServicesAsrPolicy`</span><span class="sxs-lookup"><span data-stu-id="9881c-271">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="9881c-272">Agora, o parâmetro `TargetStorageAccountName` é obrigatório para os restauros de discos geridos no cmdlet `Restore-AzRecoveryServicesBackupItem`</span><span class="sxs-lookup"><span data-stu-id="9881c-272">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="9881c-273">Os parâmetros `StorageAccountName` e `StorageAccountResourceGroupName` foram removidos no cmdlet `Restore-AzRecoveryServicesBackupItem`</span><span class="sxs-lookup"><span data-stu-id="9881c-273">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="9881c-274">O parâmetro `Name` foi removido no cmdlet `Get-AzRecoveryServicesBackupContainer`</span><span class="sxs-lookup"><span data-stu-id="9881c-274">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="9881c-275">Az.Resources (anteriormente AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="9881c-275">Az.Resources (previously AzureRM.Resources)</span></span>

- <span data-ttu-id="9881c-276">O parâmetro `Sku` foi removido do cmdlet `New/Set-AzPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="9881c-276">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="9881c-277">O parâmetro `Password` foi removido dos cmdlets `New-AzADServicePrincipal` e `New-AzADSpCredential`. As palavras-passe são geradas automaticamente e o scripts que forneciam a palavra-passe:</span><span class="sxs-lookup"><span data-stu-id="9881c-277">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>

  ```azurepowershell-interactive
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="9881c-278">Devem ser alterados de modo a obterem a palavra-passe a partir da saída:</span><span class="sxs-lookup"><span data-stu-id="9881c-278">Should be changed to retrieve the password from the output:</span></span>

  ```azurepowershell-interactive
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="9881c-279">Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="9881c-279">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>

- <span data-ttu-id="9881c-280">Foram alterados os seguintes tipos de retorno de cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9881c-280">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="9881c-281">A propriedade `ServiceTypeHealthPolicies` do tipo `ApplicationHealthPolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9881c-281">The property `ServiceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="9881c-282">A propriedade `ApplicationHealthPolicies` do tipo `ClusterUpgradeDeltaHealthPolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9881c-282">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="9881c-283">A propriedade `OverrideUserUpgradePolicy` do tipo `ClusterUpgradePolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9881c-283">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="9881c-284">Estas alterações afetam os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9881c-284">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="9881c-285">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="9881c-285">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="9881c-286">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="9881c-286">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="9881c-287">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="9881c-287">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="9881c-288">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="9881c-288">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="9881c-289">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="9881c-289">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="9881c-290">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="9881c-290">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="9881c-291">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="9881c-291">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="9881c-292">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="9881c-292">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="9881c-293">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="9881c-293">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="9881c-294">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="9881c-294">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="9881c-295">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="9881c-295">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="9881c-296">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="9881c-296">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="9881c-297">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="9881c-297">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="9881c-298">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="9881c-298">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="9881c-299">Az.Sql (anteriormente AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="9881c-299">Az.Sql (previously AzureRM.Sql)</span></span>

- <span data-ttu-id="9881c-300">Os parâmetros `State` e `ResourceId` foram removidos do cmdlet `Set-AzSqlDatabaseBackupLongTermRetentionPolicy`</span><span class="sxs-lookup"><span data-stu-id="9881c-300">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="9881c-301">Foram removidos os seguintes cmdlets preteridos: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing` e `Remove-AzSqlServerAuditing`</span><span class="sxs-lookup"><span data-stu-id="9881c-301">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="9881c-302">O parâmetro preterido `Current` foi removido do cmdlet `Get-AzSqlDatabaseBackupLongTermRetentionPolicy`</span><span class="sxs-lookup"><span data-stu-id="9881c-302">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="9881c-303">O parâmetro preterido `DatabaseName` foi removido do cmdlet `Get-AzSqlServerServiceObjective`</span><span class="sxs-lookup"><span data-stu-id="9881c-303">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="9881c-304">O parâmetro preterido `PrivilegedLogin` foi removido do cmdlet `Set-AzSqlDatabaseDataMaskingPolicy`</span><span class="sxs-lookup"><span data-stu-id="9881c-304">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="9881c-305">Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="9881c-305">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>

- <span data-ttu-id="9881c-306">Para suportar a criação de um contexto de armazenamento de Oauth com apenas o nome da conta de armazenamento, o conjunto de parâmetros predefinido foi alterado para `OAuthParameterSet`</span><span class="sxs-lookup"><span data-stu-id="9881c-306">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="9881c-307">Exemplo: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="9881c-307">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="9881c-308">O parâmetro `Location` tornou-se obrigatório no cmdlet `Get-AzStorageUsage`</span><span class="sxs-lookup"><span data-stu-id="9881c-308">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="9881c-309">Os métodos da API de Armazenamento utilizam agora o Padrão Assíncrono Baseado em Tarefas (TAP), em vez de chamadas síncronas à API.</span><span class="sxs-lookup"><span data-stu-id="9881c-309">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span> <span data-ttu-id="9881c-310">Os exemplos seguintes demonstram os novos comandos assíncronos:</span><span class="sxs-lookup"><span data-stu-id="9881c-310">The following examples demonstrate the new asynchronous commands:</span></span>

#### <a name="blob-snapshot"></a><span data-ttu-id="9881c-311">Instantâneo do Blob</span><span class="sxs-lookup"><span data-stu-id="9881c-311">Blob Snapshot</span></span>

<span data-ttu-id="9881c-312">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9881c-312">AzureRM:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

<span data-ttu-id="9881c-313">Az:</span><span class="sxs-lookup"><span data-stu-id="9881c-313">Az:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="share-snapshot"></a><span data-ttu-id="9881c-314">Instantâneo da Partilha</span><span class="sxs-lookup"><span data-stu-id="9881c-314">Share Snapshot</span></span>

<span data-ttu-id="9881c-315">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9881c-315">AzureRM:</span></span>

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```

<span data-ttu-id="9881c-316">Az:</span><span class="sxs-lookup"><span data-stu-id="9881c-316">Az:</span></span>

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="undelete-soft-deleted-blob"></a><span data-ttu-id="9881c-317">Anular eliminação do blob eliminado de forma recuperável</span><span class="sxs-lookup"><span data-stu-id="9881c-317">Undelete soft-deleted blob</span></span>

<span data-ttu-id="9881c-318">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9881c-318">AzureRM:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```

<span data-ttu-id="9881c-319">Az:</span><span class="sxs-lookup"><span data-stu-id="9881c-319">Az:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="set-blob-tier"></a><span data-ttu-id="9881c-320">Definir Camada de Blob</span><span class="sxs-lookup"><span data-stu-id="9881c-320">Set Blob Tier</span></span>

<span data-ttu-id="9881c-321">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9881c-321">AzureRM:</span></span>

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

<span data-ttu-id="9881c-322">Az:</span><span class="sxs-lookup"><span data-stu-id="9881c-322">Az:</span></span>

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="9881c-323">Az.Websites (anteriormente AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="9881c-323">Az.Websites (previously AzureRM.Websites)</span></span>

- <span data-ttu-id="9881c-324">As propriedades preteridas foram removidas dos objetos `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` e `PSSite`</span><span class="sxs-lookup"><span data-stu-id="9881c-324">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>
