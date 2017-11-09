---
title: "Registo de alterações do Azure PowerShell | Microsoft Docs"
description: "Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 5fe7591855577e083aad5923aed37b18d0b2a40c
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2017
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