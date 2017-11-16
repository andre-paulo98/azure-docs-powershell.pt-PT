---
title: "Utilizar módulos experimentais do Azure PowerShell"
description: "Compreenda a filosofia e utilização dos módulos experimentais do Azure PowerShell."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/05/2017
ms.openlocfilehash: 7a01957040be7c0498ef4f0e9b8f7297119221a5
ms.sourcegitcommit: 358d260a867c6ee2e8700b91f776ba4f1b0e24a5
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/11/2017
---
# <a name="using-experimental-azure-powershell-modules"></a><span data-ttu-id="a40a3-103">Utilizar módulos experimentais do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a40a3-103">Using experimental Azure PowerShell modules</span></span>

<span data-ttu-id="a40a3-104">Com o ênfase em ferramentas de programador (especialmente CLIs) no Azure, a equipa do Azure PowerShell está a experimentar várias melhorias na experiência do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a40a3-104">With the emphasis on developer tools (especially CLIs) in Azure, the Azure PowerShell team is experimenting with many improvements to the Azure PowerShell experience.</span></span>

## <a name="experimentation-methodology"></a><span data-ttu-id="a40a3-105">Metodologia de experimentação</span><span class="sxs-lookup"><span data-stu-id="a40a3-105">Experimentation methodology</span></span>

<span data-ttu-id="a40a3-106">Para facilitar a experimentação, estamos a criar novos módulos do Azure PowerShell que implementam funcionalidades SDK existentes do Azure em novas formas, mais fáceis de utilizar.</span><span class="sxs-lookup"><span data-stu-id="a40a3-106">To facilitate experimentation, we are creating new Azure PowerShell modules that implement existing Azure SDK functionality in new, easier to use ways.</span></span> <span data-ttu-id="a40a3-107">Na maioria dos casos, os cmdlets espelham exatamente os cmdlets existentes.</span><span class="sxs-lookup"><span data-stu-id="a40a3-107">In most cases, the cmdlets exactly mirror existing cmdlets.</span></span> <span data-ttu-id="a40a3-108">No entanto, os cmdlets experimentais fornecem uma notação abreviada compacta e valores predefinidos mais inteligentes, que facilitam a criação e gestão dos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="a40a3-108">However, the experimental cmdlets provide a shorthand notation and smarter default values that make it easier to create and manage Azure resources.</span></span>

<span data-ttu-id="a40a3-109">Estes módulos podem ser instalados lado a lado com módulos existentes do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a40a3-109">These modules can be installed side-by-side with existing Azure PowerShell modules.</span></span> <span data-ttu-id="a40a3-110">Os nomes dos cmdlets foram abreviados para fornecer nomes mais curtos e evitar conflitos de nomes com cmdlets existentes não experimentais.</span><span class="sxs-lookup"><span data-stu-id="a40a3-110">The cmdlet names have been shortened to provide shorter names and avoid name conflicts with existing, non-experimental cmdlets.</span></span>

<span data-ttu-id="a40a3-111">Os módulos experimentais utilizam a seguinte convenção de nomenclatura:</span><span class="sxs-lookup"><span data-stu-id="a40a3-111">The experimental modules use the following naming convention:</span></span>

- <span data-ttu-id="a40a3-112">AzureRM.Compute.Experiments</span><span class="sxs-lookup"><span data-stu-id="a40a3-112">AzureRM.Compute.Experiments</span></span>
- <span data-ttu-id="a40a3-113">AzureRM.Websites.Experiments</span><span class="sxs-lookup"><span data-stu-id="a40a3-113">AzureRM.Websites.Experiments</span></span>

