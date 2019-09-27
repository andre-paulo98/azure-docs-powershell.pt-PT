---
title: Apresentação do módulo do Azure PowerShell Az
description: Apresentação do novo módulo do Azure PowerShell Az, a substituição do módulo AzureRM.
ms.date: 05/10/2019
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 21d41b6e14d1b39a78e40daee74b80de3a80c2a0
ms.sourcegitcommit: 92722d603b60dc769660e7517da60110133d9959
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/24/2019
ms.locfileid: "71226427"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="cc659-103">Apresentação do novo módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="cc659-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="cc659-104">A partir de dezembro de 2018, o módulo do Az do Azure PowerShell passa a ser uma versão de disponibilidade geral e é agora o módulo indicado do PowerShell para interagir com o Azure.</span><span class="sxs-lookup"><span data-stu-id="cc659-104">Starting in December 2018, the Azure PowerShell Az module is in general release and now the intended PowerShell module for interacting with Azure.</span></span> <span data-ttu-id="cc659-105">O Az oferece comandos mais curtos, maior estabilidade e suporte para várias plataformas.</span><span class="sxs-lookup"><span data-stu-id="cc659-105">Az offers shorter commands, improved stability, and cross-platform support.</span></span> <span data-ttu-id="cc659-106">O Az também tem paridade de funcionalidades com o AzureRM, o que lhe oferece um caminho de migração fácil.</span><span class="sxs-lookup"><span data-stu-id="cc659-106">Az also has feature parity with AzureRM, giving you an easy migration path.</span></span>

<span data-ttu-id="cc659-107">Com o módulo Az, o Azure PowerShell passa a ser compatível com o PowerShell 5.1 no Windows e com o PowerShell Core 6.x e versões posteriores em todas as plataformas suportadas, incluindo Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="cc659-107">With the Az module, Azure PowerShell is now compatible with PowerShell 5.1 on Windows and PowerShell Core 6.x and later on all supported platforms - including Windows, macOS, and Linux.</span></span>

<span data-ttu-id="cc659-108">O Az é um módulo novo, pelo que a versão foi reposta para 1.0.0.</span><span class="sxs-lookup"><span data-stu-id="cc659-108">Az is a new module, so the version has been reset to 1.0.0.</span></span>

## <a name="why-a-new-module"></a><span data-ttu-id="cc659-109">Por quê um novo módulo?</span><span class="sxs-lookup"><span data-stu-id="cc659-109">Why a new module?</span></span>

<span data-ttu-id="cc659-110">As principais atualizações podem ser inconvenientes, pelo que é importante informá-lo das razões que nos levaram a optar por introduzir um novo conjunto de módulos, com novos cmdlets, para interagir com o Azure a partir do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cc659-110">Major updates can be inconvenient, so it's important that we let you know why the decision was made to introduce a new set of modules, with new cmdlets, for interacting with Azure from PowerShell.</span></span>

<span data-ttu-id="cc659-111">A alteração mais importante e mais significativa é que o PowerShell tem sido um produto compatível com várias plataformas desde o lançamento do [PowerShell Core 6.x](/powershell/scripting/overview), com base na biblioteca do .NET Standard.</span><span class="sxs-lookup"><span data-stu-id="cc659-111">The biggest and most important change is that PowerShell has been a cross-platform product since the introduction of [PowerShell Core 6.x](/powershell/scripting/overview), based on the .NET Standard library.</span></span>
<span data-ttu-id="cc659-112">Assumimos o compromisso de levar o suporte do Azure a todas as plataformas e, para isso, os módulos do Azure PowerShell tinham de ser atualizados para utilizar o .NET Standard e ser compatíveis com o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="cc659-112">We're committed to bringing Azure support to all platforms, which means that the Azure PowerShell modules needed to be updated to use .NET Standard and be compatible with PowerShell Core.</span></span> <span data-ttu-id="cc659-113">Em vez de introduzirmos alterações complexas ao módulo AzureRM para adicionar este suporte, criámos o módulo Az.</span><span class="sxs-lookup"><span data-stu-id="cc659-113">Rather than taking the existing AzureRM module and introduce complex changes to add this support, the Az module was created.</span></span>

<span data-ttu-id="cc659-114">A criação de um novo módulo também deu aos nossos engenheiros a oportunidade de garantir a consistência da estruturação e da nomenclatura dos cmdlets e módulos.</span><span class="sxs-lookup"><span data-stu-id="cc659-114">Creating a new module also gave our engineers the opportunity to make the design and naming of cmdlets and modules consistent.</span></span> <span data-ttu-id="cc659-115">Agora, todos os módulos começam com o prefixo `Az.` e todos os cmdlets utilizam a forma _Verbo_-`Az`_Substantivo_.</span><span class="sxs-lookup"><span data-stu-id="cc659-115">All modules now start with the `Az.` prefix and cmdlets all use the _Verb_-`Az`_Noun_ form.</span></span> <span data-ttu-id="cc659-116">Anteriormente, os nomes dos cmdlets não só eram mais longos como tinham mais inconsistências.</span><span class="sxs-lookup"><span data-stu-id="cc659-116">Previously, cmdlet names were not only longer, there were inconsistencies in cmdlet names.</span></span>

