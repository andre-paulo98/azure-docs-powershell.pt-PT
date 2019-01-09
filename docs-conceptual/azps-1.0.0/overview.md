---
title: Descrição Geral do Azure PowerShell
description: Uma descrição geral do módulo do Az do Azure PowerShell, com informações sobre como instalar e começar a utilizar.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736465"
---
# <a name="overview-of-azure-powershell"></a>Descrição Geral do Azure PowerShell

O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure. O Azure PowerShell utiliza o .NET Standard, o que significa que o mesmo está disponível para Windows, macOS e Linux.
O Azure PowerShell também está disponível no Azure Cloud Shell.

Utilize o [Azure Cloud Shell](/azure/cloud-shell/overview) para executar o Azure PowerShell no seu browser ou [instale localmente](install-az-ps.md). Consulte o artigo [Introdução](get-started-azureps.md) para se familiarizar com as noções básicas do Azure PowerShell e obter uma introdução ao Azure.

Para obter informações sobre a versão mais recente do Azure PowerShell, veja as [notas de versão](release-notes-azureps.md).

## <a name="about-the-new-az-module"></a>Acerca do novo módulo do Az

Esta documentação descreve o novo módulo do Az para o Azure PowerShell. Este novo módulo foi escrito de raiz com base no .NET Standard. A utilização do .NET Standard permite que o Azure PowerShell seja executado no PowerShell 5.x em Windows ou no PowerShell 6 em qualquer plataforma. O módulo do Az é agora o modo com se deve interagir com o Azure através do PowerShell.
O AzureRM irá continuar a ser alvo de correções de erros, mas deixará de receber novas funcionalidades.

Obtenha os detalhes completos sobre o novo módulo, incluindo a mudança de nome dos comandos e os planos de manutenção para o AzureRM, no artigo [Apresentação do módulo do Az do Azure PowerShell](new-azureps-module-az.md). Se pretender começar a utilizar imediatamente o novo módulo, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).

Também existe [documentação do AzureRM](/powershell/azure/azurerm) disponível.

> [!IMPORTANT]
>
> Apesar de a documentação do Azure estar a ser alvo de atualizações de modo a refletir os novos nomes de cmdlets do módulo, é possível que os artigos ainda utilizem os comandos do AzureRM. Depois de instalar o módulo do Az, recomenda-se que ative os aliases de cmdlets do AzureRM com `Enable-AzureRmAlias`. Veja o artigo [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md) para obter mais detalhes.

## <a name="common-scenarios"></a>Cenários comuns

Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:

* [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a>Aprenda as noções básicas do PowerShell

Se não está familiarizado com o PowerShell, uma introdução poderá revelar-se útil.

* [Instalar o PowerShell](/powershell/scripting/setup/installing-windows-powershell)
* [Scripting com o PowerShell](/powershell/scripting/powershell-scripting)

Também pode ver este vídeo: [Noções básicas do PowerShell: (Parte 1) Introdução ao PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).

Ou assista à [Introdução ao Arranque do PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) da Microsoft Virtual Academy.

## <a name="build-your-skills-with-microsoft-learn"></a>Desenvolva as suas competências com o Microsoft Learn

- [Utilizar scripts para automatizar as tarefas do Azure com o PowerShell](/learn/modules/automate-azure-tasks-with-powershell/)
- [Mais aprendizagem interativa...](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a>Outros módulos do Azure PowerShell

* [Azure Active Directory](/powershell/azure/active-directory/)
* [Azure Information Protection](/powershell/azure/aip/)
* [Azure Service Fabric](/powershell/azure/service-fabric/)
* [Azure ElasticDB](/powershell/azure/elasticdbjobs/)
