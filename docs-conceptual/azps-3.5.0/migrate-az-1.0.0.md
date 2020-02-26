---
title: Todas as alterações do AzureRM para o Azure PowerShell Az 1.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 1.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2019
ms.openlocfilehash: e5121d61b0f5f68ff3e1f33d774e3533adfeb64f
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477768"
---
# <a name="breaking-changes-for-az-100"></a><span data-ttu-id="9fd82-103">Alterações interruptivas do Az 1.0.0</span><span class="sxs-lookup"><span data-stu-id="9fd82-103">Breaking changes for Az 1.0.0</span></span>

<span data-ttu-id="9fd82-104">Este documento fornece informações detalhadas sobre as alterações entre o AzureRM 6.x e o novo módulo do Az, versão 1.x e posterior.</span><span class="sxs-lookup"><span data-stu-id="9fd82-104">This document provides detailed information on the changes between AzureRM 6.x and the new Az module, version 1.x and later.</span></span> <span data-ttu-id="9fd82-105">O índice irá guiá-lo através de um caminho de migração completo, incluindo alterações específicas do módulo que podem afetar os scripts.</span><span class="sxs-lookup"><span data-stu-id="9fd82-105">The table of contents will help guide you through a full migration path, including module-specific changes that may affect your scripts.</span></span>

