---
title: Migrar scripts do Azure PowerShell do AzureRM para o Az
description: Conheça os passos e as ferramentas para migrar scripts do módulo do AzureRM para o novo módulo do Az.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/10/2019
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 83860dd5abfbb1c3da94de6813bceca1bbb0fca7
ms.sourcegitcommit: 15f21c40dcb7610e2fbaaabf264ad925e4224500
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90928407"
---
# <a name="migrate-azure-powershell-from-azurerm-to-az"></a>Migrar o Azure PowerShell do AzureRM para o Az

O módulo do Az tem paridade de funcionalidades com o AzureRM, mas utiliza nomes de cmdlet mais curtos e mais consistentes.
Os scripts escritos para os cmdlets do AzureRM não irão funcionar automaticamente com o módulo novo. Para facilitar a transição, o Az oferece ferramentas para permitir a execução dos seus scripts existentes com o AzureRM. Uma migração para um novo conjunto de comandos nunca é conveniente, mas este artigo ajuda-o a fazer a transição para o novo módulo.

Para ver a lista completa das alterações interruptivas entre o AzureRM e o Az, veja [todas as alterações do AzureRM para o Az](migrate-az-1.0.0.md).

## <a name="ensure-existing-scripts-work-with-the-latest-azurerm-release"></a>Certifique-se de que os scripts existentes funcionam com a versão mais recente do AzureRM

Antes de realizar quaisquer passos de migração, verifique quais são as versões do AzureRM que se encontram instaladas no sistema. Ao fazê-lo, certifica-se de que os scripts já estão em execução na versão mais recente e fica a saber que versões do AzureRM têm de ser desinstaladas.

Para verificar quais são as versões do AzureRM que se encontram instaladas, execute o comando:

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

A versão __mais recente__ disponível do AzureRM é a __6.13.1__. Se não tiver esta versão instalada, os seus scripts existentes poderão precisar de modificações adicionais para funcionar com o módulo Az para além do que foi descrito aqui e na [lista de alterações interruptivas](migrate-az-1.0.0.md).

Se os scripts não funcionarem com o AzureRM 6.13.1, atualize-os de acordo com o [guia de migração do AzureRM 5.x para o 6.x](/powershell/azure/azurerm/migration-guide.6.0.0).
Se utilizar uma versão anterior do módulo AzureRM, existem guias de migração disponíveis para cada versão principal.

## <a name="uninstall-azurerm"></a>Desinstalar o AzureRM

Não é garantido que o módulo Az seja compatível com quaisquer instalações existentes do AzureRM no PowerShell 5.1 para Windows. Antes de instalar o módulo Az, [desinstale o AzureRM](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).

