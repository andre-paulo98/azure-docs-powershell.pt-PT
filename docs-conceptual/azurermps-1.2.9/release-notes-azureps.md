---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 91d97260568a36e1135196899503fb0c8e1c6731
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853020"
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

## <a name="version-129"></a>Versão 1.2.9

Alterações nesta Versão

* Módulo AzureRm.AzureStackAdmin
    + Alterações no cmdlet Add-AzureRmResourceProviderRegistration para o suporte do Azure Resource Manager de Administrador e divisão do Azure Resource Manager de inquilino. Foi adicionado um novo parâmetro -ResourceManagerType.
    + Remoção dos parâmetros - AdminUri, -ApiVersion, -SubscriptionId e -Token de cada um dos cmdlets. Temos publicado avisos de que estes parâmetros serão preteridos e agora foram removidos.
* Módulo AzureStackStorage
    + Novos cmdlets adicionados para suportar cenários de migração de contentores.
    + Remoção dos cmdlets que fazem referência a componentes internos e funcionalidades subjacentes.
* AzureRM.BootStrapper
    + Novo módulo criado para a gestão de versões de cmdlets do Azure PowerShell através da utilização de perfis de versão