---
title: Utilizar módulos experimentais do Azure PowerShell
description: Compreenda a filosofia e utilização dos módulos experimentais do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: ae2fecf73271a34a08ac66de03962a7a529e353b
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882493"
---
# <a name="use-experimental-azure-powershell-modules"></a>Utilizar módulos experimentais do Azure PowerShell

Dada a ênfase nas ferramentas de programador no Azure, a equipa do Azure PowerShell está a experimentar várias melhorias na experiência do Azure PowerShell. Este artigo descreve como optar ativamente por participar nas experiências com o Azure PowerShell e enviar comentários à equipa de desenvolvimento.

## <a name="experimentation-methodology"></a>Metodologia de experimentação

Para facilitar a experimentação, estamos a criar novos módulos do Azure PowerShell que implementam funcionalidades SDK existentes do Azure em novas formas, mais fáceis de utilizar. Na maioria dos casos, os cmdlets espelham exatamente os cmdlets existentes. No entanto, os cmdlets experimentais fornecem uma notação abreviada compacta e valores predefinidos mais inteligentes, que facilitam a criação e gestão dos recursos do Azure.

Estes módulos podem ser instalados lado a lado com módulos existentes do Azure PowerShell. Os nomes dos cmdlets foram abreviados para fornecer nomes mais curtos e evitar conflitos de nomes com cmdlets existentes não experimentais.

Os módulos experimentais utilizam a seguinte convenção de nomenclatura: `Az.*.Experiments`. Esta convenção de nomenclatura é semelhante à nomenclatura dos módulos de Pré-visualização: `Az.*.Preview`. Os módulos de pré-visualização diferem dos módulos experimentais. Os módulos de pré-visualização implementam novas funcionalidades dos serviços do Azure que só estão disponíveis como uma oferta de Pré-visualização. Os módulos de pré-visualização substituem os módulos existentes do Azure PowerShell e utilizam o mesmo cmdlet e os nomes dos parâmetros.

## <a name="how-to-install-an-experimental-module"></a>Como instalar um módulo experimental

Os módulos experimentais são publicados na Galeria do PowerShell, tal como os módulos existentes do Azure PowerShell. Para ver uma lista de módulos experimentais, execute o comando seguinte:

```azurepowershell-interactive
Find-Module Az.*.Experiments
```

Para instalar um módulo experimental, utilize o cmdlet `Install-Module`.

### <a name="documentation-and-support"></a>Documentação e suporte

A documentação está incluída no pacote de instalação e é acedida utilizando o cmdlet `Get-Help`. Não foi publicada nenhuma documentação oficial dos módulos experimentais.

Aconselhamo-lo a testar estes módulos. Os seus comentários permitem-nos melhorar a facilidade de utilização e responder às suas necessidades. No entanto, por ser experimental, o suporte para estes módulos é limitado. As perguntas ou relatórios de problemas podem ser submetidos criando um [problema](https://github.com/Azure/azure-powershell/issues) no repositório do GitHub.

## <a name="experiments-and-areas-of-improvement"></a>Experimentações e áreas de melhoria

Estas melhorias foram selecionadas com base em diferenciadores-chave de produtos concorrentes. Por exemplo, a CLI do Azure fez questão de basear os comandos em _cenários_, em vez de na _área de superfície da API_.
A CLI do Azure utiliza várias predefinições inteligentes que simplificam os cenários de "introdução" para os utilizadores finais.

### <a name="core-improvements"></a>Melhorias centrais

As melhorias centrais são consideradas de “senso comum”, e é necessária pouca experimentação para avançar na implementação destas atualizações.

- Cmdlets baseados em cenários - * *Todos* - os cmdlets devem ser concebidos em torno de cenários, e não em torno do serviço REST do Azure.

- Nomes mais curtos - inclui os nomes de cmdlets e os nomes de parâmetros.
  Utilize aliases para compatibilidade com os cmdlets “antigos”. Forneça conjuntos de parâmetros _retrocompatíveis_.

- Predefinições inteligentes - crie predefinições inteligentes para preencher informações “obrigatórias”. Por exemplo:
  - Grupo de Recursos
  - Localização
  - Recursos dependentes

### <a name="experimental-improvements"></a>Melhorias experimentais

As melhorias experimentais apresentam uma alteração significativa que a equipa pretende validar através de experimentação.

- Tipos simples - a criação de cenários deve afastar-se de tipos complexos e objetos de configuração. Simplifique a configuração para um ou dois parâmetros.

- “Criação Inteligente” - todos os cenários de criação que implementam a “Criação Inteligente” _não_ deviam ter parâmetros obrigatórios: todas as informações necessárias seriam escolhidas pelo Azure PowerShell, de forma opinativa.

- Parâmetros Cinzentos - em muitos casos, alguns parâmetros podem ser “cinzentos” ou semi-opcionais. Se o parâmetro não for especificado, é perguntado ao utilizador se pretende que o parâmetro seja gerado. Também faz sentido que os parâmetros cinzentos infiram um valor baseado no contexto, com o consentimento do utilizador.
  Por exemplo, faz sentido que o parâmetro cinzento sugira o valor mais recentemente utilizado.

- Comutador `-Auto` - o comutador `-Auto` iria fornecer uma forma de “opt-in” para os utilizadores _predefinirem todos os aspetos_, mantendo a integridade dos parâmetros obrigatórios no caminho da linha principal.

### <a name="feature-specific-switches"></a>Comutadores específicos de funcionalidades

Por exemplo, o cenário “Criar aplicação Web” poderia ter um comutador `-Git` ou `-AddRemote` que iria adicionar automaticamente um “azure” remoto a um repositório existente do git.

- Predefinições definíveis: os utilizadores podem definir as predefinições para os parâmetros comuns, como `-ResourceGroupName` e `-Location`.

- Predefinições de Tamanho - os “tamanhos” dos recursos podem ser confusos para os utilizadores, uma vez que muitos Fornecedores de Recursos utilizam nomes diferentes (por exemplo, “Standard\_DS1\_v2” ou “S1”). No entanto, a maioria dos utilizadores preocupa-se mais com o custo. Por isso, faz sentido definir tamanhos "universais", com base num agendamento de preços. Os utilizadores podem escolher um tamanho específico ou permitir que o Azure PowerShell escolha a _melhor opção_ com base no orçamento para recursos.

- Formato de Saída - atualmente, o Azure PowerShell devolve `PSObject`s e há pouca saída da consola. O Azure PowerShell poderá ter de apresente algumas informações ao utilizador sobre as "predefinições inteligentes" utilizadas.
