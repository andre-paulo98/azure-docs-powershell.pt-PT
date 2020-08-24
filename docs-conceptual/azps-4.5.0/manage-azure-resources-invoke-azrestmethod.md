---
title: Gerir recursos do Azure com o Invoke-AzRestMethod
description: Como utilizar o Azure PowerShell para gerir recursos com o cmdlet Invoke-AzRestMethod.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/17/2020
ms.openlocfilehash: 380fd818a3af2474ce192c7a1da8a6798795cf21
ms.sourcegitcommit: bd7edc4d48b6a8a8bec864edc876e16af0a49505
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/18/2020
ms.locfileid: "88512994"
---
# <a name="manage-azure-resources-with-invoke-azrestmethod"></a><span data-ttu-id="2c72e-103">Gerir recursos do Azure com o Invoke-AzRestMethod</span><span class="sxs-lookup"><span data-stu-id="2c72e-103">Manage Azure resources with Invoke-AzRestMethod</span></span>

<span data-ttu-id="2c72e-104">O [Invoke-AzRestMethod](/powershell/module/az.accounts/invoke-azrestmethod) é um cmdlet do Azure PowerShell que foi introduzido na versão 4.4.0 do módulo Az do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2c72e-104">[Invoke-AzRestMethod](/powershell/module/az.accounts/invoke-azrestmethod) is an Azure PowerShell cmdlet that was introduced in Az PowerShell module version 4.4.0.</span></span> <span data-ttu-id="2c72e-105">Permite-lhe fazer pedidos HTTP personalizados ao ponto final do Azure Resource Manager (ARM) com o contexto do Az.</span><span class="sxs-lookup"><span data-stu-id="2c72e-105">It allows you to make custom HTTP requests to the Azure Resource Management (ARM) endpoint using the Az context.</span></span>

<span data-ttu-id="2c72e-106">Este cmdlet é útil quando quer gerir os serviços do Azure no que respeita funcionalidades que ainda não estão disponíveis no módulo Az do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2c72e-106">This cmdlet is useful when you want to manage Azure services for features that aren't yet available in the Az PowerShell module.</span></span>

## <a name="how-to-use-invoke-azrestmethod"></a><span data-ttu-id="2c72e-107">Como utilizar o Invoke-AzRestMethod</span><span class="sxs-lookup"><span data-stu-id="2c72e-107">How to use Invoke-AzRestMethod</span></span>

<span data-ttu-id="2c72e-108">A título de exemplo, pode permitir o acesso ao Azure Container Registry (ACR) apenas para redes específicas ou recusar o acesso público.</span><span class="sxs-lookup"><span data-stu-id="2c72e-108">As an example, you can allow access to Azure Container Registry (ACR) only for specific networks or deny public access.</span></span> <span data-ttu-id="2c72e-109">Esta funcionalidade ainda não está disponível no [módulo Az.ContainerRegistry do PowerShell](/powershell/module/Az.ContainerRegistry/).</span><span class="sxs-lookup"><span data-stu-id="2c72e-109">This feature isn't available yet in the [Az.ContainerRegistry PowerShell module](/powershell/module/Az.ContainerRegistry/).</span></span>
<span data-ttu-id="2c72e-110">No entanto, pode geri-la provisoriamente com o `Invoke-AzRestMethod`.</span><span class="sxs-lookup"><span data-stu-id="2c72e-110">However, it can be managed in the interim with `Invoke-AzRestMethod`.</span></span>

## <a name="using-invoke-azrestmethod-with-get-operations"></a><span data-ttu-id="2c72e-111">Utilizar o Invoke-AzRestMethod com operações GET</span><span class="sxs-lookup"><span data-stu-id="2c72e-111">Using Invoke-AzRestMethod with GET operations</span></span>

<span data-ttu-id="2c72e-112">O exemplo seguinte demonstra como utilizar o cmdlet `Invoke-AzRestMethod` com uma operação GET:</span><span class="sxs-lookup"><span data-stu-id="2c72e-112">The following example demonstrates how to use the `Invoke-AzRestMethod` cmdlet with a GET operation:</span></span>

```azurepowershell-interactive
$getParams = @{
  ResourceGroupName = 'myresourcegroup'
  ResourceProviderName = 'Microsoft.ContainerRegistry'
  ResourceType = 'registries'
  Name = 'myacr'
  ApiVersion = '2019-12-01-preview'
  Method = 'GET'
}
Invoke-AzRestMethod @getParams
```

<span data-ttu-id="2c72e-113">Para permitir a máxima flexibilidade, a maioria dos parâmetros de `Invoke-AzRestMethod` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="2c72e-113">To allow maximum flexibility, most of the parameters for `Invoke-AzRestMethod` are optional.</span></span>
<span data-ttu-id="2c72e-114">Contudo, quando estiver a gerir recursos num grupo de recursos, é provável que precise de fornecer o ID completo do recurso ou parâmetros como o grupo de recursos, fornecedor de recursos e tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="2c72e-114">However, when you're managing resources within a resource group, you'll most likely need to provide either the full ID to the resource or parameters like resource group, resource provider, and resource type.</span></span>