> [!IMPORTANT]
>
> Se não estiver pronto para remover o módulo AzureRM do sistema, pode antes instalar o módulo Az para o [PowerShell Core](/powershell/scripting/install/installing-powershell-core-on-windows) 6.x ou versão posterior. O PowerShell Core e o PowerShell 5.1 para Windows utilizam diferentes bibliotecas de módulos, pelo que não ocorrerão conflitos. Continua a poder [ativar aliases](#enable-azurerm-compatibility-aliases) no PowerShell Core.

## <a name="install-the-azure-powershell-az-module"></a>Instalar o módulo do Azure PowerShell Az

O primeiro passo é instalar o módulo do Az na sua plataforma. Quando instalar o Az, recomenda-se que desinstale o AzureRM. Nos passos seguintes, irá aprender como continuar a executar os scripts existentes e permitir a compatibilidade dos nomes de cmdlet antigos.

Para instalar o módulo Az do Azure PowerShell, siga as instruções em [Instalar o módulo Az](install-az-ps.md).

> [!NOTE]
> Neste momento, poderá querer executar o cmdlet [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) fornecido no módulo Az, apenas para se certificar de que todas as versões do AzureRM foram desinstaladas e não causarão conflitos.

## <a name="enable-azurerm-compatibility-aliases"></a>Ativar aliases de compatibilidade do AzureRM

Com o AzureRM desinstalado e os scripts a funcionarem com a versão mais recente do AzureRM, chegou o momento de ativar o modo de compatibilidade para o módulo do Az. A compatibilidade é ativada com o comando:

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

Os aliases ativam a capacidade de utilizar nomes de cmdlets antigos com o módulo do Az instalado. Estes aliases são escritos para o perfil do âmbito selecionado. Se não existir um perfil, é criado um.
Quando utilizar um `-Scope` mais amplo do que `CurrentUser`, são necessárias as permissões adequadas para criar ou atualizar o ficheiro de perfil correspondente.

> [!IMPORTANT]
> __Apenas__ os nomes de cmdlet têm aliases. Os nomes dos módulos não têm! Se estiver a utilizar `#Requires`, `Import-Module`, listas de dependência num `.psd1` ou nomes de cmdlet completamente qualificados, certifique-se de que os migra neste momento através do processo descrito na [lista de alterações interruptivas](migrate-az-1.0.0.md) relativa aos nomes de módulos.

> [!WARNING]
>
> Pode utilizar um `-Scope` diferente para este comando, mas tal não é recomendado. Os aliases são escritos para o perfil de utilizador para o âmbito selecionado, por isso continue a permitir que tenham um âmbito o mais limitado possível. A ativação dos aliases no sistema em geral pode causar problemas a outros utilizadores que tenham o AzureRM instalado no respetivo âmbito local.

Assim que o modo de alias estiver ativado, execute os seus scripts novamente para confirmar que ainda funcionam como esperado.
Alguns nomes de parâmetro foram alterados, adicionados ou passaram a ser obrigatórios para o módulo Az. Os tipos de saída dos cmdlets também podem ter sido alterados. Estas alterações estão detalhadas na [lista de alterações interruptivas](migrate-az-1.0.0.md).

## <a name="update-cmdlets-modules-and-parameters"></a>Atualizar cmdlets, módulos e parâmetros

Com os scripts atualizados e em execução nos aliases, pode atualizá-los quando quiser para que utilizem os novos cmdlets e tirem partido de outras alterações, como novas funcionalidades. Para a maioria dos scripts, apenas terá de atualizar os nomes dos cmdlets, pelo que terá de [seguir o novo esquema de nomenclatura de cmdlets no Az](migrate-az-1.0.0.md#cmdlet-noun-prefix-changes). Também poderá haver outras alterações que terá de fazer para que os seus scripts funcionem, consoante a função dos mesmos e das funcionalidades do Azure PowerShell de que tiram partido.

Por exemplo, os [cmdlets do Armazenamento de Blobs](migrate-az-1.0.0.md#azstorage-previously-azurestorage-and-azurermstorage) foram completamente reformulados de forma a utilizar um novo modelo assíncrono, pelo que será mais difícil atualizar os scripts que utilizem estes cmdlets do que os scripts em que as únicas alterações relevantes foram alterações de nomes de cmdlet.

Mesmo que apenas tenha tido de fazer alterações pequenas e simples aos seus scripts até este momento, ou ainda que funcionem sem modificações adicionais quando os aliases estão ativados, leia a [lista completa de alterações interruptivas no Az 1.0.0](migrate-az-1.0.0.md) para se certificar de que não está dependente do comportamento "transparente" de aliases que poderão desaparecer depois de alterar os nomes dos cmdlets e desativar os aliases.

## <a name="disable-aliases"></a>Desativar aliases

Depois de concluir a migração e de já não estar dependente do comportamento dos aliases, recomendamos que desative os aliases. Para isso, utilize o cmdlet [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).

> [!IMPORTANT]
> Quando executar este cmdlet, __certifique-se__ de que o invoca para cada `-Scope` para os quais `Enable-AzureRmAlias` foi invocado. Caso contrário, poderá continuar a existir scripts no seu sistema dependentes do comportamento dos aliases.
