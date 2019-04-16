---
title: Descrição Geral do Azure PowerShell
description: Uma descrição geral do módulo do Az do Azure PowerShell, com informações sobre como instalar e começar a utilizar.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 01/10/2019
ms.openlocfilehash: 45ab083dd133c8c7b8dbe902484c92564bc216b9
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364258"
---
# <a name="overview-of-azure-powershell"></a>Descrição Geral do Azure PowerShell

O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure. O Azure PowerShell utiliza o .NET Standard, o que significa que o mesmo está disponível para Windows, macOS e Linux.
O Azure PowerShell também está disponível no Azure Cloud Shell.

## <a name="about-the-new-az-module"></a>Acerca do novo módulo do Az

Esta documentação descreve o novo módulo do Az para o Azure PowerShell. Este novo módulo foi escrito de raiz com base no .NET Standard. A utilização do .NET Standard permite executar o Azure PowerShell no PowerShell 5, no Windows ou no PowerShell 6 em qualquer plataforma. O módulo do Az é agora o modo com se deve interagir com o Azure através do PowerShell.
O AzureRM irá continuar a ser alvo de correções de erros, mas deixará de receber novas funcionalidades.

Obtenha os detalhes completos sobre o novo módulo, incluindo a mudança de nome dos comandos e os planos de manutenção para o AzureRM, no artigo [Apresentação do módulo do Az do Azure PowerShell](new-azureps-module-az.md). Se pretender começar a utilizar imediatamente o novo módulo, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).

Também existe [documentação do AzureRM](/powershell/azure/azurerm) disponível.

> [!IMPORTANT]
>
> Apesar de a documentação do Azure estar a ser alvo de atualizações de modo a refletir os novos nomes de cmdlets do módulo, é possível que os artigos ainda utilizem os comandos do AzureRM. Depois de instalar o módulo do Az, recomenda-se que ative os aliases de cmdlets do AzureRM com `Enable-AzureRmAlias`. Veja o artigo [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md) para obter mais detalhes.

## <a name="run-or-install"></a>Executar ou instalar

Pode instalar o Azure PowerShell no PowerShell 5.1 ou superior no Windows e no PowerShell 6 em qualquer plataforma, ou pode optar por executá-lo no Azure Cloud Shell.

* Para executar no browser com o Azure Cloud Shell, veja [Início Rápido do PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Para instalar o Azure PowerShell no seu sistema, veja [Instalar o Azure PowerShell](install-az-ps.md).

Para obter informações sobre a versão mais recente do Azure PowerShell, veja as [notas de versão](release-notes-azureps.md).

## <a name="get-started"></a>Introdução

Leia o artigo [Introdução ao Azure PowerShell](get-started-azureps.md) para aprender as noções básicas do Azure PowerShell. Se não está familiarizado com o PowerShell, uma introdução poderá revelar-se útil:

* [Instalar o PowerShell](/powershell/scripting/install/installing-powershell)
* [Scripting com o PowerShell](/powershell/scripting/powershell-scripting)
* [Noções Básicas do PowerShell: (Parte 1) Introdução ao PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)
* [Introdução ao Arranque do PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) da Microsoft Virtual Academy

Os exemplos seguintes podem ajudá-lo com algumas utilizações comuns do Azure:

* [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="build-your-skills-with-microsoft-learn"></a>Desenvolva as suas competências com o Microsoft Learn

- [Automatizar as tarefas do Azure com scripts com o PowerShell](/learn/modules/automate-azure-tasks-with-powershell/)
- [Mais aprendizagem interativa...](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a>Outros módulos do Azure PowerShell

* [Azure Active Directory](/powershell/azure/active-directory/)
* [Azure Service Fabric](/powershell/azure/service-fabric/)
* [Azure ElasticDB](/powershell/azure/elasticdbjobs/)