<span data-ttu-id="2c72e-115">Os parâmetros `ResourceType` e `Name` podem receber vários valores ao visar recursos que precisem de mais do que um nome.</span><span class="sxs-lookup"><span data-stu-id="2c72e-115">The `ResourceType` and `Name` parameters can take multiple values when targeting resources that require more than one name.</span></span> <span data-ttu-id="2c72e-116">Por exemplo, para manipular uma pesquisa guardada numa área de trabalho do Log Analytics, os parâmetros serão semelhantes ao exemplo seguinte: `-ResourceType @('workspaces', 'savedsearches') -Name @('my-la', 'my-search')`.</span><span class="sxs-lookup"><span data-stu-id="2c72e-116">For example, to manipulate a saved search in a Log Analytics workspace, the parameters look like the following example: `-ResourceType @('workspaces', 'savedsearches') -Name @('my-la', 'my-search')`.</span></span>

<span data-ttu-id="2c72e-117">Através de um mapeamento baseado na posição na matriz, o cmdlet constrói o seguinte recurso: `Id:'/workspaces/my-la/savedsearches/my-search'`.</span><span class="sxs-lookup"><span data-stu-id="2c72e-117">Using a mapping based on the position in the array, the cmdlet constructs the following resource: `Id:'/workspaces/my-la/savedsearches/my-search'`.</span></span>