<span data-ttu-id="9fd82-106">Para obter orientação geral sobre como começar uma migração do AzureRM para o Az, veja [Iniciar a migração do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="9fd82-106">For general advice on getting started with a migration from AzureRM to Az, see [Start migration from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9fd82-107">Também têm sido feitas alterações interruptivas entre o Az 1.0.0 e o Az 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="9fd82-107">There have been breaking changes between Az 1.0.0 and Az 2.0.0 as well.</span></span> <span data-ttu-id="9fd82-108">Depois de seguir este guia para atualizar do AzureRM para o Az, veja as [alterações interruptivas do Az 2.0.0](migrate-az-2.0.0.md) para saber se tem de fazer alterações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9fd82-108">After following this guide for updating from AzureRM to Az, see the [Az 2.0.0 breaking changes](migrate-az-2.0.0.md) to find out if you need to make additional changes.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="9fd82-109">Índice</span><span class="sxs-lookup"><span data-stu-id="9fd82-109">Table of Contents</span></span>

- [<span data-ttu-id="9fd82-110">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="9fd82-110">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="9fd82-111">Alterações dos prefixo de nomes de cmdlets</span><span class="sxs-lookup"><span data-stu-id="9fd82-111">Cmdlet noun prefix changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="9fd82-112">Alterações de Nomes de Módulos</span><span class="sxs-lookup"><span data-stu-id="9fd82-112">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="9fd82-113">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="9fd82-113">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="9fd82-114">Windows PowerShell 5.1 e .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="9fd82-114">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="9fd82-115">Remoção temporária do início de sessão do utilizador através de PSCredential</span><span class="sxs-lookup"><span data-stu-id="9fd82-115">Temporary removal of user login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="9fd82-116">Início de sessão com o código de dispositivo predefinido em vez da linha de comandos do browser</span><span class="sxs-lookup"><span data-stu-id="9fd82-116">Default device code login instead of web browser prompt</span></span>](#default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="9fd82-117">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="9fd82-117">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="9fd82-118">Az.ApiManagement (anteriormente AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="9fd82-118">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="9fd82-119">Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="9fd82-119">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="9fd82-120">Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="9fd82-120">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="9fd82-121">Az.Compute (anteriormente AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="9fd82-121">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="9fd82-122">Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="9fd82-122">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="9fd82-123">Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="9fd82-123">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="9fd82-124">Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="9fd82-124">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="9fd82-125">Az.KeyVault (anteriormente AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="9fd82-125">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="9fd82-126">Az.Media (anteriormente AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="9fd82-126">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="9fd82-127">Az.Monitor (anteriormente AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="9fd82-127">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="9fd82-128">Az.Network (anteriormente AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="9fd82-128">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="9fd82-129">Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="9fd82-129">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="9fd82-130">Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="9fd82-130">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="9fd82-131">Az.Resources (anteriormente AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="9fd82-131">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="9fd82-132">Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="9fd82-132">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="9fd82-133">Az.Sql (anteriormente AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="9fd82-133">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="9fd82-134">Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="9fd82-134">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="9fd82-135">Az.Websites (anteriormente AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="9fd82-135">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="9fd82-136">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="9fd82-136">General breaking changes</span></span>

<span data-ttu-id="9fd82-137">Esta secção fornece detalhes sobre as alterações interruptivas gerais que fazem parte do novo design do módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="9fd82-137">This section details the general breaking changes that are part of the redesign of the Az module.</span></span>

### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="9fd82-138">Alterações do Prefixo de Nomes de Cmdlet</span><span class="sxs-lookup"><span data-stu-id="9fd82-138">Cmdlet Noun Prefix Changes</span></span>

<span data-ttu-id="9fd82-139">No módulo do AzureRM, os cmdlets utilizavam `AzureRM` ou `Azure` como prefixo de nome.</span><span class="sxs-lookup"><span data-stu-id="9fd82-139">In the AzureRM module, cmdlets used either `AzureRM` or `Azure` as a noun prefix.</span></span>  <span data-ttu-id="9fd82-140">O Az simplifica e normaliza os nomes de cmdlets, para que todos os cmdlets utilizem "Az" como prefixo de nome de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9fd82-140">Az simplifies and normalizes cmdlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="9fd82-141">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9fd82-141">For example:</span></span>

```azurepowershell-interactive
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="9fd82-142">Foi alterado para:</span><span class="sxs-lookup"><span data-stu-id="9fd82-142">Has changed to:</span></span>

```azurepowershell-interactive
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="9fd82-143">Para simplificar a transição para estes novos nomes de cmdlets, o Az apresenta dois novos cmdlets, [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) e [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span><span class="sxs-lookup"><span data-stu-id="9fd82-143">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) and [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span></span>  <span data-ttu-id="9fd82-144">`Enable-AzureRmAlias` cria aliases para os nomes de cmdlets mais antigos no AzureRM que os mapeia para os nomes de cmdlets do Az mais recentes.</span><span class="sxs-lookup"><span data-stu-id="9fd82-144">`Enable-AzureRmAlias` creates aliases for the older cmdlet names in AzureRM that map to the newer Az cmdlet names.</span></span> <span data-ttu-id="9fd82-145">A utilização do argumento `-Scope` com `Enable-AzureRmAlias` permite-lhe escolher onde os aliases estão ativados.</span><span class="sxs-lookup"><span data-stu-id="9fd82-145">Using the `-Scope` argument with `Enable-AzureRmAlias` allows you to choose where aliases are enabled.</span></span>

<span data-ttu-id="9fd82-146">Por exemplo, o seguinte script no AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9fd82-146">For example, the following script in AzureRM:</span></span>

```azurepowershell-interactive
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9fd82-147">Pode ser executado com alterações mínimas com `Enable-AzureRmAlias`:</span><span class="sxs-lookup"><span data-stu-id="9fd82-147">Can be run with minimal changes using `Enable-AzureRmAlias`:</span></span>

```azurepowershell-interactive
#Requires -Modules Az.Storage
Enable-AzureRmAlias -Scope Process
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9fd82-148">A utilização de `Enable-AzureRmAlias -Scope CurrentUser` permite atualizar os aliases em todas as sessões do PowerShell que forem abertas, para que, após a execução deste cmdlet, não seja necessário alterar um script deste tipo:</span><span class="sxs-lookup"><span data-stu-id="9fd82-148">Running `Enable-AzureRmAlias -Scope CurrentUser` will enable the aliases for all PowerShell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>

```azurepowershell-interactive
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9fd82-149">Para obter detalhes completos sobre a utilização de cmdlets de aliases,veja a [referência Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias).</span><span class="sxs-lookup"><span data-stu-id="9fd82-149">For complete details on the usage of the alias cmdlets, see the [Enable-AzureRmAlias reference](/powershell/module/az.accounts/enable-azurermalias).</span></span>

<span data-ttu-id="9fd82-150">Quando estiver pronto para desativar aliases, `Disable-AzureRmAlias` remove os aliases criados.</span><span class="sxs-lookup"><span data-stu-id="9fd82-150">When you're ready to disable aliases, `Disable-AzureRmAlias` removes the created aliases.</span></span> <span data-ttu-id="9fd82-151">Para obter detalhes completos, veja a [referência Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span><span class="sxs-lookup"><span data-stu-id="9fd82-151">For complete details, see the [Disable-AzureRmAlias reference](/powershell/module/az.accounts/disable-azurermalias).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9fd82-152">Quando desativar aliases, certifique-se de que estão desativados para _todos_ os âmbitos que tiveram aliases ativados.</span><span class="sxs-lookup"><span data-stu-id="9fd82-152">When disabling aliases, make sure that they are disabled for _all_ scopes which had aliases enabled.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="9fd82-153">Alterações de Nomes de Módulos</span><span class="sxs-lookup"><span data-stu-id="9fd82-153">Module Name Changes</span></span>

<span data-ttu-id="9fd82-154">Os nomes de módulos foram alterados de `AzureRM.*` para `Az.*`, exceto para os seguintes módulos:</span><span class="sxs-lookup"><span data-stu-id="9fd82-154">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>

| <span data-ttu-id="9fd82-155">Módulo do AzureRM</span><span class="sxs-lookup"><span data-stu-id="9fd82-155">AzureRM module</span></span> | <span data-ttu-id="9fd82-156">Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="9fd82-156">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="9fd82-157">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9fd82-157">Azure.Storage</span></span> | <span data-ttu-id="9fd82-158">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9fd82-158">Az.Storage</span></span> |
| <span data-ttu-id="9fd82-159">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9fd82-159">Azure.AnalysisServices</span></span> | <span data-ttu-id="9fd82-160">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9fd82-160">Az.AnalysisServices</span></span> |
| <span data-ttu-id="9fd82-161">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9fd82-161">AzureRM.Profile</span></span> | <span data-ttu-id="9fd82-162">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9fd82-162">Az.Accounts</span></span> |
| <span data-ttu-id="9fd82-163">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9fd82-163">AzureRM.Insights</span></span> | <span data-ttu-id="9fd82-164">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="9fd82-164">Az.Monitor</span></span> |
| <span data-ttu-id="9fd82-165">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="9fd82-165">AzureRM.DataFactories</span></span> | <span data-ttu-id="9fd82-166">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9fd82-166">Az.DataFactory</span></span> |
| <span data-ttu-id="9fd82-167">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9fd82-167">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="9fd82-168">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9fd82-168">Az.DataFactory</span></span> |
| <span data-ttu-id="9fd82-169">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9fd82-169">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="9fd82-170">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9fd82-170">Az.RecoveryServices</span></span> |
| <span data-ttu-id="9fd82-171">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9fd82-171">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="9fd82-172">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9fd82-172">Az.RecoveryServices</span></span> |
| <span data-ttu-id="9fd82-173">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9fd82-173">AzureRM.Tags</span></span> | <span data-ttu-id="9fd82-174">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9fd82-174">Az.Resources</span></span> |
| <span data-ttu-id="9fd82-175">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="9fd82-175">AzureRM.MachineLearningCompute</span></span> | <span data-ttu-id="9fd82-176">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="9fd82-176">Az.MachineLearning</span></span> |
| <span data-ttu-id="9fd82-177">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="9fd82-177">AzureRM.UsageAggregates</span></span> | <span data-ttu-id="9fd82-178">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="9fd82-178">Az.Billing</span></span> |
| <span data-ttu-id="9fd82-179">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9fd82-179">AzureRM.Consumption</span></span> | <span data-ttu-id="9fd82-180">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="9fd82-180">Az.Billing</span></span> |

<span data-ttu-id="9fd82-181">As alterações realizadas ao nível dos nomes de módulos significam que qualquer script que utilizar `#Requires` ou `Import-Module` para carregar módulos específicos terá de ser alterado de modo a utilizar o novo módulo.</span><span class="sxs-lookup"><span data-stu-id="9fd82-181">The changes in module names mean that any script that uses `#Requires` or `Import-Module` to load specific modules will need to be changed to use the new module instead.</span></span> <span data-ttu-id="9fd82-182">Para os módulos em que o sufixo de cmdlet não foi alterado, embora o nome do módulo tenha sido alterado, o sufixo que indica o espaço da operação _não foi alterado_.</span><span class="sxs-lookup"><span data-stu-id="9fd82-182">For modules where the cmdlet suffix has not changed, this means that although the module name has changed, the suffix indicating the operation space has _not_.</span></span>

#### <a name="migrating-requires-and-import-module-statements"></a><span data-ttu-id="9fd82-183">Migrar Declarações #Requires e Import-Module</span><span class="sxs-lookup"><span data-stu-id="9fd82-183">Migrating #Requires and Import-Module Statements</span></span>

<span data-ttu-id="9fd82-184">Os scripts que utilizam `#Requires` ou `Import-Module` para declarar uma dependência nos módulos do AzureRM devem ser atualizados de modo a utilizarem os novos nomes de módulos.</span><span class="sxs-lookup"><span data-stu-id="9fd82-184">Scripts that use `#Requires` or `Import-Module` to declare a dependency on AzureRM modules must be updated to use the new module names.</span></span> <span data-ttu-id="9fd82-185">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9fd82-185">For example:</span></span>

```azurepowershell-interactive
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="9fd82-186">Deve ser alterado para:</span><span class="sxs-lookup"><span data-stu-id="9fd82-186">Should be changed to:</span></span>

```azurepowershell-interactive
#Requires -Module Az.Compute
```

<span data-ttu-id="9fd82-187">Para `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="9fd82-187">For `Import-Module`:</span></span>

```azurepowershell-interactive
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="9fd82-188">Deve ser alterado para:</span><span class="sxs-lookup"><span data-stu-id="9fd82-188">Should be changed to:</span></span>

```azurepowershell-interactive
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="9fd82-189">Migrar Invocações de Cmdlets Completamente Qualificados</span><span class="sxs-lookup"><span data-stu-id="9fd82-189">Migrating Fully-Qualified Cmdlet Invocations</span></span>

<span data-ttu-id="9fd82-190">Os scripts que utilizam invocações de cmdlets qualificados por módulo, como:</span><span class="sxs-lookup"><span data-stu-id="9fd82-190">Scripts that use module-qualified cmdlet invocations, such as:</span></span>

```azurepowershell-interactive
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="9fd82-191">Têm de ser alterados de modo a utilizarem os novos nomes de módulos e cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9fd82-191">Must be changed to use the new module and cmdlet names:</span></span>

```azurepowershell-interactive
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="9fd82-192">Migrar dependências de manifestos de módulos</span><span class="sxs-lookup"><span data-stu-id="9fd82-192">Migrating module manifest dependencies</span></span>

<span data-ttu-id="9fd82-193">Os módulos que expressam dependências nos módulos do AzureRM através de um ficheiro (.psd1) de manifesto de módulo terão de atualizar os nomes de módulos na respetiva secção `RequiredModules`:</span><span class="sxs-lookup"><span data-stu-id="9fd82-193">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their `RequiredModules` section:</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="9fd82-194">Tem de ser alterado para:</span><span class="sxs-lookup"><span data-stu-id="9fd82-194">Must be changed to:</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="9fd82-195">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="9fd82-195">Removed modules</span></span>

<span data-ttu-id="9fd82-196">Os módulos seguintes foram removidos:</span><span class="sxs-lookup"><span data-stu-id="9fd82-196">The following modules have been removed:</span></span>

- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="9fd82-197">As ferramentas para estes serviços já não são suportadas ativamente.</span><span class="sxs-lookup"><span data-stu-id="9fd82-197">The tools for these services are no longer actively supported.</span></span>  <span data-ttu-id="9fd82-198">Os clientes são incentivados a mudar para serviços alternativos assim que for possível.</span><span class="sxs-lookup"><span data-stu-id="9fd82-198">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="9fd82-199">Windows PowerShell 5.1 e .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="9fd82-199">Windows PowerShell 5.1 and .NET 4.7.2</span></span>

<span data-ttu-id="9fd82-200">Para utilizar o Az com o PowerShell 5.1 para Windows, tem de instalar o .NET Framework 4.7.2.</span><span class="sxs-lookup"><span data-stu-id="9fd82-200">Using Az with PowerShell 5.1 for Windows requires the installation of .NET Framework 4.7.2.</span></span> <span data-ttu-id="9fd82-201">A utilização do PowerShell Core 6.x ou posterior não requer o .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="9fd82-201">Using PowerShell Core 6.x or later does not require .NET Framework.</span></span>

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="9fd82-202">Remoção temporária do Início de sessão do utilizador através de PSCredential</span><span class="sxs-lookup"><span data-stu-id="9fd82-202">Temporary removal of User login using PSCredential</span></span>

<span data-ttu-id="9fd82-203">Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a remover temporariamente o início de sessão do utilizador através de PSCredential.</span><span class="sxs-lookup"><span data-stu-id="9fd82-203">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="9fd82-204">Esta capacidade será introduzida novamente na versão de 15/01/2019 para o PowerShell 5.1 para Windows.</span><span class="sxs-lookup"><span data-stu-id="9fd82-204">This capability will be re-introduced in the 1/15/2019 release for PowerShell 5.1 for Windows.</span></span> <span data-ttu-id="9fd82-205">Este assunto é abordado em detalhe [neste debate sobre o problema no GitHub](https://github.com/Azure/azure-powershell/issues/7430).</span><span class="sxs-lookup"><span data-stu-id="9fd82-205">This is discussed in detail in [this GitHub issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="9fd82-206">Início de sessão com o código de dispositivo predefinido em vez da linha de comandos do browser</span><span class="sxs-lookup"><span data-stu-id="9fd82-206">Default device code login instead of web browser prompt</span></span>

<span data-ttu-id="9fd82-207">Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a utilizar o início de sessão de dispositivo como o fluxo de início de sessão predefinido durante o início de sessão interativo.</span><span class="sxs-lookup"><span data-stu-id="9fd82-207">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="9fd82-208">O início de sessão baseado no browser será introduzido novamente para o PowerShell 5.1 para Windows como a predefinição na versão de 15/01/2019.</span><span class="sxs-lookup"><span data-stu-id="9fd82-208">Web browser based login will be re-introduced for PowerShell 5.1 for Windows as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="9fd82-209">Nessa altura, os utilizadores poderão escolher o início de sessão de dispositivo através de um parâmetro de mudança (Switch).</span><span class="sxs-lookup"><span data-stu-id="9fd82-209">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="9fd82-210">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="9fd82-210">Module breaking changes</span></span>

<span data-ttu-id="9fd82-211">Esta secção fornece detalhes sobre alterações interruptivas específicas para cmdlets e módulos individuais.</span><span class="sxs-lookup"><span data-stu-id="9fd82-211">This section details specific breaking changes for individual modules and cmdlets.</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="9fd82-212">Az.ApiManagement (anteriormente AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="9fd82-212">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>

- <span data-ttu-id="9fd82-213">Foram removidos os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9fd82-213">Removed the following cmdlets:</span></span>
  - <span data-ttu-id="9fd82-214">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fd82-214">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="9fd82-215">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9fd82-215">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="9fd82-216">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9fd82-216">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="9fd82-217">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9fd82-217">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="9fd82-218">Em alternativa, utilize o cmdlet **Set-AzApiManagement** para definir estas propriedades</span><span class="sxs-lookup"><span data-stu-id="9fd82-218">Use **Set-AzApiManagement** cmdlet to set these properties instead</span></span>
- <span data-ttu-id="9fd82-219">Foram removidas as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="9fd82-219">Removed the following properties:</span></span>
  - <span data-ttu-id="9fd82-220">As propriedades `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` e `ScmHostnameConfiguration` do tipo `PsApiManagementHostnameConfiguration` foram removidas de `PsApiManagementContext`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-220">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="9fd82-221">Em vez disso, utilize `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` e `ScmCustomHostnameConfiguration` do tipo `PsApiManagementCustomHostNameConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-221">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="9fd82-222">A propriedade `StaticIPs` foi removida de PsApiManagementContext.</span><span class="sxs-lookup"><span data-stu-id="9fd82-222">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="9fd82-223">A propriedade foi dividida em `PublicIPAddresses` e `PrivateIPAddresses`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-223">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="9fd82-224">A propriedade necessária `Location` foi removida do cmdlet New-AzureApiManagementVirtualNetwork.</span><span class="sxs-lookup"><span data-stu-id="9fd82-224">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="9fd82-225">Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="9fd82-225">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>

- <span data-ttu-id="9fd82-226">O parâmetro `InvoiceName` foi removido do cmdlet `Get-AzConsumptionUsageDetail`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-226">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="9fd82-227">Os scripts terão de utilizar outros parâmetros de identidade para a faturação.</span><span class="sxs-lookup"><span data-stu-id="9fd82-227">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="9fd82-228">Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="9fd82-228">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>

- <span data-ttu-id="9fd82-229">O conjunto de parâmetros `GetSkusWithAccountParamSetName` foi removido do cmdlet `Get-AzCognitiveServicesAccountSkus`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-229">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="9fd82-230">Tem de obter os Skus através do Tipo de Conta e da Localização, em vez de utilizar ResourceGroupName e o Nome da Conta.</span><span class="sxs-lookup"><span data-stu-id="9fd82-230">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="9fd82-231">Az.Compute (anteriormente AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="9fd82-231">Az.Compute (previously AzureRM.Compute)</span></span>

- <span data-ttu-id="9fd82-232">Os `IdentityIds` foram removidos da propriedade `Identity` nos objetos `PSVirtualMachine` e `PSVirtualMachineScaleSet`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9fd82-232">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="9fd82-233">O tipo de propriedade `InstanceView` do objeto `PSVirtualMachineScaleSetVM` foi alterado de `VirtualMachineInstanceView` para `VirtualMachineScaleSetVMInstanceView`</span><span class="sxs-lookup"><span data-stu-id="9fd82-233">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="9fd82-234">As propriedades `AutoOSUpgradePolicy` e `AutomaticOSUpgrade` foram removidas da propriedade `UpgradePolicy`</span><span class="sxs-lookup"><span data-stu-id="9fd82-234">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="9fd82-235">O tipo de propriedade `Sku` no objeto `PSSnapshotUpdate` foi alterado de `DiskSku` para `SnapshotSku`</span><span class="sxs-lookup"><span data-stu-id="9fd82-235">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="9fd82-236">`VmScaleSetVMParameterSet` foi removido do cmdlet `Add-AzVMDataDisk`. Já não pode adicionar um disco de dados individualmente a uma VM de conjunto de dimensionamento (ScaleSet).</span><span class="sxs-lookup"><span data-stu-id="9fd82-236">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you can no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="9fd82-237">Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="9fd82-237">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>

- <span data-ttu-id="9fd82-238">O parâmetro `GatewayName` tornou-se obrigatório no cmdlet `New-AzDataFactoryEncryptValue`</span><span class="sxs-lookup"><span data-stu-id="9fd82-238">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="9fd82-239">O cmdlet `New-AzDataFactoryGatewayKey` foi removido</span><span class="sxs-lookup"><span data-stu-id="9fd82-239">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="9fd82-240">O parâmetro `LinkedServiceName` foi removido do cmdlet `Get-AzDataFactoryV2ActivityRun`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9fd82-240">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="9fd82-241">Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="9fd82-241">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>

- <span data-ttu-id="9fd82-242">Os cmdlets preteridos que se seguem foram removidos: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret` e `Set-AzDataLakeAnalyticsCatalogSecret`</span><span class="sxs-lookup"><span data-stu-id="9fd82-242">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="9fd82-243">Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="9fd82-243">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>

- <span data-ttu-id="9fd82-244">O tipo do parâmetro `Encoding` foi alterado de `FileSystemCmdletProviderEncoding` para `System.Text.Encoding` nos cmdlets que se seguem.</span><span class="sxs-lookup"><span data-stu-id="9fd82-244">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="9fd82-245">Esta alteração remove os valores de codificação `String` e `Oem`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-245">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="9fd82-246">Todos os outros valores de codificação anteriores permanecem.</span><span class="sxs-lookup"><span data-stu-id="9fd82-246">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="9fd82-247">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="9fd82-247">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="9fd82-248">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="9fd82-248">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="9fd82-249">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="9fd82-249">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="9fd82-250">O alias de propriedade preterido `Tags` foi removido dos cmdlets `New-AzDataLakeStoreAccount` e `Set-AzDataLakeStoreAccount`</span><span class="sxs-lookup"><span data-stu-id="9fd82-250">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="9fd82-251">Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9fd82-251">Scripts using</span></span>
  ```azurepowershell-interactive
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="9fd82-252">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9fd82-252">Should be changed to</span></span>
  ```azurepowershell-interactive
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="9fd82-253">As propriedades preteridas `Identity`, `EncryptionState`, `EncryptionProvisioningState`, `EncryptionConfig`, `FirewallState`, `FirewallRules`, `VirtualNetworkRules`, `TrustedIdProviderState`, `TrustedIdProviders`, `DefaultGroup`, `NewTier`, `CurrentTier` e `FirewallAllowAzureIps` foram removidas do objeto `PSDataLakeStoreAccountBasic`.</span><span class="sxs-lookup"><span data-stu-id="9fd82-253">Removed deprecated properties `Identity`, `EncryptionState`, `EncryptionProvisioningState`, `EncryptionConfig`, `FirewallState`, `FirewallRules`, `VirtualNetworkRules`, `TrustedIdProviderState`, `TrustedIdProviders`, `DefaultGroup`, `NewTier`, `CurrentTier`, `FirewallAllowAzureIps` from `PSDataLakeStoreAccountBasic` object.</span></span>  <span data-ttu-id="9fd82-254">Qualquer script que utilize `PSDatalakeStoreAccount` devolvido a partir de `Get-AzDataLakeStoreAccount` não deve fazer referência a essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9fd82-254">Any script that uses the `PSDatalakeStoreAccount` returned from `Get-AzDataLakeStoreAccount` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="9fd82-255">Az.KeyVault (anteriormente AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="9fd82-255">Az.KeyVault (previously AzureRM.KeyVault)</span></span>

- <span data-ttu-id="9fd82-256">A propriedade `PurgeDisabled` foi removida dos objetos `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` e `PSKeyVaultSecretAttributes`. Os scripts devem deixar de fazer referência à propriedade ```PurgeDisabled``` para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9fd82-256">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts should no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="9fd82-257">Az.Media (anteriormente AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="9fd82-257">Az.Media (previously AzureRM.Media)</span></span>

- <span data-ttu-id="9fd82-258">O alias de propriedade preterido `Tags` foi removido do cmdlet `New-AzMediaService`. Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9fd82-258">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```azurepowershell-interactive
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="9fd82-259">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9fd82-259">Should be changed to</span></span>
  ```azurepowershell-interactive
  New-AzMediaService -Tag @{TagName="TagValue"}
  ```

### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="9fd82-260">Az.Monitor (anteriormente AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="9fd82-260">Az.Monitor (previously AzureRM.Insights)</span></span>

- <span data-ttu-id="9fd82-261">Os nomes de parâmetros no plural `Categories` e `Timegrains` foram removidos em prol de nomes de parâmetros no singular do cmdlet `Set-AzDiagnosticSetting`. Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9fd82-261">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```azurepowershell-interactive
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="9fd82-262">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9fd82-262">Should be changed to</span></span>
  ```azurepowershell-interactive
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```

### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="9fd82-263">Az.Network (anteriormente AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="9fd82-263">Az.Network (previously AzureRM.Network)</span></span>

- <span data-ttu-id="9fd82-264">O parâmetro preterido `ResourceId` foi removido do cmdlet `Get-AzServiceEndpointPolicyDefinition`</span><span class="sxs-lookup"><span data-stu-id="9fd82-264">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="9fd82-265">A propriedade preterida `EnableVmProtection` foi removida do objeto `PSVirtualNetwork`</span><span class="sxs-lookup"><span data-stu-id="9fd82-265">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="9fd82-266">O cmdlet preterido `Set-AzVirtualNetworkGatewayVpnClientConfig` foi removido</span><span class="sxs-lookup"><span data-stu-id="9fd82-266">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>

<span data-ttu-id="9fd82-267">Os scripts devem deixar de tomar decisões de processamento com base nos valores destes campos.</span><span class="sxs-lookup"><span data-stu-id="9fd82-267">Scripts should no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="9fd82-268">Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="9fd82-268">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>

- <span data-ttu-id="9fd82-269">O conjunto de parâmetros predefinido para `Get-AzOperationalInsightsDataSource` foi removido e `ByWorkspaceNameByKind` passou a ser o conjunto de parâmetros predefinido</span><span class="sxs-lookup"><span data-stu-id="9fd82-269">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="9fd82-270">Os scripts que listavam origens de dados com</span><span class="sxs-lookup"><span data-stu-id="9fd82-270">Scripts that listed data sources using</span></span>
  ```azurepowershell-interactive
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="9fd82-271">Devem ser alterados para especificar um tipo (Kind)</span><span class="sxs-lookup"><span data-stu-id="9fd82-271">Should be changed to specify a Kind</span></span>
  ```azurepowershell-interactive
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9fd82-272">Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="9fd82-272">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>

- <span data-ttu-id="9fd82-273">O parâmetro `Encryption` foi removido do cmdlet `New/Set-AzRecoveryServicesAsrPolicy`</span><span class="sxs-lookup"><span data-stu-id="9fd82-273">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="9fd82-274">Agora, o parâmetro `TargetStorageAccountName` é obrigatório para os restauros de discos geridos no cmdlet `Restore-AzRecoveryServicesBackupItem`</span><span class="sxs-lookup"><span data-stu-id="9fd82-274">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="9fd82-275">Os parâmetros `StorageAccountName` e `StorageAccountResourceGroupName` foram removidos no cmdlet `Restore-AzRecoveryServicesBackupItem`</span><span class="sxs-lookup"><span data-stu-id="9fd82-275">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="9fd82-276">O parâmetro `Name` foi removido no cmdlet `Get-AzRecoveryServicesBackupContainer`</span><span class="sxs-lookup"><span data-stu-id="9fd82-276">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="9fd82-277">Az.Resources (anteriormente AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="9fd82-277">Az.Resources (previously AzureRM.Resources)</span></span>

- <span data-ttu-id="9fd82-278">O parâmetro `Sku` foi removido do cmdlet `New/Set-AzPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="9fd82-278">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="9fd82-279">O parâmetro `Password` foi removido dos cmdlets `New-AzADServicePrincipal` e `New-AzADSpCredential`. As palavras-passe são geradas automaticamente e o scripts que forneciam a palavra-passe:</span><span class="sxs-lookup"><span data-stu-id="9fd82-279">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>

  ```azurepowershell-interactive
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="9fd82-280">Devem ser alterados de modo a obterem a palavra-passe a partir da saída:</span><span class="sxs-lookup"><span data-stu-id="9fd82-280">Should be changed to retrieve the password from the output:</span></span>

  ```azurepowershell-interactive
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="9fd82-281">Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="9fd82-281">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>

- <span data-ttu-id="9fd82-282">Foram alterados os seguintes tipos de retorno de cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9fd82-282">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="9fd82-283">A propriedade `ServiceTypeHealthPolicies` do tipo `ApplicationHealthPolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9fd82-283">The property `ServiceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="9fd82-284">A propriedade `ApplicationHealthPolicies` do tipo `ClusterUpgradeDeltaHealthPolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9fd82-284">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="9fd82-285">A propriedade `OverrideUserUpgradePolicy` do tipo `ClusterUpgradePolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9fd82-285">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="9fd82-286">Estas alterações afetam os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9fd82-286">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="9fd82-287">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="9fd82-287">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="9fd82-288">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="9fd82-288">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="9fd82-289">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="9fd82-289">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="9fd82-290">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="9fd82-290">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="9fd82-291">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="9fd82-291">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="9fd82-292">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="9fd82-292">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="9fd82-293">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="9fd82-293">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="9fd82-294">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="9fd82-294">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="9fd82-295">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="9fd82-295">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="9fd82-296">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="9fd82-296">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="9fd82-297">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="9fd82-297">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="9fd82-298">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="9fd82-298">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="9fd82-299">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="9fd82-299">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="9fd82-300">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="9fd82-300">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="9fd82-301">Az.Sql (anteriormente AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="9fd82-301">Az.Sql (previously AzureRM.Sql)</span></span>

- <span data-ttu-id="9fd82-302">Os parâmetros `State` e `ResourceId` foram removidos do cmdlet `Set-AzSqlDatabaseBackupLongTermRetentionPolicy`</span><span class="sxs-lookup"><span data-stu-id="9fd82-302">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="9fd82-303">Foram removidos os seguintes cmdlets preteridos: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing` e `Remove-AzSqlServerAuditing`</span><span class="sxs-lookup"><span data-stu-id="9fd82-303">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="9fd82-304">O parâmetro preterido `Current` foi removido do cmdlet `Get-AzSqlDatabaseBackupLongTermRetentionPolicy`</span><span class="sxs-lookup"><span data-stu-id="9fd82-304">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="9fd82-305">O parâmetro preterido `DatabaseName` foi removido do cmdlet `Get-AzSqlServerServiceObjective`</span><span class="sxs-lookup"><span data-stu-id="9fd82-305">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="9fd82-306">O parâmetro preterido `PrivilegedLogin` foi removido do cmdlet `Set-AzSqlDatabaseDataMaskingPolicy`</span><span class="sxs-lookup"><span data-stu-id="9fd82-306">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="9fd82-307">Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="9fd82-307">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>

- <span data-ttu-id="9fd82-308">Para suportar a criação de um contexto de armazenamento de Oauth com apenas o nome da conta de armazenamento, o conjunto de parâmetros predefinido foi alterado para `OAuthParameterSet`</span><span class="sxs-lookup"><span data-stu-id="9fd82-308">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="9fd82-309">Exemplo: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="9fd82-309">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="9fd82-310">O parâmetro `Location` tornou-se obrigatório no cmdlet `Get-AzStorageUsage`</span><span class="sxs-lookup"><span data-stu-id="9fd82-310">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="9fd82-311">Os métodos da API de Armazenamento utilizam agora o Padrão Assíncrono Baseado em Tarefas (TAP), em vez de chamadas síncronas à API.</span><span class="sxs-lookup"><span data-stu-id="9fd82-311">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span> <span data-ttu-id="9fd82-312">Os exemplos seguintes demonstram os novos comandos assíncronos:</span><span class="sxs-lookup"><span data-stu-id="9fd82-312">The following examples demonstrate the new asynchronous commands:</span></span>

#### <a name="blob-snapshot"></a><span data-ttu-id="9fd82-313">Instantâneo do Blob</span><span class="sxs-lookup"><span data-stu-id="9fd82-313">Blob Snapshot</span></span>

<span data-ttu-id="9fd82-314">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9fd82-314">AzureRM:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

<span data-ttu-id="9fd82-315">Az:</span><span class="sxs-lookup"><span data-stu-id="9fd82-315">Az:</span></span>

```azurepowershell-interactive
$b = Get-AzStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="share-snapshot"></a><span data-ttu-id="9fd82-316">Instantâneo da Partilha</span><span class="sxs-lookup"><span data-stu-id="9fd82-316">Share Snapshot</span></span>

<span data-ttu-id="9fd82-317">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9fd82-317">AzureRM:</span></span>

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```

<span data-ttu-id="9fd82-318">Az:</span><span class="sxs-lookup"><span data-stu-id="9fd82-318">Az:</span></span>

```azurepowershell-interactive
$Share = Get-AzStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="undelete-soft-deleted-blob"></a><span data-ttu-id="9fd82-319">Anular eliminação do blob eliminado de forma recuperável</span><span class="sxs-lookup"><span data-stu-id="9fd82-319">Undelete soft-deleted blob</span></span>

<span data-ttu-id="9fd82-320">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9fd82-320">AzureRM:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```

<span data-ttu-id="9fd82-321">Az:</span><span class="sxs-lookup"><span data-stu-id="9fd82-321">Az:</span></span>

```azurepowershell-interactive
$b = Get-AzStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="set-blob-tier"></a><span data-ttu-id="9fd82-322">Definir Camada de Blob</span><span class="sxs-lookup"><span data-stu-id="9fd82-322">Set Blob Tier</span></span>

<span data-ttu-id="9fd82-323">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9fd82-323">AzureRM:</span></span>

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

<span data-ttu-id="9fd82-324">Az:</span><span class="sxs-lookup"><span data-stu-id="9fd82-324">Az:</span></span>

```azurepowershell-interactive
$blockBlob = Get-AzStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="9fd82-325">Az.Websites (anteriormente AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="9fd82-325">Az.Websites (previously AzureRM.Websites)</span></span>

- <span data-ttu-id="9fd82-326">As propriedades preteridas foram removidas dos objetos `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` e `PSSite`</span><span class="sxs-lookup"><span data-stu-id="9fd82-326">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>
