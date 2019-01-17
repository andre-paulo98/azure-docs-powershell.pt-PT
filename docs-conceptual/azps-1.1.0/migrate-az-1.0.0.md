---
title: Alterações interruptivas do Microsoft Azure PowerShell Az 1.0.0
description: Este guia de migração contém uma lista das alterações interruptivas realizadas no Azure PowerShell no lançamento da versão do Az 1.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/14/2018
ms.openlocfilehash: be3e19dc4b689adbc63b933dd9f3454122d5344a
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342213"
---
# <a name="migration-guide-for-az-100"></a><span data-ttu-id="9176c-103">Guia de migração para o Az 1.0.0</span><span class="sxs-lookup"><span data-stu-id="9176c-103">Migration Guide for Az 1.0.0</span></span>

<span data-ttu-id="9176c-104">Este documento descreve as alterações realizadas entre as versões de 6.x do AzureRM e a versão do Az 1.0.0.</span><span class="sxs-lookup"><span data-stu-id="9176c-104">This document describes the changes between the 6.x versions of AzureRM and Az version 1.0.0.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="9176c-105">Índice</span><span class="sxs-lookup"><span data-stu-id="9176c-105">Table of Contents</span></span>
- [<span data-ttu-id="9176c-106">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="9176c-106">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="9176c-107">Alterações do Prefixo de Nomes de Cmdlet</span><span class="sxs-lookup"><span data-stu-id="9176c-107">Cmdlet Noun Prefix Changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="9176c-108">Alterações de Nomes de Módulos</span><span class="sxs-lookup"><span data-stu-id="9176c-108">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="9176c-109">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="9176c-109">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="9176c-110">Windows PowerShell 5.1 e .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="9176c-110">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="9176c-111">Remoção temporária do Início de sessão do utilizador através de PSCredential</span><span class="sxs-lookup"><span data-stu-id="9176c-111">Temporary removal of User login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="9176c-112">Início de sessão com o Código de Dispositivo Predefinido em vez da linha de comandos do Browser</span><span class="sxs-lookup"><span data-stu-id="9176c-112">Default Device Code login instead of Web Browser prompt</span></span>](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="9176c-113">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="9176c-113">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="9176c-114">Az.ApiManagement (anteriormente AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="9176c-114">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="9176c-115">Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="9176c-115">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="9176c-116">Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="9176c-116">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="9176c-117">Az.Compute (anteriormente AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="9176c-117">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="9176c-118">Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="9176c-118">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="9176c-119">Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="9176c-119">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="9176c-120">Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="9176c-120">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="9176c-121">Az.KeyVault (anteriormente AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="9176c-121">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="9176c-122">Az.Media (anteriormente AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="9176c-122">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="9176c-123">Az.Monitor (anteriormente AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="9176c-123">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="9176c-124">Az.Network (anteriormente AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="9176c-124">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="9176c-125">Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="9176c-125">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="9176c-126">Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="9176c-126">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="9176c-127">Az.Resources (anteriormente AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="9176c-127">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="9176c-128">Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="9176c-128">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="9176c-129">Az.Sql (anteriormente AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="9176c-129">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="9176c-130">Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="9176c-130">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="9176c-131">Az.Websites (anteriormente AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="9176c-131">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="9176c-132">Alterações interruptivas gerais</span><span class="sxs-lookup"><span data-stu-id="9176c-132">General breaking changes</span></span>
### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="9176c-133">Alterações do Prefixo de Nomes de Cmdlet</span><span class="sxs-lookup"><span data-stu-id="9176c-133">Cmdlet Noun Prefix Changes</span></span>
<span data-ttu-id="9176c-134">No AzureRM, os cmdlets utilizavam "AzureRM" ou "Azure" como prefixo de nome.</span><span class="sxs-lookup"><span data-stu-id="9176c-134">In AzureRM, cmdlets used either 'AzureRM' or 'Azure' as a noun prefix.</span></span>  <span data-ttu-id="9176c-135">O Az simplifica e normaliza os nomes de cmdlet, para que todos os cmdlets utilizem "Az" como prefixo de nomes de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9176c-135">Az simplifies and normalizes cmndlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="9176c-136">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9176c-136">For example:</span></span>
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="9176c-137">Foi alterado para</span><span class="sxs-lookup"><span data-stu-id="9176c-137">Have changed to</span></span>
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="9176c-138">Para simplificar a transição para estes novos nomes de cmdlet, o Az apresenta dois novos cmdlets: ```Enable-AzureRmAlias``` e ```Disable-AzureRmAlias```.</span><span class="sxs-lookup"><span data-stu-id="9176c-138">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, ```Enable-AzureRmAlias``` and ```Disable-AzureRmAlias```.</span></span>  <span data-ttu-id="9176c-139">```Enable-AzureRmAlias``` cria aliases a partir dos nomes de cmdlet mais antigos no AzureRM e transforma-os em nomes de cmdlet do Az mais recentes.</span><span class="sxs-lookup"><span data-stu-id="9176c-139">```Enable-AzureRmAlias``` creates aliases from the older cmdlet names in AzureRM to the newer Az cmdlet names.</span></span>  <span data-ttu-id="9176c-140">O cmdlet permite criar aliases na sessão atual, ou em todas as sessões, ao alterar o seu perfil de utilizador ou de computador.</span><span class="sxs-lookup"><span data-stu-id="9176c-140">The cmdlet allows creating aliases in the current session, or across all sessions by changing your user or machine profile.</span></span> 

<span data-ttu-id="9176c-141">Por exemplo, o seguinte script no AzureRM:</span><span class="sxs-lookup"><span data-stu-id="9176c-141">For example, the following script in AzureRM:</span></span>
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9176c-142">Pode ser executado com alterações mínimas com ```Enable-AzureRmAlias```:</span><span class="sxs-lookup"><span data-stu-id="9176c-142">Could be run with minimal changes using ```Enable-AzureRmAlias```:</span></span>
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9176c-143">A utilização de ```Enable-AzureRmAlias -Scope CurrentUser``` permite empregar os aliases em todas as sessões do Powershell que forem abertas, para que, após a execução deste cmdlet, não seja necessário alterar um script deste tipo:</span><span class="sxs-lookup"><span data-stu-id="9176c-143">Running ```Enable-AzureRmAlias -Scope CurrentUser``` will enable the aliases for all powershell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="9176c-144">Para obter detalhes completos sobre a utilização de cmdlets do alias, execute ```Get-Help -Online Enable-AzureRmAlias``` a partir da linha de comandos do Powershell.</span><span class="sxs-lookup"><span data-stu-id="9176c-144">For complete details on the usage of the alias cmdlets, execute ```Get-Help -Online Enable-AzureRmAlias``` from the powershell prompt.</span></span>

<span data-ttu-id="9176c-145">```Disable-AzureRmAlias``` remove os aliases de cmdlet do AzureRM criados por ```Enable-AzureRmAlias```.</span><span class="sxs-lookup"><span data-stu-id="9176c-145">```Disable-AzureRmAlias``` removes AzureRM cmdlet aliases created by ```Enable-AzureRmAlias```.</span></span>  <span data-ttu-id="9176c-146">Para obter detalhes completos, execute ```Get-Help -Online Disable-AzureRmAlias``` a partir da linha de comandos do Powershell.</span><span class="sxs-lookup"><span data-stu-id="9176c-146">For complete details, execute ```Get-Help -Online Disable-AzureRmAlias``` from the powershell prompt.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="9176c-147">Alterações de Nomes de Módulos</span><span class="sxs-lookup"><span data-stu-id="9176c-147">Module Name Changes</span></span>
- <span data-ttu-id="9176c-148">Os nomes de módulos foram alterados de `AzureRM.*` para `Az.*`, exceto para os seguintes módulos:</span><span class="sxs-lookup"><span data-stu-id="9176c-148">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>
```
AzureRM.Profile                       -> Az.Accounts
Azure.AnalysisServices                -> Az.AnalysisServices
AzureRM.Consumption                   -> Az.Billing
AzureRM.UsageAggregates               -> Az.Billing
AzureRM.DataFactories                 -> Az.DataFactory
AzureRM.DataFactoryV2                 -> Az.DataFactory
AzureRM.MachineLearningCompute        -> Az.MachineLearning
AzureRM.Insights                      -> Az.Monitor
AzureRM.RecoveryServices.Backup       -> Az.RecoveryServices
AzureRM.RecoveryServices.SiteRecovery -> Az.RecoveryServices
AzureRM.Tags                          -> Az.Resources
Azure.Storage                         -> Az.Storage
```

<span data-ttu-id="9176c-149">As alterações realizadas ao nível dos nomes de módulos significam que qualquer script que utilizar ```#Requires``` ou ```Import-Module``` para carregar módulos específicos terá de ser alterado de modo a utilizar o novo módulo.</span><span class="sxs-lookup"><span data-stu-id="9176c-149">The changes in module names mean that any script that uses ```#Requires``` or ```Import-Module``` to load specific modules will need to be changed to use the new module instead.</span></span>

#### <a name="migrating-requires-statements"></a><span data-ttu-id="9176c-150">Migrar Declarações #Requires</span><span class="sxs-lookup"><span data-stu-id="9176c-150">Migrating #Requires Statements</span></span>
<span data-ttu-id="9176c-151">Os scripts que utilizam #Requires para declarar uma dependência nos módulos do AzureRM devem ser atualizados de modo a utilizarem os novos nomes de módulos</span><span class="sxs-lookup"><span data-stu-id="9176c-151">Scripts that use #Requires to declare a dependency on AzureRM modules should be updated to use the new module names</span></span>
```powershell
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="9176c-152">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9176c-152">Should be changed to</span></span>
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a><span data-ttu-id="9176c-153">Migrar Declarações Import-Module</span><span class="sxs-lookup"><span data-stu-id="9176c-153">Migrating Import-Module Statements</span></span>
<span data-ttu-id="9176c-154">Os scripts que utilizam ```Import-Module``` para carregar módulos do AzureRM têm de ser atualizados de modo a refletirem os novos nomes de módulos.</span><span class="sxs-lookup"><span data-stu-id="9176c-154">Scripts that use ```Import-Module``` to load AzureRM modules will need to be updated to reflect the new module names.</span></span>
```powershell
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="9176c-155">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9176c-155">Should be changed to</span></span>
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="9176c-156">Migrar Invocações de Cmdlets Completamente Qualificados</span><span class="sxs-lookup"><span data-stu-id="9176c-156">Migrating Fully-Qualified Cmdlet Invocations</span></span>
<span data-ttu-id="9176c-157">Os scripts que utilizam invocações de cmdlets qualificados por módulo, como</span><span class="sxs-lookup"><span data-stu-id="9176c-157">Scripts that use module-qualified cmdlet invocations, like</span></span>
```powershell
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="9176c-158">Devem ser alterados de modo a utilizarem os novos nomes de módulos e cmdlets</span><span class="sxs-lookup"><span data-stu-id="9176c-158">Should be changed to use the new module and cmdlet names</span></span>
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="9176c-159">Migrar Dependências de Manifestos de Módulos</span><span class="sxs-lookup"><span data-stu-id="9176c-159">Migrating Module Manifest Dependencies</span></span>
<span data-ttu-id="9176c-160">Os módulos que expressam dependências nos módulos do AzureRM através de um ficheiro (. psd1) de manifesto de módulo terão de atualizar os nomes de módulos na respetiva secção "RequiredModules"</span><span class="sxs-lookup"><span data-stu-id="9176c-160">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their 'RequiredModules' section</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="9176c-161">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9176c-161">Should be changed to</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="9176c-162">Módulos removidos</span><span class="sxs-lookup"><span data-stu-id="9176c-162">Removed modules</span></span>
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="9176c-163">As ferramentas para estes serviços já não são suportadas ativamente.</span><span class="sxs-lookup"><span data-stu-id="9176c-163">The tooling for these services are no longer actively supported.</span></span>  <span data-ttu-id="9176c-164">Os clientes são incentivados a mudar para serviços alternativos assim que for possível.</span><span class="sxs-lookup"><span data-stu-id="9176c-164">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="9176c-165">Windows PowerShell 5.1 e .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="9176c-165">Windows PowerShell 5.1 and .NET 4.7.2</span></span>
- <span data-ttu-id="9176c-166">Para utilizar o Az com o Windows PowerShell 5.1, tem de instalar o .NET 4.7.2.</span><span class="sxs-lookup"><span data-stu-id="9176c-166">Using Az with Windows PowerShell 5.1 requires the installation of .NET 4.7.2.</span></span> <span data-ttu-id="9176c-167">No entanto, para utilizar o Az com o PowerShell Core não é preciso o .NET 4.7.2.</span><span class="sxs-lookup"><span data-stu-id="9176c-167">However, using Az with PowerShell Core does not require .NET 4.7.2.</span></span> 

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="9176c-168">Remoção temporária do Início de sessão do utilizador através de PSCredential</span><span class="sxs-lookup"><span data-stu-id="9176c-168">Temporary removal of User login using PSCredential</span></span>
- <span data-ttu-id="9176c-169">Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a remover temporariamente o início de sessão do utilizador através de PSCredential.</span><span class="sxs-lookup"><span data-stu-id="9176c-169">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="9176c-170">Esta capacidade será introduzida novamente na versão de 15/01/2019 para o Windows PowerShell 5.1.</span><span class="sxs-lookup"><span data-stu-id="9176c-170">This capability will be re-introduced in the 1/15/2019 release for Windows PowerShell 5.1.</span></span> <span data-ttu-id="9176c-171">Este assunto é abordado em detalhe [neste debate sobre o problema](https://github.com/Azure/azure-powershell/issues/7430).</span><span class="sxs-lookup"><span data-stu-id="9176c-171">This is duscussed in detail in [this issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="9176c-172">Início de sessão com o Código de Dispositivo Predefinido em vez da linha de comandos do Browser</span><span class="sxs-lookup"><span data-stu-id="9176c-172">Default Device Code login instead of Web Browser prompt</span></span>
- <span data-ttu-id="9176c-173">Devido a alterações no fluxo de autenticação para o .NET Standard, estamos a utilizar o início de sessão de dispositivo como o fluxo de início de sessão predefinido durante o início de sessão interativo.</span><span class="sxs-lookup"><span data-stu-id="9176c-173">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="9176c-174">O início de sessão baseado no browser será introduzido novamente para o Windows PowerShell 5.1 como a predefinição na versão de 15/01/2019.</span><span class="sxs-lookup"><span data-stu-id="9176c-174">Web browser based login will be re-introduced for Windows PowerShell 5.1 as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="9176c-175">Nessa altura, os utilizadores poderão escolher o início de sessão de dispositivo através de um parâmetro de mudança (Switch).</span><span class="sxs-lookup"><span data-stu-id="9176c-175">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="9176c-176">Alterações interruptivas do módulo</span><span class="sxs-lookup"><span data-stu-id="9176c-176">Module breaking changes</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="9176c-177">Az.ApiManagement (anteriormente AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="9176c-177">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>
- <span data-ttu-id="9176c-178">Os cmdlets que se seguem vão ser removidos:</span><span class="sxs-lookup"><span data-stu-id="9176c-178">Removing the following cmdlets:</span></span>
  - <span data-ttu-id="9176c-179">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9176c-179">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="9176c-180">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9176c-180">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="9176c-181">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9176c-181">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="9176c-182">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9176c-182">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="9176c-183">Em alternativa, utilize o cmdlet **Set-AzApiManagement** para definir estas propriedades</span><span class="sxs-lookup"><span data-stu-id="9176c-183">Use **Set-AzApiManagement** cmdlet to set these properites instead</span></span>
- <span data-ttu-id="9176c-184">As propriedades que se seguem foram removidas</span><span class="sxs-lookup"><span data-stu-id="9176c-184">Following properties were removed</span></span>
  - <span data-ttu-id="9176c-185">As propriedades `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` e `ScmHostnameConfiguration` do tipo `PsApiManagementHostnameConfiguration` foram removidas de `PsApiManagementContext`.</span><span class="sxs-lookup"><span data-stu-id="9176c-185">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="9176c-186">Em vez disso, utilize `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` e `ScmCustomHostnameConfiguration` do tipo `PsApiManagementCustomHostNameConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="9176c-186">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="9176c-187">A propriedade `StaticIPs` foi removida de PsApiManagementContext.</span><span class="sxs-lookup"><span data-stu-id="9176c-187">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="9176c-188">A propriedade foi dividida em `PublicIPAddresses` e `PrivateIPAddresses`.</span><span class="sxs-lookup"><span data-stu-id="9176c-188">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="9176c-189">A propriedade necessária `Location` foi removida do cmdlet New-AzureApiManagementVirtualNetwork.</span><span class="sxs-lookup"><span data-stu-id="9176c-189">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="9176c-190">Az.Billing (anteriormente AzureRM.Billing, AzureRM.Consumption e AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="9176c-190">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>
- <span data-ttu-id="9176c-191">O parâmetro `InvoiceName` foi removido do cmdlet `Get-AzConsumptionUsageDetail`.</span><span class="sxs-lookup"><span data-stu-id="9176c-191">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="9176c-192">Os scripts terão de utilizar outros parâmetros de identidade para a faturação.</span><span class="sxs-lookup"><span data-stu-id="9176c-192">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="9176c-193">Az.CognitiveServices (anteriormente AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="9176c-193">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>
- <span data-ttu-id="9176c-194">O conjunto de parâmetros `GetSkusWithAccountParamSetName` foi removido do cmdlet `Get-AzCognitiveServicesAccountSkus`.</span><span class="sxs-lookup"><span data-stu-id="9176c-194">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="9176c-195">Tem de obter os Skus através do Tipo de Conta e da Localização, em vez de utilizar ResourceGroupName e o Nome da Conta.</span><span class="sxs-lookup"><span data-stu-id="9176c-195">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="9176c-196">Az.Compute (anteriormente AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="9176c-196">Az.Compute (previously AzureRM.Compute)</span></span>
- <span data-ttu-id="9176c-197">Os `IdentityIds` foram removidos da propriedade `Identity` nos objetos `PSVirtualMachine` e `PSVirtualMachineScaleSet`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9176c-197">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="9176c-198">O tipo de propriedade `InstanceView` do objeto `PSVirtualMachineScaleSetVM` foi alterado de `VirtualMachineInstanceView` para `VirtualMachineScaleSetVMInstanceView`</span><span class="sxs-lookup"><span data-stu-id="9176c-198">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="9176c-199">As propriedades `AutoOSUpgradePolicy` e `AutomaticOSUpgrade` foram removidas da propriedade `UpgradePolicy`</span><span class="sxs-lookup"><span data-stu-id="9176c-199">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="9176c-200">O tipo de propriedade `Sku` no objeto `PSSnapshotUpdate` foi alterado de `DiskSku` para `SnapshotSku`</span><span class="sxs-lookup"><span data-stu-id="9176c-200">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="9176c-201">`VmScaleSetVMParameterSet` foi removido do cmdlet `Add-AzVMDataDisk`. Já não pode adicionar um disco de dados individualmente a uma VM de conjunto de dimensionamento (ScaleSet).</span><span class="sxs-lookup"><span data-stu-id="9176c-201">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you cna no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="9176c-202">Az.DataFactory (anteriormente AzureRM.DataFactories e AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="9176c-202">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>
- <span data-ttu-id="9176c-203">O parâmetro `GatewayName` tornou-se obrigatório no cmdlet `New-AzDataFactoryEncryptValue`</span><span class="sxs-lookup"><span data-stu-id="9176c-203">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="9176c-204">O cmdlet `New-AzDataFactoryGatewayKey` foi removido</span><span class="sxs-lookup"><span data-stu-id="9176c-204">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="9176c-205">O parâmetro `LinkedServiceName` foi removido do cmdlet `Get-AzDataFactoryV2ActivityRun`. Os scripts devem deixar de utilizar o valor deste campo para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9176c-205">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="9176c-206">Az.DataLakeAnalytics (anteriormente AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="9176c-206">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>
- <span data-ttu-id="9176c-207">Os cmdlets preteridos que se seguem foram removidos: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret` e `Set-AzDataLakeAnalyticsCatalogSecret`</span><span class="sxs-lookup"><span data-stu-id="9176c-207">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="9176c-208">Az.DataLakeStore (anteriormente AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="9176c-208">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>
- <span data-ttu-id="9176c-209">O tipo do parâmetro `Encoding` foi alterado de `FileSystemCmdletProviderEncoding` para `System.Text.Encoding` nos cmdlets que se seguem.</span><span class="sxs-lookup"><span data-stu-id="9176c-209">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="9176c-210">Esta alteração remove os valores de codificação `String` e `Oem`.</span><span class="sxs-lookup"><span data-stu-id="9176c-210">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="9176c-211">Todos os outros valores de codificação anteriores permanecem.</span><span class="sxs-lookup"><span data-stu-id="9176c-211">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="9176c-212">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="9176c-212">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="9176c-213">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="9176c-213">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="9176c-214">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="9176c-214">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="9176c-215">O alias de propriedade preterido `Tags` foi removido dos cmdlets `New-AzDataLakeStoreAccount` e `Set-AzDataLakeStoreAccount`</span><span class="sxs-lookup"><span data-stu-id="9176c-215">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="9176c-216">Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9176c-216">Scripts using</span></span>
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="9176c-217">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9176c-217">Should be changed to</span></span>
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="9176c-218">As propriedades preteridas ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier``` e ```FirewallAllowAzureIps``` foram removidas do objeto ```PSDataLakeStoreAccountBasic```.</span><span class="sxs-lookup"><span data-stu-id="9176c-218">Removed deprecated properties ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier```, ```FirewallAllowAzureIps``` from ```PSDataLakeStoreAccountBasic``` object.</span></span>  <span data-ttu-id="9176c-219">Qualquer script que utilize ```PSDatalakeStoreAccount``` devolvido a partir de ```Get-AzDataLakeStoreAccount``` não deve fazer referência a essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9176c-219">Any script that uses the ```PSDatalakeStoreAccount``` returned from ```Get-AzDataLakeStoreAccount``` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="9176c-220">Az.KeyVault (anteriormente AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="9176c-220">Az.KeyVault (previously AzureRM.KeyVault)</span></span>
- <span data-ttu-id="9176c-221">A propriedade `PurgeDisabled` foi removida dos objetos `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` e `PSKeyVaultSecretAttributes`. Os scripts devem deixar de fazer referência à propriedade ```PurgeDisabled``` para tomar decisões de processamento.</span><span class="sxs-lookup"><span data-stu-id="9176c-221">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts shoudl no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="9176c-222">Az.Media (anteriormente AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="9176c-222">Az.Media (previously AzureRM.Media)</span></span>
- <span data-ttu-id="9176c-223">O alias de propriedade preterido `Tags` foi removido do cmdlet `New-AzMediaService`. Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9176c-223">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="9176c-224">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9176c-224">Should be changed to</span></span>
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="9176c-225">Az.Monitor (anteriormente AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="9176c-225">Az.Monitor (previously AzureRM.Insights)</span></span>
- <span data-ttu-id="9176c-226">Os nomes de parâmetros no plural `Categories` e `Timegrains` foram removidos em prol de nomes de parâmetros no singular do cmdlet `Set-AzDiagnosticSetting`. Os scripts que utilizam</span><span class="sxs-lookup"><span data-stu-id="9176c-226">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="9176c-227">Devem ser alterados para</span><span class="sxs-lookup"><span data-stu-id="9176c-227">Should be changed to</span></span>
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="9176c-228">Az.Network (anteriormente AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="9176c-228">Az.Network (previously AzureRM.Network)</span></span>
- <span data-ttu-id="9176c-229">O parâmetro preterido `ResourceId` foi removido do cmdlet `Get-AzServiceEndpointPolicyDefinition`</span><span class="sxs-lookup"><span data-stu-id="9176c-229">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="9176c-230">A propriedade preterida `EnableVmProtection` foi removida do objeto `PSVirtualNetwork`</span><span class="sxs-lookup"><span data-stu-id="9176c-230">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="9176c-231">O cmdlet preterido `Set-AzVirtualNetworkGatewayVpnClientConfig` foi removido</span><span class="sxs-lookup"><span data-stu-id="9176c-231">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>
  
<span data-ttu-id="9176c-232">Os scripts devem deixar de tomar decisões de processamento com base nos valores destes campos.</span><span class="sxs-lookup"><span data-stu-id="9176c-232">Scripts shoudl no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="9176c-233">Az.OperationalInsights (anteriormente AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="9176c-233">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>
- <span data-ttu-id="9176c-234">O conjunto de parâmetros predefinido para `Get-AzOperationalInsightsDataSource` foi removido e `ByWorkspaceNameByKind` passou a ser o conjunto de parâmetros predefinido</span><span class="sxs-lookup"><span data-stu-id="9176c-234">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="9176c-235">Os scripts que listavam origens de dados com</span><span class="sxs-lookup"><span data-stu-id="9176c-235">Scripts that listed data sources using</span></span>
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="9176c-236">Devem ser alterados para especificar um tipo (Kind)</span><span class="sxs-lookup"><span data-stu-id="9176c-236">Should be changed to specify a Kind</span></span>
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9176c-237">Az.RecoveryServices (anteriormente AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup e AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="9176c-237">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>
- <span data-ttu-id="9176c-238">O parâmetro `Encryption` foi removido do cmdlet `New/Set-AzRecoveryServicesAsrPolicy`</span><span class="sxs-lookup"><span data-stu-id="9176c-238">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="9176c-239">Agora, o parâmetro `TargetStorageAccountName` é obrigatório para os restauros de discos geridos no cmdlet `Restore-AzRecoveryServicesBackupItem`</span><span class="sxs-lookup"><span data-stu-id="9176c-239">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="9176c-240">Os parâmetros `StorageAccountName` e `StorageAccountResourceGroupName` foram removidos no cmdlet `Restore-AzRecoveryServicesBackupItem`</span><span class="sxs-lookup"><span data-stu-id="9176c-240">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="9176c-241">O parâmetro `Name` foi removido no cmdlet `Get-AzRecoveryServicesBackupContainer`</span><span class="sxs-lookup"><span data-stu-id="9176c-241">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="9176c-242">Az.Resources (anteriormente AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="9176c-242">Az.Resources (previously AzureRM.Resources)</span></span>
- <span data-ttu-id="9176c-243">O parâmetro `Sku` foi removido do cmdlet `New/Set-AzPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="9176c-243">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="9176c-244">O parâmetro `Password` foi removido dos cmdlets `New-AzADServicePrincipal` e `New-AzADSpCredential`. As palavras-passe são geradas automaticamente e o scripts que forneciam a palavra-passe:</span><span class="sxs-lookup"><span data-stu-id="9176c-244">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="9176c-245">Devem ser alterados de modo a obterem a palavra-passe a partir da saída:</span><span class="sxs-lookup"><span data-stu-id="9176c-245">Should be changed to retriedve the password from the output:</span></span>
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="9176c-246">Az.ServiceFabric (anteriormente AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="9176c-246">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>
- <span data-ttu-id="9176c-247">Foram alterados os seguintes tipos de retorno de cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9176c-247">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="9176c-248">A propriedade `SerivceTypeHealthPolicies` do tipo `ApplicationHealthPolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9176c-248">The property `SerivceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="9176c-249">A propriedade `ApplicationHealthPolicies` do tipo `ClusterUpgradeDeltaHealthPolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9176c-249">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="9176c-250">A propriedade `OverrideUserUpgradePolicy` do tipo `ClusterUpgradePolicy` foi removida.</span><span class="sxs-lookup"><span data-stu-id="9176c-250">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="9176c-251">Estas alterações afetam os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9176c-251">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="9176c-252">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="9176c-252">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="9176c-253">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="9176c-253">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="9176c-254">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="9176c-254">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="9176c-255">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="9176c-255">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="9176c-256">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="9176c-256">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="9176c-257">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="9176c-257">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="9176c-258">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="9176c-258">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="9176c-259">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="9176c-259">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="9176c-260">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="9176c-260">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="9176c-261">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="9176c-261">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="9176c-262">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="9176c-262">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="9176c-263">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="9176c-263">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="9176c-264">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="9176c-264">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="9176c-265">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="9176c-265">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="9176c-266">Az.Sql (anteriormente AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="9176c-266">Az.Sql (previously AzureRM.Sql)</span></span>
- <span data-ttu-id="9176c-267">Os parâmetros `State` e `ResourceId` foram removidos do cmdlet `Set-AzSqlDatabaseBackupLongTermRetentionPolicy`</span><span class="sxs-lookup"><span data-stu-id="9176c-267">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="9176c-268">Foram removidos os seguintes cmdlets preteridos: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing` e `Remove-AzSqlServerAuditing`</span><span class="sxs-lookup"><span data-stu-id="9176c-268">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="9176c-269">O parâmetro preterido `Current` foi removido do cmdlet `Get-AzSqlDatabaseBackupLongTermRetentionPolicy`</span><span class="sxs-lookup"><span data-stu-id="9176c-269">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="9176c-270">O parâmetro preterido `DatabaseName` foi removido do cmdlet `Get-AzSqlServerServiceObjective`</span><span class="sxs-lookup"><span data-stu-id="9176c-270">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="9176c-271">O parâmetro preterido `PrivilegedLogin` foi removido do cmdlet `Set-AzSqlDatabaseDataMaskingPolicy`</span><span class="sxs-lookup"><span data-stu-id="9176c-271">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="9176c-272">Az.Storage (anteriormente Azure.Storage e AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="9176c-272">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>
- <span data-ttu-id="9176c-273">Para suportar a criação de um contexto de armazenamento de Oauth com apenas o nome da conta de armazenamento, o conjunto de parâmetros predefinido foi alterado para `OAuthParameterSet`</span><span class="sxs-lookup"><span data-stu-id="9176c-273">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="9176c-274">Exemplo: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="9176c-274">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="9176c-275">O parâmetro `Location` tornou-se obrigatório no cmdlet `Get-AzStorageUsage`</span><span class="sxs-lookup"><span data-stu-id="9176c-275">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="9176c-276">Os métodos da API de Armazenamento utilizam agora o Padrão Assíncrono Baseado em Tarefas (TAP), em vez de chamadas síncronas à API.</span><span class="sxs-lookup"><span data-stu-id="9176c-276">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span>
#### <a name="1-blob-snapshot"></a><span data-ttu-id="9176c-277">1. Instantâneo do Blob</span><span class="sxs-lookup"><span data-stu-id="9176c-277">1. Blob Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="9176c-278">Antes:</span><span class="sxs-lookup"><span data-stu-id="9176c-278">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a><span data-ttu-id="9176c-279">Depois:</span><span class="sxs-lookup"><span data-stu-id="9176c-279">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a><span data-ttu-id="9176c-280">2. Instantâneo da Partilha</span><span class="sxs-lookup"><span data-stu-id="9176c-280">2. Share Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="9176c-281">Antes:</span><span class="sxs-lookup"><span data-stu-id="9176c-281">Before:</span></span>
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a><span data-ttu-id="9176c-282">Depois:</span><span class="sxs-lookup"><span data-stu-id="9176c-282">After:</span></span>
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a><span data-ttu-id="9176c-283">3. Anular a eliminação de um blob de eliminação de forma recuperável</span><span class="sxs-lookup"><span data-stu-id="9176c-283">3. Undelete a soft delete blob</span></span>
##### <a name="before"></a><span data-ttu-id="9176c-284">Antes:</span><span class="sxs-lookup"><span data-stu-id="9176c-284">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a><span data-ttu-id="9176c-285">Depois:</span><span class="sxs-lookup"><span data-stu-id="9176c-285">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a><span data-ttu-id="9176c-286">4. Definir Camada de Blob</span><span class="sxs-lookup"><span data-stu-id="9176c-286">4. Set Blob Tier</span></span>
##### <a name="before"></a><span data-ttu-id="9176c-287">Antes:</span><span class="sxs-lookup"><span data-stu-id="9176c-287">Before:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a><span data-ttu-id="9176c-288">Depois:</span><span class="sxs-lookup"><span data-stu-id="9176c-288">After:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="9176c-289">Az.Websites (anteriormente AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="9176c-289">Az.Websites (previously AzureRM.Websites)</span></span>
- <span data-ttu-id="9176c-290">As propriedades preteridas foram removidas dos objetos `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` e `PSSite`</span><span class="sxs-lookup"><span data-stu-id="9176c-290">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>