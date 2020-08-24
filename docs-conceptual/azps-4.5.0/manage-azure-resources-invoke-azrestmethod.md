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
# <a name="manage-azure-resources-with-invoke-azrestmethod"></a>Gerir recursos do Azure com o Invoke-AzRestMethod

O [Invoke-AzRestMethod](/powershell/module/az.accounts/invoke-azrestmethod) é um cmdlet do Azure PowerShell que foi introduzido na versão 4.4.0 do módulo Az do PowerShell. Permite-lhe fazer pedidos HTTP personalizados ao ponto final do Azure Resource Manager (ARM) com o contexto do Az.

Este cmdlet é útil quando quer gerir os serviços do Azure no que respeita funcionalidades que ainda não estão disponíveis no módulo Az do PowerShell.

## <a name="how-to-use-invoke-azrestmethod"></a>Como utilizar o Invoke-AzRestMethod

A título de exemplo, pode permitir o acesso ao Azure Container Registry (ACR) apenas para redes específicas ou recusar o acesso público. Esta funcionalidade ainda não está disponível no [módulo Az.ContainerRegistry do PowerShell](/powershell/module/Az.ContainerRegistry/).
No entanto, pode geri-la provisoriamente com o `Invoke-AzRestMethod`.

## <a name="using-invoke-azrestmethod-with-get-operations"></a>Utilizar o Invoke-AzRestMethod com operações GET

O exemplo seguinte demonstra como utilizar o cmdlet `Invoke-AzRestMethod` com uma operação GET:

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

Para permitir a máxima flexibilidade, a maioria dos parâmetros de `Invoke-AzRestMethod` são opcionais.
Contudo, quando estiver a gerir recursos num grupo de recursos, é provável que precise de fornecer o ID completo do recurso ou parâmetros como o grupo de recursos, fornecedor de recursos e tipo de recurso.

Os parâmetros `ResourceType` e `Name` podem receber vários valores ao visar recursos que precisem de mais do que um nome. Por exemplo, para manipular uma pesquisa guardada numa área de trabalho do Log Analytics, os parâmetros serão semelhantes ao exemplo seguinte: `-ResourceType @('workspaces', 'savedsearches') -Name @('my-la', 'my-search')`.

Através de um mapeamento baseado na posição na matriz, o cmdlet constrói o seguinte recurso: `Id:'/workspaces/my-la/savedsearches/my-search'`.

O parâmetro `APIVersion` permite-lhe utilizar uma versão de API específica, incluindo as versões de pré-visualização. As versões de API suportadas para Fornecedores de recursos do Azure podem ser encontradas no repositório do GitHub [azure-rest-api-specs](https://github.com/Azure/azure-rest-api-specs).

Pode encontrar a definição da versão 2019-12-01-preview do ACR na localização seguinte: [azure-rest-api-specs/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview/](https://github.com/Azure/azure-rest-api-specs/tree/master/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview).

## <a name="using-invoke-azrestmethod-with-patch-operations"></a>Utilizar o Invoke-AzRestMethod com operações PATCH

Pode desativar o acesso público ao ACR existente com o nome `myacr` no grupo de recursos `myresourcegroup` com o cmdlet Invoke-AzRestMethod.

Para desativar o acesso de rede pública, tem de fazer uma chamada **PATCH** à API que altera o valor do parâmetro `publicNetwokAccess`, conforme demonstrado no exemplo seguinte:

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

A propriedade `Payload` é uma cadeia de carateres JSON que mostra o caminho da propriedade a ser modificada.

Todos os parâmetros desta API estão descritos no ficheiro **rest-api-spec** associado a esta API.
A definição específica do parâmetro publicNetworkAccess pode ser encontrada no [ficheiro JSON do registo de contentor](https://github.com/Azure/azure-rest-api-specs/blob/2a9da9a79d0a7b74089567ec4f0289f3e0f31bec/specification/containerregistry/resource-manager/Microsoft.ContainerRegistry/preview/2019-12-01-preview/containerregistry.json) da versão de pré-visualização 2019-12-01 da API.

Para permitir o acesso apenas ao registo a partir de um endereço IP específico, o payload tem de ser modificado, conforme demonstrado no exemplo seguinte:

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

## <a name="comparison-to-get-azresource-new-azresource-and-remove-azresource"></a>Comparação com o Get-AzResource, New-AzResource e Remove-AzResource

Os cmdlets `*-AzResource` permitem-lhe personalizar a chamada à API REST para o Azure ao especificar o tipo de recurso, a versão da API e as propriedades a serem atualizadas. No entanto, as propriedades têm de ser um `PSObject`, pelo que podem tornar-se facilmente mais complicadas de criar.

`Invoke-AzRestMethod` oferece uma maneira mais simples de gerir os recursos do Azure. No exemplo anterior, pode ver que o payload é uma cadeia de carateres JSON. Não precisa de ter dificuldades na conversão entre JSON e `PSObjects`.

Se já estiver familiarizado com os cmdlets `*-AzResource`, pode continuar a utilizá-los. Não planeamos descontinuar o suporte para estes cmdlets. Com `Invoke-AzRestMethod`, adicionámos um novo cmdlet à família.

## <a name="see-also"></a>Consulte também

* [Get-AzResource](/powershell/module/az.resources/get-azresource)
* [New-AzResource](/powershell/module/az.resources/new-azresource)
* [Remove-AzResource](/powershell/module/az.resources/remove-azresource)
