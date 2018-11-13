---
title: Migrar scripts do Azure PowerShell do AzureRM para o Az
description: Conheça os passos e as ferramentas para migrar scripts do módulo do AzureRM para o novo módulo do Az.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 0c73e7ac1d47a2a97b6136fa481d0adce8de33db
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274903"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>Migrar do AzureRM para o Azure PowerShell Az

O módulo do Az tem paridade de funcionalidades com o AzureRM, mas utiliza nomes de cmdlet mais curtos e mais consistentes.
Os scripts escritos para os cmdlets do AzureRM não irão funcionar automaticamente com o módulo novo. Para facilitar a transição, o Az oferece ferramentas para permitir a execução dos seus scripts existentes com o AzureRM. Uma migração para um novo conjunto de comandos nunca é conveniente, mas este artigo ajuda-o a fazer a transição para o novo módulo.

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>Certifique-se de que os seus scripts existentes funcionam com a versão mais recente do AzureRM

Este é o passo mais importante! Execute os seus scripts existentes e certifique-se de que funcionam com a versão _mais recente_ do AzureRM (__6.12.0__). Se os scripts não funcionarem, certifique-se de que lê o [guia de migração do AzureRM](migration-guide.6.0.0.md).

## <a name="install-the-azure-powershell-az-module"></a>Instalar o módulo do Azure PowerShell Az

O primeiro passo é instalar o módulo do Az na sua plataforma. Para instalar o Az, precisa de desinstalar o AzureRM.
Nos passos seguintes, irá aprender como continuar a executar os scripts existentes e permitir a compatibilidade dos nomes de cmdlet antigos.

Para instalar o módulo do Azure PowerShell Az, siga estes passos:

* [Desinstalar o módulo do AzureRM](uninstall-azurerm-ps.md). Certifique-se de que remove _todas_ as versões instaladas do AzureRM, e não apenas a versão mais recente.
* [Instalar o módulo do Az](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><a name="aliases"/>Ativar o modo de alias do AzureRM

Com o AzureRM desinstalado e os seus scripts a funcionarem com a versão mais recente do AzureRM, chegou o momento de ativar o modo de compatibilidade para o módulo do Az. A compatibilidade é ativada com o comando:

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

Os aliases ativam a capacidade de utilizar nomes de cmdlet antigos com o módulo `Az` instalado. Estes aliases são escritos para o perfil de utilizador do âmbito selecionado. Se não existir um perfil de utilizador, é criado um.

> [!WARNING]
>
> Pode utilizar um `-Scope` diferente para este comando, mas não é recomendado! Os aliases são escritos para o perfil de utilizador para o âmbito selecionado, por isso continue a permitir que tenham um âmbito o mais limitado possível. Ativar aliases em todo o sistema também pode causar problemas para outros utilizadores que têm o `AzureRM` instalado no seu âmbito local.

Assim que o modo de alias estiver ativado, execute os seus scripts novamente para confirmar que ainda funcionam como esperado. 

## <a name="change-module-imports-and-cmdlet-names"></a>Alterar importações de módulo e nomes de cmdlet

Em geral, os nomes dos módulos foram alterados para que `AzureRM` e `Azure` se tornassem `Az`, e o mesmo para os cmdlets.
Por exemplo, o módulo `AzureRM.Compute` foi renomeado para `Az.Compute`. `New-AzureRmVM` tornou-se `New-AzVM`, e `Get-AzureStorageBlob` é agora `Get-AzStorageBlob`.

Existem exceções a esta alteração de nomenclatura que deve ter conhecimento antes de fazer qualquer mudança de nome:

| Módulo do AzureRM | Módulo do Az |
|----------------|-----------|
| AzureRM.DataFactories | Az.DataFactory |
| AzureRM.DataFactoryV2 | Az.DataFactory |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices |

## <a name="summary"></a>Resumo

Ao seguir estes passos, pode atualizar todos os scripts existentes para utilizarem o módulo novo. Se tiver dúvidas ou problemas com estes passos que dificultaram a sua migração, comente este artigo para que possamos melhorar as instruções.