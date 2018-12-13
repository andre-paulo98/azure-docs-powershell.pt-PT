---
title: Apresentação do módulo do Azure PowerShell Az
description: Apresentação do novo módulo do Azure PowerShell Az, a substituição do módulo AzureRM.
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217546"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="fc3a7-103">Apresentação do novo módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="fc3a7-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="fc3a7-104">A partir de novembro de 2018, o módulo do Azure PowerShell `Az` está disponível para pré-visualização pública completa.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-104">Starting in November 2018, the Azure PowerShell `Az` module is available for full public preview.</span></span>
<span data-ttu-id="fc3a7-105">O Az disponibiliza comandos mais curtos, maior estabilidade e suporta Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-105">Az offers shorter commands, improved stability, and supports Windows, macOS, and Linux.</span></span> <span data-ttu-id="fc3a7-106">O Az também oferece paridade de funcionalidades e um caminho de migração fácil a partir do AzureRM.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="fc3a7-107">O Az utiliza a biblioteca .NET Standard, o que significa que é executada no PowerShell 5.x e no PowerShell 6.x.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-107">Az uses the .NET Standard library, which means it runs on PowerShell 5.x and PowerShell 6.x.</span></span>
<span data-ttu-id="fc3a7-108">Dado que o PowerShell 6.x pode ser executado em Linux, macOS e Windows, o Az está disponível para todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-108">Since PowerShell 6.x can run on Linux, macOS, and Windows, that means Az is available for all platforms.</span></span>
<span data-ttu-id="fc3a7-109">A utilização do .NET Standard permite-nos unificar a base de código do Azure PowerShell com o mínimo impacto nos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="fc3a7-110">O Az é um módulo novo, pelo que a versão foi reposta.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-110">Az is a new module, so the version has been reset.</span></span> <span data-ttu-id="fc3a7-111">A primeira versão estável será 1.0, mas o módulo tem paridade de funcionalidades com o AzureRm a partir de novembro de 2018.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-111">The first stable release will be 1.0, but the module has feature parity with AzureRm as of November 2018.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="fc3a7-112">Atualizar para Az</span><span class="sxs-lookup"><span data-stu-id="fc3a7-112">Upgrade to Az</span></span>

<span data-ttu-id="fc3a7-113">Recomenda-se que os utilizadores atualizem para o novo módulo do `Az`.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-113">It's recommended that users upgrade to the new `Az` module.</span></span> <span data-ttu-id="fc3a7-114">Para tal:</span><span class="sxs-lookup"><span data-stu-id="fc3a7-114">To do so:</span></span>

* [<span data-ttu-id="fc3a7-115">Desinstalar o módulo do Azure PowerShell AzureRM</span><span class="sxs-lookup"><span data-stu-id="fc3a7-115">Uninstall the Azure PowerShell AzureRM module</span></span>](/powershell/azure/uninstall-azurerm-ps)
* [<span data-ttu-id="fc3a7-116">Instalar o módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="fc3a7-116">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="fc3a7-117">Ative o modo de compatibilidade para o AzureRM com `Enable-AzureRMAlias`, enquanto se familiariza com o novo conjunto de comandos.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-117">Enable compatibility mode for AzureRM with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="fc3a7-118">Migrar scripts existentes para o Az</span><span class="sxs-lookup"><span data-stu-id="fc3a7-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="fc3a7-119">As atualizações importantes podem ser inconvenientes.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="fc3a7-120">No entanto, o módulo `Az` tem um modo de compatibilidade para o ajudar a utilizar os scripts existentes enquanto trabalha em atualizações para a nova sintaxe.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-120">However, the `Az` module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="fc3a7-121">Utilize o cmdlet `Enable-AzureRmAlias` para ativar o modo de compatibilidade `AzureRM`.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-121">Use the `Enable-AzureRmAlias` cmdlet to enable the `AzureRM` compatibility mode.</span></span> <span data-ttu-id="fc3a7-122">Este cmdlet define nomes de cmdlet `AzureRM` como aliases para os novos nomes de cmdlet `Az`.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-122">This cmdlet defines `AzureRM` cmdlet names as aliases for the new `Az` cmdlet names.</span></span>

<span data-ttu-id="fc3a7-123">Os novos nomes de cmdlet foram criados para serem fáceis de aprender.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="fc3a7-124">Em vez de utilizar `AzureRm` ou `Azure` em nomes de cmdlet, utilize `Az`.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="fc3a7-125">Por exemplo, o comando antigo `New-AzureRmVm` tornou-se `New-AzVm`.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-125">For example, the old command `New-AzureRmVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="fc3a7-126">Para obter uma descrição completa do processo de migração, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="fc3a7-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="fc3a7-127">O futuro do suporte para o AzureRM</span><span class="sxs-lookup"><span data-stu-id="fc3a7-127">The future of support for AzureRM</span></span>

<span data-ttu-id="fc3a7-128">A módulo `AzureRM` atual deixará de receber novos cmdlets ou funcionalidades quando a versão 1.0 `Az` for lançada em dezembro de 2018.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-128">The existing `AzureRM` module will no longer receive new cmdlets or features when `Az` version 1.0 is released in December 2018.</span></span> <span data-ttu-id="fc3a7-129">No entanto, `AzureRM` ainda é oficialmente mantida e irá obter as correções de erros.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-129">However, `AzureRM` is still officially maintained and will get bug fixes.</span></span> <span data-ttu-id="fc3a7-130">Para se manter atualizado com os mais recentes serviços e funcionalidades do Azure, deve trocar para o módulo `Az`.</span><span class="sxs-lookup"><span data-stu-id="fc3a7-130">To keep up with the latest Azure services and features, you should switch to the `Az` module.</span></span>