<span data-ttu-id="a40a3-114">Esta convenção de nomenclatura é semelhante à nomenclatura dos módulos de Pré-visualização: `AzureRM.*.Preview`.</span><span class="sxs-lookup"><span data-stu-id="a40a3-114">This naming convention is similar to the naming of Preview modules: `AzureRM.*.Preview`.</span></span> <span data-ttu-id="a40a3-115">Os módulos de pré-visualização diferem dos módulos experimentais.</span><span class="sxs-lookup"><span data-stu-id="a40a3-115">Preview modules differ from experimental modules.</span></span> <span data-ttu-id="a40a3-116">Os módulos de pré-visualização implementam novas funcionalidades dos serviços do Azure que só estão disponíveis como uma oferta de Pré-visualização.</span><span class="sxs-lookup"><span data-stu-id="a40a3-116">Preview modules implement new functionality of Azure services that is only available as a Preview offering.</span></span> <span data-ttu-id="a40a3-117">Os módulos de pré-visualização substituem os módulos existentes do Azure PowerShell e utilizam o mesmo cmdlet e os nomes dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a40a3-117">Preview modules replace existing Azure PowerShell modules and use the same cmdlet and parameter names.</span></span>

## <a name="how-to-install-an-experimental-module"></a><span data-ttu-id="a40a3-118">Como instalar um módulo experimental</span><span class="sxs-lookup"><span data-stu-id="a40a3-118">How to install an experimental module</span></span>

<span data-ttu-id="a40a3-119">Os módulos experimentais são publicados na Galeria do PowerShell, tal como os módulos existentes do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a40a3-119">Experimental modules are published to the PowerShell Gallery just like the existing Azure PowerShell modules.</span></span> <span data-ttu-id="a40a3-120">Para ver uma lista de módulos experimentais, execute o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="a40a3-120">To see a list of experimental modules, run the following command:</span></span>

```powershell
Find-Module AzureRM.*.Experiments
```

```Output
Version    Name                                Repository           Description
-------    ----                                ----------           -----------
1.0.0      AzureRM.Websites.Experiments        PSGallery            Create and deploy web applications using Azure Ap...
1.0.25     AzureRM.Compute.Experiments         PSGallery            Azure Compute experiments for VM creation
```

<span data-ttu-id="a40a3-121">Para instalar o módulo experimental, utilize os seguintes comandos a partir de uma sessão elevada do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a40a3-121">To install the experimental module, use the following commands from an elevated PowerShell session:</span></span>

```powershell
Install-Module AzureRM.Compute.Experiments
Install-Module AzureRM.Websites.Experiments
```

### <a name="documentation-and-support"></a><span data-ttu-id="a40a3-122">Documentação e suporte</span><span class="sxs-lookup"><span data-stu-id="a40a3-122">Documentation and support</span></span>

<span data-ttu-id="a40a3-123">A documentação está incluída no pacote de instalação e é acedida utilizando o cmdlet `Get-Help`.</span><span class="sxs-lookup"><span data-stu-id="a40a3-123">Documentation is included in the install package and is accessed using the `Get-Help` cmdlet.</span></span> <span data-ttu-id="a40a3-124">Não foi publicada nenhuma documentação oficial dos módulos experimentais.</span><span class="sxs-lookup"><span data-stu-id="a40a3-124">No official documentation is published for experimental modules.</span></span>