<span data-ttu-id="2c72e-118">O parâmetro `APIVersion` permite-lhe utilizar uma versão de API específica, incluindo as versões de pré-visualização.</span><span class="sxs-lookup"><span data-stu-id="2c72e-118">The `APIVersion` parameter allows you to use a specific API version, including preview ones.</span></span> <span data-ttu-id="2c72e-119">As versões de API suportadas para Fornecedores de recursos do Azure podem ser encontradas no repositório do GitHub [azure-rest-api-specs](https://github.com/Azure/azure-rest-api-specs).</span><span class="sxs-lookup"><span data-stu-id="2c72e-119">The supported API versions for Azure Resource providers can be found in the [azure-rest-api-specs](https://github.com/Azure/azure-rest-api-specs) GitHub repository.</span></span>

<span data-ttu-id="2c72e-120">Pode encontrar a definição da versão 2019-12-01-preview do ACR na localização seguinte: [azure-rest-api-specs/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview/](https://github.com/Azure/azure-rest-api-specs/tree/master/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview).</span><span class="sxs-lookup"><span data-stu-id="2c72e-120">You can find the definition for the 2019-12-01-preview version of ACR in the following location: [azure-rest-api-specs/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview/](https://github.com/Azure/azure-rest-api-specs/tree/master/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview).</span></span>

## <a name="using-invoke-azrestmethod-with-patch-operations"></a><span data-ttu-id="2c72e-121">Utilizar o Invoke-AzRestMethod com operações PATCH</span><span class="sxs-lookup"><span data-stu-id="2c72e-121">Using Invoke-AzRestMethod with PATCH operations</span></span>

<span data-ttu-id="2c72e-122">Pode desativar o acesso público ao ACR existente com o nome `myacr` no grupo de recursos `myresourcegroup` com o cmdlet Invoke-AzRestMethod.</span><span class="sxs-lookup"><span data-stu-id="2c72e-122">You can disable public access to the existing ACR named `myacr` in the `myresourcegroup` resource group using the Invoke-AzRestMethod cmdlet.</span></span>

<span data-ttu-id="2c72e-123">Para desativar o acesso de rede pública, tem de fazer uma chamada **PATCH** à API que altera o valor do parâmetro `publicNetwokAccess`, conforme demonstrado no exemplo seguinte:</span><span class="sxs-lookup"><span data-stu-id="2c72e-123">To disable the public network access, you need to make a **PATCH** call to the API that changes the value of the `publicNetwokAccess` parameter as shown in the following example:</span></span>

```azurepowershell-interactive
$patchParams = @{
  ResourceGroupName = 'myresourcegroup'
  Name = 'myacr'
  ResourceProviderName = 'Microsoft.ContainerRegistry'
  ResourceType = 'registries'
  ApiVersion = '2019-12-01-preview'
  Payload = '{ "properties": {
     "publicNetworkAccess": "Disabled"
     } }'
  Method = 'PATCH'
}
Invoke-AzRestMethod @patchParams
```

<span data-ttu-id="2c72e-124">A propriedade `Payload` é uma cadeia de carateres JSON que mostra o caminho da propriedade a ser modificada.</span><span class="sxs-lookup"><span data-stu-id="2c72e-124">The `Payload` property is a JSON string that shows the path of the property to be modified.</span></span>

<span data-ttu-id="2c72e-125">Todos os parâmetros desta API estão descritos no ficheiro **rest-api-spec** associado a esta API.</span><span class="sxs-lookup"><span data-stu-id="2c72e-125">All the parameters for this API are described in the **rest-api-spec** file associated with this API.</span></span>
<span data-ttu-id="2c72e-126">A definição específica do parâmetro publicNetworkAccess pode ser encontrada no [ficheiro JSON do registo de contentor](https://github.com/Azure/azure-rest-api-specs/blob/2a9da9a79d0a7b74089567ec4f0289f3e0f31bec/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview/2019-12-01-preview/containerregistry.json) da versão de pré-visualização 2019-12-01 da API.</span><span class="sxs-lookup"><span data-stu-id="2c72e-126">The specific definition for the publicNetworkAccess parameter can be found in the [container registry JSON file](https://github.com/Azure/azure-rest-api-specs/blob/2a9da9a79d0a7b74089567ec4f0289f3e0f31bec/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview/2019-12-01-preview/containerregistry.json) for the 2019-12-01 preview version of the API.</span></span>

<span data-ttu-id="2c72e-127">Para permitir o acesso apenas ao registo a partir de um endereço IP específico, o payload tem de ser modificado, conforme demonstrado no exemplo seguinte:</span><span class="sxs-lookup"><span data-stu-id="2c72e-127">To only allow access to the registry from a specific IP address, the payload needs to be modified as shown in the following example:</span></span>

```azurepowershell-interactive
$specificIpParams = @{
  ResourceGroupName = 'myresourcegroup'
  Name = 'myacr'
  ResourceProviderName = 'Microsoft.ContainerRegistry'
  ResourceType = 'registries'
  ApiVersion = '2019-12-01-preview'
  Payload = '{ "properties": {
      "networkRuleSet": {
      "defaultAction": "Deny",
      "ipRules": [ {
         "action": "Allow",
         "value": "24.22.123.123"
         } ]
      }
  } }'
  -Method = 'PATCH'
}
Invoke-AzRestMethod @specificIpParams
```

## <a name="comparison-to-get-azresource-new-azresource-and-remove-azresource"></a><span data-ttu-id="2c72e-128">Comparação com o Get-AzResource, New-AzResource e Remove-AzResource</span><span class="sxs-lookup"><span data-stu-id="2c72e-128">Comparison to Get-AzResource, New-AzResource, and Remove-AzResource</span></span>

<span data-ttu-id="2c72e-129">Os cmdlets `*-AzResource` permitem-lhe personalizar a chamada à API REST para o Azure ao especificar o tipo de recurso, a versão da API e as propriedades a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="2c72e-129">The `*-AzResource` cmdlets allow you to customize the REST API call to Azure by specifying the resource type, the API version, and the properties to be updated.</span></span> <span data-ttu-id="2c72e-130">No entanto, as propriedades têm de ser um `PSObject`, pelo que podem tornar-se facilmente mais complicadas de criar.</span><span class="sxs-lookup"><span data-stu-id="2c72e-130">However, the properties need to be a `PSObject` that can easily become complicated to create.</span></span>

<span data-ttu-id="2c72e-131">`Invoke-AzRestMethod` oferece uma maneira mais simples de gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="2c72e-131">`Invoke-AzRestMethod` offers a simpler way to manage Azure resources.</span></span> <span data-ttu-id="2c72e-132">No exemplo anterior, pode ver que o payload é uma cadeia de carateres JSON.</span><span class="sxs-lookup"><span data-stu-id="2c72e-132">In the previous example, you can see that the payload is a JSON string.</span></span> <span data-ttu-id="2c72e-133">Não precisa de ter dificuldades na conversão entre JSON e `PSObjects`.</span><span class="sxs-lookup"><span data-stu-id="2c72e-133">You don't have to struggle with the conversion between JSON and `PSObjects`.</span></span>

<span data-ttu-id="2c72e-134">Se já estiver familiarizado com os cmdlets `*-AzResource`, pode continuar a utilizá-los.</span><span class="sxs-lookup"><span data-stu-id="2c72e-134">If you're already familiar with the `*-AzResource` cmdlets, you can continue using them.</span></span> <span data-ttu-id="2c72e-135">Não planeamos descontinuar o suporte para estes cmdlets.</span><span class="sxs-lookup"><span data-stu-id="2c72e-135">We have no plans to stop supporting them.</span></span> <span data-ttu-id="2c72e-136">Com `Invoke-AzRestMethod`, adicionámos um novo cmdlet à família.</span><span class="sxs-lookup"><span data-stu-id="2c72e-136">With `Invoke-AzRestMethod`, we have added a new cmdlet to the family.</span></span>

## <a name="see-also"></a><span data-ttu-id="2c72e-137">Consulte também</span><span class="sxs-lookup"><span data-stu-id="2c72e-137">See Also</span></span>

* [<span data-ttu-id="2c72e-138">Get-AzResource</span><span class="sxs-lookup"><span data-stu-id="2c72e-138">Get-AzResource</span></span>](/powershell/module/az.resources/get-azresource)
* [<span data-ttu-id="2c72e-139">New-AzResource</span><span class="sxs-lookup"><span data-stu-id="2c72e-139">New-AzResource</span></span>](/powershell/module/az.resources/new-azresource)
* [<span data-ttu-id="2c72e-140">Remove-AzResource</span><span class="sxs-lookup"><span data-stu-id="2c72e-140">Remove-AzResource</span></span>](/powershell/module/az.resources/remove-azresource)
