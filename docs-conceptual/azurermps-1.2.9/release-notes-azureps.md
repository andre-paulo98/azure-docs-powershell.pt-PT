---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: b42ad6f22f47e10c9190cf5a919f781375ff26f2
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2018
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