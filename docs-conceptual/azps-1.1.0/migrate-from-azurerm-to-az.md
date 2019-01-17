---
title: Migrar scripts do Azure PowerShell do AzureRM para o Az
description: Conheça os passos e as ferramentas para migrar scripts do módulo do AzureRM para o novo módulo do Az.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 28122ca953d62b405f19effbbc680f2dc6202cca
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342116"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>Migrar do AzureRM para o Azure PowerShell Az

O módulo do Az tem paridade de funcionalidades com o AzureRM, mas utiliza nomes de cmdlet mais curtos e mais consistentes.
Os scripts escritos para os cmdlets do AzureRM não irão funcionar automaticamente com o módulo novo. Para facilitar a transição, o Az oferece ferramentas para permitir a execução dos seus scripts existentes com o AzureRM. Uma migração para um novo conjunto de comandos nunca é conveniente, mas este artigo ajuda-o a fazer a transição para o novo módulo.

Para ver a lista completa das alterações interruptivas entre o AzureRM e o Az, consulte o [Guia de migração do Az 1.0.0](migrate-az-1.0.0.md)

## <a name="check-for-installed-versions-of-azurerm"></a>Verificar se existem versões instaladas do AzureRM

O módulo do Az pode estar instalado lado a lado com o módulo do AzureRM, mas tal não é recomendável. Antes de realizar quaisquer passos de migração, verifique quais são as versões do AzureRM que se encontram instaladas no sistema. Ao fazê-lo, certifica-se de que os scripts já estão em execução na versão mais recente e fica a saber se pode ativar aliases de comandos sem desinstalar o AzureRM.

Para verificar quais são as versões do AzureRM que se encontram instaladas, execute o comando:

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>Certifique-se de que os seus scripts existentes funcionam com a versão mais recente do AzureRM

Este é o passo mais importante! Execute os scripts existentes e certifique-se de que funcionam com a versão _mais recente_ do AzureRM (__6.13.1__). Se os scripts não funcionarem, certifique-se de que lê o [guia de migração do AzureRM](/powershell/azure/azurerm/migration-guide.6.0.0).

## <a name="install-the-azure-powershell-az-module"></a>Instalar o módulo do Azure PowerShell Az

O primeiro passo é instalar o módulo do Az na sua plataforma. Quando instalar o Az, recomenda-se que desinstale o AzureRM. Nos passos seguintes, irá aprender como continuar a executar os scripts existentes e permitir a compatibilidade dos nomes de cmdlet antigos.

Para instalar o módulo do Azure PowerShell Az, siga estes passos:

* __RECOMENDADO__: [Desinstalar o módulo do AzureRM](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).
  Certifique-se de que remove _todas_ as versões instaladas do AzureRM, e não apenas a versão mais recente.
* [Instalar o módulo do Az](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-compatibility-aliases"></a><a name="aliases"/>Ativar os aliases de compatibilidade do AzureRM 

> [!IMPORTANT]
>
> Ative o modo de compatibilidade apenas se tiver desinstalado _todas as_ versões do AzureRM. A ativação do modo de compatibilidade com os cmdlets do AzureRM ainda disponíveis pode resultar num comportamento imprevisível. Ignore este passo se optar por manter o AzureRM instalado, mas tenha em atenção que os cmdlets do AzureRM irão utilizar os módulos mais antigos e não vão chamar quaisquer cmdlets do Az.

Com o AzureRM desinstalado e os scripts a funcionarem com a versão mais recente do AzureRM, chegou o momento de ativar o modo de compatibilidade para o módulo do Az. A compatibilidade é ativada com o comando:

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

Os aliases ativam a capacidade de utilizar nomes de cmdlets antigos com o módulo do Az instalado. Estes aliases são escritos para o perfil de utilizador do âmbito selecionado. Se não existir um perfil de utilizador, é criado um.

> [!WARNING]
>
> Pode utilizar um `-Scope` diferente para este comando, mas tal não é recomendado. Os aliases são escritos para o perfil de utilizador para o âmbito selecionado, por isso continue a permitir que tenham um âmbito o mais limitado possível. A ativação dos aliases no sistema em geral também pode causar problemas a outros utilizadores que tenham o AzureRM instalado no respetivo âmbito local.

Assim que o modo de alias estiver ativado, execute os seus scripts novamente para confirmar que ainda funcionam como esperado. 

## <a name="change-module-imports-and-cmdlet-names"></a>Alterar importações de módulo e nomes de cmdlet

Em geral, os nomes dos módulos foram alterados para que `AzureRM` e `Azure` se tornassem `Az`, e o mesmo para os cmdlets.
Por exemplo, o módulo `AzureRM.Compute` foi renomeado para `Az.Compute`. `New-AzureRMVM` tornou-se `New-AzVM`, e `Get-AzureStorageBlob` é agora `Get-AzStorageBlob`.

Existem exceções a esta alteração de nomenclatura de que deve estar ciente. Os nomes de alguns módulos foram mudados ou intercalados com os de módulos existentes sem afetar o sufixo dos respetivos cmdlets, exceto o facto de alterar `AzureRM` ou `Azure` para `Az`. Fora isso, o sufixo do cmdlet completo foi alterado de modo a refletir o novo nome do módulo.

| Módulo do AzureRM | Módulo do Az | O sufixo do cmdlet foi alterado? |
|----------------|-----------|------------------------|
| AzureRM.Profile | Az.Accounts | Sim |
| AzureRM.Insights | Az.Monitor | Sim |
| AzureRM.DataFactories | Az.DataFactory | Sim |
| AzureRM.DataFactoryV2 | Az.DataFactory | Sim |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices | Não |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices | Não |
| AzureRM.Tags | Az.Resources | Não |
| AzureRM.MachineLearningCompute | Az.MachineLearning | Não |
| AzureRM.UsageAggregates | Az.Billing | Não |
| AzureRM.Consumption | Az.Billing | Não |

## <a name="summary"></a>Resumo

Ao seguir estes passos, pode atualizar todos os scripts existentes para utilizarem o módulo novo. Se tiver dúvidas ou problemas com estes passos que dificultaram a sua migração, comente este artigo para que possamos melhorar as instruções.