<span data-ttu-id="a40a3-125">Aconselhamo-lo a testar estes módulos.</span><span class="sxs-lookup"><span data-stu-id="a40a3-125">We encourage you to test these modules.</span></span> <span data-ttu-id="a40a3-126">Os seus comentários permitem-nos melhorar a facilidade de utilização e responder às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="a40a3-126">Your feedback allows us to improve usability and respond to your needs.</span></span> <span data-ttu-id="a40a3-127">No entanto, por ser experimental, o suporte para estes módulos é limitado.</span><span class="sxs-lookup"><span data-stu-id="a40a3-127">However, being experimental, support for these modules is limited.</span></span> <span data-ttu-id="a40a3-128">As perguntas ou relatórios de problemas podem ser submetidos criando um [problema](https://github.com/Azure/azure-powershell/issues) no repositório do GitHub.</span><span class="sxs-lookup"><span data-stu-id="a40a3-128">Questions or problem reports can be submitted by creating an [issue](https://github.com/Azure/azure-powershell/issues) in the GitHub repository.</span></span>

## <a name="experiments-and-areas-of-improvement"></a><span data-ttu-id="a40a3-129">Experimentações e áreas de melhoria</span><span class="sxs-lookup"><span data-stu-id="a40a3-129">Experiments and areas of improvement</span></span>

<span data-ttu-id="a40a3-130">Estas melhorias foram selecionadas com base em diferenciadores-chave de produtos concorrentes.</span><span class="sxs-lookup"><span data-stu-id="a40a3-130">These improvements were selected based on key differentiators in competing products.</span></span> <span data-ttu-id="a40a3-131">Por exemplo, a CLI 2.0 do Azure fez questão de basear os comandos em _cenários_, em vez de na _área de superfície da API_.</span><span class="sxs-lookup"><span data-stu-id="a40a3-131">For example, Azure CLI 2.0 has made a point of basing commands on _scenarios_ rather than _API surface area_.</span></span>
<span data-ttu-id="a40a3-132">A CLI 2.0 do Azure utiliza várias predefinições inteligentes que facilitam os cenários de “introdução” aos utilizadores finais.</span><span class="sxs-lookup"><span data-stu-id="a40a3-132">Azure CLI 2.0 use a number of smart defaults that make "getting started" scenarios easier for end users.</span></span>

### <a name="core-improvements"></a><span data-ttu-id="a40a3-133">Melhorias centrais</span><span class="sxs-lookup"><span data-stu-id="a40a3-133">Core improvements</span></span>

<span data-ttu-id="a40a3-134">As melhorias centrais são consideradas de “senso comum”, e é necessária pouca experimentação para avançar na implementação destas atualizações.</span><span class="sxs-lookup"><span data-stu-id="a40a3-134">The core improvements are regarded as "common sense", and little experimentation is needed to move forward in implementing these updates.</span></span>

- <span data-ttu-id="a40a3-135">Cmdlets baseados em cenários - * *Todos* - os cmdlets devem ser concebidos em torno de cenários, e não em torno do serviço REST do Azure.</span><span class="sxs-lookup"><span data-stu-id="a40a3-135">Scenario-based Cmdlets - **All*- cmdlets should be designed around scenarios, not the Azure REST service.</span></span>

- <span data-ttu-id="a40a3-136">Nomes mais curtos - inclui os nomes do cmdlets (por exemplo, `New-AzureRmVM` => `New-AzVm`) e os nomes dos parâmetros (por exemplo, `-ResourceGroupName` => `-Rg`).</span><span class="sxs-lookup"><span data-stu-id="a40a3-136">Shorter Names - Includes the names of cmdlets (for example, `New-AzureRmVM` => `New-AzVm`) and the names of parameters (for example, `-ResourceGroupName` => `-Rg`).</span></span> <span data-ttu-id="a40a3-137">Utilize aliases para compatibilidade com os cmdlets “antigos”.</span><span class="sxs-lookup"><span data-stu-id="a40a3-137">Use aliases for compatibility with "old" cmdlets.</span></span> <span data-ttu-id="a40a3-138">Forneça conjuntos de parâmetros _retrocompatíveis_.</span><span class="sxs-lookup"><span data-stu-id="a40a3-138">Provide _backwards compatible_ parameter sets.</span></span>

- <span data-ttu-id="a40a3-139">Predefinições inteligentes - crie predefinições inteligentes para preencher informações “obrigatórias”.</span><span class="sxs-lookup"><span data-stu-id="a40a3-139">Smart Defaults - Create smart defaults to fill in "required" information.</span></span> <span data-ttu-id="a40a3-140">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="a40a3-140">For example:</span></span>
  - <span data-ttu-id="a40a3-141">Grupo de Recursos</span><span class="sxs-lookup"><span data-stu-id="a40a3-141">Resource Group</span></span>
  - <span data-ttu-id="a40a3-142">Localização</span><span class="sxs-lookup"><span data-stu-id="a40a3-142">Location</span></span>
  - <span data-ttu-id="a40a3-143">Recursos dependentes</span><span class="sxs-lookup"><span data-stu-id="a40a3-143">Dependent resources</span></span>

### <a name="experimental-improvements"></a><span data-ttu-id="a40a3-144">Melhorias experimentais</span><span class="sxs-lookup"><span data-stu-id="a40a3-144">Experimental improvements</span></span>

<span data-ttu-id="a40a3-145">As melhorias experimentais apresentam uma alteração significativa que a equipa pretende validar através de experimentação.</span><span class="sxs-lookup"><span data-stu-id="a40a3-145">The experimental improvements present a significant change that the team wants to validate via experimentation.</span></span>

- <span data-ttu-id="a40a3-146">Tipos simples - a criação de cenários deve afastar-se de tipos complexos e objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="a40a3-146">Simple types - Create scenarios should move away from complex types and config objects.</span></span> <span data-ttu-id="a40a3-147">Simplifique a configuração para um ou dois parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a40a3-147">Simplify the configuration down to one or two parameters.</span></span>

- <span data-ttu-id="a40a3-148">“Criação Inteligente” - todos os cenários de criação que implementam a “Criação Inteligente” _não_ deviam ter parâmetros obrigatórios: todas as informações necessárias seriam escolhidas pelo Azure PowerShell, de forma opinativa.</span><span class="sxs-lookup"><span data-stu-id="a40a3-148">"Smart Create" - All create scenarios implementing "Smart Create" would have _no_ required parameters: all necessary information would be chosen by Azure PowerShell in an opinionated fashion.</span></span>

- <span data-ttu-id="a40a3-149">Parâmetros Cinzentos - em muitos casos, alguns parâmetros podem ser “cinzentos” ou semi-opcionais.</span><span class="sxs-lookup"><span data-stu-id="a40a3-149">Gray Parameters - In many cases, some parameters could be "gray" or semi-optional.</span></span> <span data-ttu-id="a40a3-150">Se o parâmetro não for especificado, é perguntado ao utilizador se pretende que o parâmetro seja gerado.</span><span class="sxs-lookup"><span data-stu-id="a40a3-150">If the parameter is not specified, the user is asked if they want the parameter generated for them.</span></span> <span data-ttu-id="a40a3-151">Também faz sentido que os parâmetros cinzentos infiram um valor baseado no contexto, com o consentimento do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a40a3-151">It also makes sense for gray parameters to infer a value based on context with the user's consent.</span></span>
  <span data-ttu-id="a40a3-152">Por exemplo, faz sentido que o parâmetro cinzento sugira o valor mais recentemente utilizado.</span><span class="sxs-lookup"><span data-stu-id="a40a3-152">For example, it may make sense to have the gray parameter suggest the most recently used value.</span></span>

- <span data-ttu-id="a40a3-153">Comutador `-Auto` - o comutador `-Auto` iria fornecer uma forma de “opt-in” para os utilizadores _predefinirem todos os aspetos_, mantendo a integridade dos parâmetros obrigatórios no caminho da linha principal.</span><span class="sxs-lookup"><span data-stu-id="a40a3-153">`-Auto` Switch - The `-Auto` switch would provide an "opt-in" way for users to _default all the things_ while maintaining the integrity of required parameters in the mainline path.</span></span>

### <a name="feature-specific-switches"></a><span data-ttu-id="a40a3-154">Comutadores específicos de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a40a3-154">Feature-specific switches</span></span>

<span data-ttu-id="a40a3-155">Por exemplo, o cenário “Criar aplicação Web” poderia ter um comutador `-Git` ou `-AddRemote` que iria adicionar automaticamente um “azure” remoto a um repositório existente do git.</span><span class="sxs-lookup"><span data-stu-id="a40a3-155">For example, the "Create web app" scenario might have a `-Git` or `-AddRemote` switch that would automatically add an "azure" remote to an existing git repository.</span></span>

- <span data-ttu-id="a40a3-156">Predefinições Definíveis - os utilizadores devem ter a capacidade de predefinir determinados parâmetros gerais como `-ResourceGroupName` e `-Location`.</span><span class="sxs-lookup"><span data-stu-id="a40a3-156">Settable Defaults - Users should have the ability to default certain ubiquitous parameters like `-ResourceGroupName` and `-Location`.</span></span>

- <span data-ttu-id="a40a3-157">Predefinições de Tamanho - os “tamanhos” dos recursos podem ser confusos para os utilizadores, uma vez que muitos Fornecedores de Recursos utilizam nomes diferentes (por exemplo, “Standard\_DS1\_v2” ou “S1”).</span><span class="sxs-lookup"><span data-stu-id="a40a3-157">Size Defaults - Resource "sizes" can be confusing to users since many Resource Providers use different names (for example, "Standard\_DS1\_v2" or "S1").</span></span> <span data-ttu-id="a40a3-158">No entanto, a maioria dos utilizadores preocupa-se mais com o custo.</span><span class="sxs-lookup"><span data-stu-id="a40a3-158">However, most users care more about cost.</span></span> <span data-ttu-id="a40a3-159">Por conseguinte, faz sentido definir tamanhos “universais”, com base num agendamento de preços.</span><span class="sxs-lookup"><span data-stu-id="a40a3-159">Therefore, it makes sense to define "universal" sizes based on a pricing schedule.</span></span> <span data-ttu-id="a40a3-160">Os utilizadores podem escolher um tamanho específico ou permitir que o Azure PowerShell escolha a _melhor opção_ com base no orçamento para recursos.</span><span class="sxs-lookup"><span data-stu-id="a40a3-160">Users can choose a specific size or let Azure PowerShell choose the _best option_ based on the resource the budget.</span></span>

- <span data-ttu-id="a40a3-161">Formato de Saída - atualmente, o Azure PowerShell devolve `PSObject`s e há pouca saída da consola.</span><span class="sxs-lookup"><span data-stu-id="a40a3-161">Output Format - Azure PowerShell currently returns `PSObject`s and there is little console output.</span></span> <span data-ttu-id="a40a3-162">O Azure PowerShell poderá ter de apresente algumas informações ao utilizador sobre as “predefinições inteligentes” utilizadas.</span><span class="sxs-lookup"><span data-stu-id="a40a3-162">Azure PowerShell may need to display some information to the user regarding the "smart defaults" used.</span></span>

## <a name="try-using-the-experiments"></a><span data-ttu-id="a40a3-163">Tente utilizar as experimentações</span><span class="sxs-lookup"><span data-stu-id="a40a3-163">Try using the experiments</span></span>

### <a name="install"></a><span data-ttu-id="a40a3-164">Instalar</span><span class="sxs-lookup"><span data-stu-id="a40a3-164">Install</span></span>

```powershell
Install-Module AzureRM.Compute.Experiments
```

### <a name="create-a-vm"></a><span data-ttu-id="a40a3-165">Criar uma VM</span><span class="sxs-lookup"><span data-stu-id="a40a3-165">Create a VM</span></span>

```powershell
$job = New-AzVm -Name MyVm -AsJob
Receive-Job $job
```

### <a name="send-us-feedback"></a><span data-ttu-id="a40a3-166">Envie-nos comentários</span><span class="sxs-lookup"><span data-stu-id="a40a3-166">Send us feedback</span></span>

```powershell
Send-Feedback
```

### <a name="uninstall-the-experimental-modules"></a><span data-ttu-id="a40a3-167">Desinstalar os módulos experimentais</span><span class="sxs-lookup"><span data-stu-id="a40a3-167">Uninstall the experimental modules</span></span>

```powershell
Uninstall-Module AzureRM.Compute.Experiments
```