<span data-ttu-id="cc659-117">O número de módulos também foi reduzido: Alguns módulos que funcionavam com os mesmos serviços foram implementados em conjunto e os cmdlets do plano de gestão e do plano de dados passam todos a estar contidos em módulos únicos relativamente aos seus serviços.</span><span class="sxs-lookup"><span data-stu-id="cc659-117">The number of modules was also reduced: Some modules which worked with the same services have been rolled together, and management plane and data plane cmdlets are now contained all within single modules for their services.</span></span> <span data-ttu-id="cc659-118">Para quem faz a gestão manual das dependências e importações, a tarefa torna-se muito mais simples.</span><span class="sxs-lookup"><span data-stu-id="cc659-118">For those of you who manually manage dependencies and imports, this makes things much simpler.</span></span>

<span data-ttu-id="cc659-119">Ao levar a cabo estas alterações importantes que exigiram a criação de um novo módulo do Azure PowerShell, a equipa assumiu o compromisso de tornar a utilização do Azure com os cmdlets do PowerShell mais fácil do que nunca e em mais plataformas do que alguma vez foi antes possível.</span><span class="sxs-lookup"><span data-stu-id="cc659-119">By making these important changes that required building a new Azure PowerShell module, the team has committed to making it easier than ever, and on more platforms than previously possible, to use Azure with PowerShell cmdlets.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="cc659-120">Atualizar para Az</span><span class="sxs-lookup"><span data-stu-id="cc659-120">Upgrade to Az</span></span>

<span data-ttu-id="cc659-121">Para se manter a par das mais recentes funcionalidades do Azure no PowerShell, deve migrar para o módulo Az assim que for possível.</span><span class="sxs-lookup"><span data-stu-id="cc659-121">To keep up with the latest Azure features in PowerShell, you should migrate to the Az module as soon as possible.</span></span> <span data-ttu-id="cc659-122">Se não estiver pronto para instalar o módulo Az como substituto do AzureRM, tem algumas opções disponíveis para experimentar o Az:</span><span class="sxs-lookup"><span data-stu-id="cc659-122">If you're not ready to install the Az module as a replacement for AzureRM, you have a couple of options available to experiment with Az:</span></span>

