---
title: Apresentação do módulo do Azure PowerShell Az
description: Apresentação do novo módulo do Azure PowerShell Az, a substituição do módulo AzureRM.
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 10665a72bc7dcae8ecf36b5ef4e2ab285a0e78b7
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048704"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="f1eab-103">Apresentação do novo módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="f1eab-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="f1eab-104">A partir de dezembro de 2018, o módulo do Az do Azure PowerShell passa a ser uma versão de disponibilidade geral e é agora o módulo indicado do PowerShell para interagir com o Azure.</span><span class="sxs-lookup"><span data-stu-id="f1eab-104">Starting in December 2018, the Azure PowerShell Az module is in general release and now the intended PowerShell module for interacting with Azure.</span></span> <span data-ttu-id="f1eab-105">O Az oferece comandos mais curtos, maior estabilidade e suporte para várias plataformas.</span><span class="sxs-lookup"><span data-stu-id="f1eab-105">Az offers shorter commands, improved stability, and cross-platform support.</span></span> <span data-ttu-id="f1eab-106">O Az também oferece paridade de funcionalidades e um caminho de migração fácil a partir do AzureRM.</span><span class="sxs-lookup"><span data-stu-id="f1eab-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="f1eab-107">O Az utiliza a biblioteca .NET Standard, o que significa pode ser executado no PowerShell 5 e no PowerShell 6.</span><span class="sxs-lookup"><span data-stu-id="f1eab-107">Az uses the .NET Standard library, which means it runs on PowerShell 5 and PowerShell 6.</span></span>
<span data-ttu-id="f1eab-108">Uma vez que o PowerShell 6 pode ser executado em Linux, macOS e Windows, o Azure PowerShell encontra-se agora disponível para todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="f1eab-108">Since PowerShell 6 can run on Linux, macOS, and Windows, Azure PowerShell is now available for all platforms.</span></span>
<span data-ttu-id="f1eab-109">A utilização do .NET Standard permite-nos unificar a base de código do Azure PowerShell com o mínimo impacto nos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="f1eab-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="f1eab-110">O Az é um módulo novo, pelo que a versão foi reposta para 1.0.0.</span><span class="sxs-lookup"><span data-stu-id="f1eab-110">Az is a new module, so the version has been reset to 1.0.0.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="f1eab-111">Atualizar para Az</span><span class="sxs-lookup"><span data-stu-id="f1eab-111">Upgrade to Az</span></span>

<span data-ttu-id="f1eab-112">Recomenda-se que todos os utilizadores façam a atualização para o novo módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="f1eab-112">It's recommended that all users upgrade to the new Az module.</span></span> <span data-ttu-id="f1eab-113">Para tal:</span><span class="sxs-lookup"><span data-stu-id="f1eab-113">To do so:</span></span>

* <span data-ttu-id="f1eab-114">__RECOMENDADO__: [Desinstalar o módulo do Azure PowerShell AzureRM](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span><span class="sxs-lookup"><span data-stu-id="f1eab-114">__RECOMMENDED__: [Uninstall the Azure PowerShell AzureRM module](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span></span>
* [<span data-ttu-id="f1eab-115">Instalar o módulo do Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="f1eab-115">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="f1eab-116">Ative o modo de compatibilidade para adicionar aliases para cmdlets do AzureRM com `Enable-AzureRMAlias` enquanto se familiariza com o novo conjunto de comandos.</span><span class="sxs-lookup"><span data-stu-id="f1eab-116">Enable compatibility mode to add aliases for AzureRM cmdlets with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span> <span data-ttu-id="f1eab-117">Ative os aliases __apenas__ se não tiver o AzureRM instalado.</span><span class="sxs-lookup"><span data-stu-id="f1eab-117">__Only__ enable aliases if you do not have AzureRM installed.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="f1eab-118">Migrar scripts existentes para o Az</span><span class="sxs-lookup"><span data-stu-id="f1eab-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="f1eab-119">As atualizações importantes podem ser inconvenientes.</span><span class="sxs-lookup"><span data-stu-id="f1eab-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="f1eab-120">No entanto, o módulo do Az tem um modo de compatibilidade para o ajudar a utilizar os scripts existentes enquanto trabalha nas atualizações para a nova sintaxe.</span><span class="sxs-lookup"><span data-stu-id="f1eab-120">However, the Az module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="f1eab-121">Utilize o cmdlet `Enable-AzureRmAlias` para ativar o modo de compatibilidade do AzureRM.</span><span class="sxs-lookup"><span data-stu-id="f1eab-121">Use the `Enable-AzureRmAlias` cmdlet to enable the AzureRM compatibility mode.</span></span> <span data-ttu-id="f1eab-122">Este cmdlet define os nomes de cmdlets do AzureRM como aliases para os novos nomes de cmdlets do Az.</span><span class="sxs-lookup"><span data-stu-id="f1eab-122">This cmdlet defines AzureRM cmdlet names as aliases for the new Az cmdlet names.</span></span>

<span data-ttu-id="f1eab-123">Os novos nomes de cmdlet foram criados para serem fáceis de aprender.</span><span class="sxs-lookup"><span data-stu-id="f1eab-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="f1eab-124">Em vez de utilizar `AzureRm` ou `Azure` em nomes de cmdlet, utilize `Az`.</span><span class="sxs-lookup"><span data-stu-id="f1eab-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="f1eab-125">Por exemplo, o comando antigo `New-AzureRMVm` tornou-se `New-AzVm`.</span><span class="sxs-lookup"><span data-stu-id="f1eab-125">For example, the old command `New-AzureRMVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="f1eab-126">Para obter uma descrição completa do processo de migração, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="f1eab-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="f1eab-127">O futuro do suporte para o AzureRM</span><span class="sxs-lookup"><span data-stu-id="f1eab-127">The future of support for AzureRM</span></span>

<span data-ttu-id="f1eab-128">O módulo do AzureRM existente deixará de receber novos cmdlets ou funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="f1eab-128">The existing AzureRM module will no longer receive new cmdlets or features.</span></span> <span data-ttu-id="f1eab-129">No entanto, o AzureRM ainda é oficialmente mantido e será alvo de correções de erros até dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="f1eab-129">However, AzureRM is still officially maintained and will get bug fixes up through December 2020.</span></span> <span data-ttu-id="f1eab-130">Para se manter a par dos serviços e funcionalidades mais recentes do Azure, mude para o módulo Az.</span><span class="sxs-lookup"><span data-stu-id="f1eab-130">To keep up with the latest Azure services and features, switch to the Az module.</span></span>