* <span data-ttu-id="cc659-123">Utilize um ambiente `PowerShell` com o [Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="cc659-123">Use a `PowerShell` environment with [Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview).</span></span>
  <span data-ttu-id="cc659-124">O Azure Cloud Shell é um ambiente de shell baseado no browser que é fornecido com o módulo Az instalado e com os aliases de compatibilidade `Enable-AzureRM` ativados.</span><span class="sxs-lookup"><span data-stu-id="cc659-124">Azure Cloud Shell is a browser-based shell environment which comes with the Az module installed and `Enable-AzureRM` compatibility aliases enabled.</span></span>
* <span data-ttu-id="cc659-125">Mantenha o módulo AzureRM instalado com o PowerShell 5.1 para Windows, mas instale o módulo Az para o PowerShell Core 6.x ou versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="cc659-125">Keep the AzureRM module installed with PowerShell 5.1 for Windows, but install the Az module for PowerShell Core 6.x or later.</span></span> <span data-ttu-id="cc659-126">O PowerShell 5.1 para Windows e o PowerShell Core utilizam coleções separadas de módulos.</span><span class="sxs-lookup"><span data-stu-id="cc659-126">PowerShell 5.1 for Windows and PowerShell Core use separate collections of modules.</span></span> <span data-ttu-id="cc659-127">Siga as instruções de [instalação do PowerShell Core](/powershell/scripting/install/installing-powershell-core-on-windows) e, em seguida, [instale o módulo Az](install-az-ps.md) a partir de um terminal do PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="cc659-127">Follow the instructions to [install PowerShell Core](/powershell/scripting/install/installing-powershell-core-on-windows) and then [install the Az module](install-az-ps.md) from a PowerShell Core terminal.</span></span>

<span data-ttu-id="cc659-128">Para atualizar a partir de uma instalação existente do AzureRM:</span><span class="sxs-lookup"><span data-stu-id="cc659-128">To upgrade from an existing AzureRM install:</span></span>

1. [<span data-ttu-id="cc659-129">Desinstalar o módulo do Azure PowerShell AzureRM</span><span class="sxs-lookup"><span data-stu-id="cc659-129">Uninstall the Azure PowerShell AzureRM module</span></span>](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
2. [<span data-ttu-id="cc659-130">Instalar o módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="cc659-130">Install the Azure PowerShell Az module</span></span>](install-az-ps.md)
3. <span data-ttu-id="cc659-131">__OPCIONAL__: Ative o modo de compatibilidade para adicionar aliases para cmdlets do AzureRM com [Enable-AzureRMAlias](/powershell/module/az.accounts/enable-azurermalias) enquanto se familiariza com o novo conjunto de comandos.</span><span class="sxs-lookup"><span data-stu-id="cc659-131">__OPTIONAL__: Enable compatibility mode to add aliases for AzureRM cmdlets with [Enable-AzureRMAlias](/powershell/module/az.accounts/enable-azurermalias) while you become familiar with the new command set.</span></span> <span data-ttu-id="cc659-132">Veja a secção seguinte ou [Inicie a migração do AzureRM para o Az](migrate-from-azurerm-to-az.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="cc659-132">See the next section or [Start migration from AzureRM to Az](migrate-from-azurerm-to-az.md) for more details.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="cc659-133">Migrar scripts existentes para o Az</span><span class="sxs-lookup"><span data-stu-id="cc659-133">Migrate existing scripts to Az</span></span>

<span data-ttu-id="cc659-134">Os novos nomes de cmdlet foram criados para serem fáceis de aprender.</span><span class="sxs-lookup"><span data-stu-id="cc659-134">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="cc659-135">Em vez de utilizar `AzureRm` ou `Azure` em nomes de cmdlet, utilize `Az`.</span><span class="sxs-lookup"><span data-stu-id="cc659-135">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="cc659-136">Por exemplo, o comando antigo `New-AzureRMVm` tornou-se `New-AzVm`.</span><span class="sxs-lookup"><span data-stu-id="cc659-136">For example, the old command `New-AzureRMVm` has become `New-AzVm`.</span></span>
<span data-ttu-id="cc659-137">Contudo, a migração exige mais do que apenas se familiarizar com os novos nomes dos cmdlets: Existem módulos com nomes alterados, parâmetros e outras alterações importantes.</span><span class="sxs-lookup"><span data-stu-id="cc659-137">Migration is more than just becoming familiar with the new cmdlet names, though: There are renamed modules, parameters, and other important changes.</span></span>

<span data-ttu-id="cc659-138">Para ajudá-lo no processo de migração do AzureRM para o Az, temos uma série de recursos:</span><span class="sxs-lookup"><span data-stu-id="cc659-138">To help you with the process of migration from AzureRM to Az, we've got a number of resources:</span></span>

* [<span data-ttu-id="cc659-139">Introdução à migração do AzureRM para o Az</span><span class="sxs-lookup"><span data-stu-id="cc659-139">Get started with migration from AzureRM to Az</span></span>](migrate-from-azurerm-to-az.md)
* [<span data-ttu-id="cc659-140">Lista completa das alterações interruptivas do AzureRM para o Az 1.0.0</span><span class="sxs-lookup"><span data-stu-id="cc659-140">Full list of breaking changes from AzureRM to Az 1.0.0</span></span>](migrate-az-1.0.0.md)
* <span data-ttu-id="cc659-141">O cmdlet [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias)</span><span class="sxs-lookup"><span data-stu-id="cc659-141">The [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) cmdlet</span></span>

<span data-ttu-id="cc659-142">O módulo Az tem um modo de compatibilidade para o ajudar a utilizar os scripts existentes enquanto atualiza para a nova sintaxe.</span><span class="sxs-lookup"><span data-stu-id="cc659-142">The Az module has a compatibility mode to help you use existing scripts while you update to the new syntax.</span></span> <span data-ttu-id="cc659-143">O cmdlet [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) ativa um modo de compatibilidade através de aliases, para que possa utilizar scripts existentes com alterações mínimas ao mesmo tempo que faz a migração completa para o Az.</span><span class="sxs-lookup"><span data-stu-id="cc659-143">The [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) cmdlet enables a compatibility mode through aliases, to allow you to use existing scripts with minimal modification while working towards a full migration to Az.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cc659-144">Embora os nomes dos cmdlets tenham aliases, poderá continuar a existir parâmetros novos (ou com nome alterado) ou valores de retorno alterados dos cmdlets do Az.</span><span class="sxs-lookup"><span data-stu-id="cc659-144">Even though the cmdlet names are aliased, there may still be new (or renamed) parameters or changed return values for the Az cmdlets.</span></span> <span data-ttu-id="cc659-145">Não espere que a ativação dos aliases trate da migração por si!</span><span class="sxs-lookup"><span data-stu-id="cc659-145">Don't expect enabling aliases to take care of the migration for you!</span></span> <span data-ttu-id="cc659-146">Veja a [lista completa de alterações interruptivas](migrate-az-1.0.0.md) para saber onde os seus scripts poderão precisar de atualizações.</span><span class="sxs-lookup"><span data-stu-id="cc659-146">See the [full breaking changes list](migrate-az-1.0.0.md) to find where your scripts may require updates.</span></span>

## <a name="continued-support-for-azurerm"></a><span data-ttu-id="cc659-147">Suporte contínuo para o AzureRM</span><span class="sxs-lookup"><span data-stu-id="cc659-147">Continued support for AzureRM</span></span>

<span data-ttu-id="cc659-148">O AzureRM deixará de receber novos cmdlets ou funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="cc659-148">AzureRM will no longer receive new cmdlets or features.</span></span> <span data-ttu-id="cc659-149">No entanto, o módulo do AzureRM ainda é oficialmente mantido e receberá correções de erros até dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="cc659-149">However, the AzureRM module is still officially maintained and will get bug fixes through December 2020.</span></span>