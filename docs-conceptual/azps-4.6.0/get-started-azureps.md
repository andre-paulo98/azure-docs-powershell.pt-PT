---
title: Introdução ao Azure PowerShell
description: ''
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 04/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 6281ac5f6ec8941e0d5c1755f90f99552db9aa92
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89242261"
---
# <a name="get-started-with-azure-powershell"></a>Introdução ao Azure PowerShell

O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos.
Utilize o Azure PowerShell para criar ferramentas automatizadas que utilizem o modelo do Azure Resource Manager. Experimente no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou instale-o no seu computador local.

Este artigo ajuda-o a começar a utilizar o Azure PowerShell e explica os principais conceitos que lhe estão subjacentes.

## <a name="install-or-run-in-azure-cloud-shell"></a>Instalar ou executar no Azure Cloud Shell

A maneira mais fácil de começar a utilizar o Azure PowerShell é experimentá-lo num ambiente do Azure Cloud Shell. Para ficar operacional com o Cloud Shell, veja [Início Rápido do PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell). O Cloud Shell executa o PowerShell num contentor do Linux, pelo que a funcionalidade específica do Windows não está disponível.

Quando estiver pronto para instalar o Azure PowerShell no seu computador local, siga as instruções em [Instalar o módulo do Azure PowerShell](install-az-ps.md).

## <a name="sign-in-to-azure"></a>Iniciar sessão no Azure

Inicie sessão interativamente com o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount). Se utilizar o Cloud Shell, ignore este passo. a sua sessão do Azure Cloud Shell já foi autenticada para o ambiente, a subscrição e o inquilino que iniciou a sessão do Cloud Shell.

```azurepowershell-interactive
Connect-AzAccount
```

Os serviços cloud do Azure oferecem ambientes em conformidade com as leis de processamento de dados regionais. Para contas numa cloud regional, utilize o parâmetro **Environment** para iniciar sessão. Obtenha o nome do ambiente para a sua região através do cmdlet [Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment).
Por exemplo, para iniciar sessão no Azure China 21Vianet:

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

Nos ambientes do Windows PowerShell 5.1, receberá uma caixa de diálogo de início de sessão que lhe pedirá o nome de utilizador e a palavra-passe da sua conta do Azure. Em todas as outras versões do PowerShell, obterá um token para utilizar em [microsoft.com/devicelogin](https://microsoft.com/devicelogin). Abra esta página no seu browser e introduza o token, inicie sessão com as suas credenciais de conta do Azure e autorize o Azure PowerShell.

Depois de iniciar sessão, são apresentadas informações que indicam qual das subscrições do Azure se encontra ativa. Se tiver várias subscrições do Azure na sua conta e quiser selecionar uma diferente, obtenha as subscrições disponíveis com [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) e utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext) com o ID da subscrição. Para obter mais informações sobre como gerir as suas subscrições do Azure no Azure PowerShell, veja [Use multiple Azure subscriptions](manage-subscriptions-azureps.md) (Utilizar várias subscrições do Azure).

Assim que tiver iniciado sessão, utilize os cmdlets do Azure PowerShell para aceder e gerir recursos na sua subscrição. Para saber mais sobre o processo de início de sessão e os métodos de autenticação, veja [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md).

## <a name="find-commands"></a>Encontrar comandos

Os cmdlets do Azure PowerShell seguem uma convenção de nomenclatura padrão para o PowerShell: `Verb-Noun`. O verbo descreve a ação (os exemplos incluem `New`, `Get`, `Set`, `Remove`) e o substantivo descreve o tipo de recurso (os exemplos incluem `AzVM`, `AzKeyVaultCertificate`, `AzFirewall`, `AzVirtualNetworkGateway`). Os substantivos no Azure PowerShell começam sempre com o prefixo `Az`. Para obter a lista completa dos verbos padrão, veja [Verbos aprovados para os Comandos do PowerShell](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands).

Saber os substantivos, verbos e módulos do Azure PowerShell disponíveis ajuda-o a encontrar os comandos com o cmdlet [Get-Command](/powershell/module/microsoft.powershell.core/get-command). Por exemplo, para encontrar todos os comandos relacionados com VMs que utilizem o verbo `Get`:

```powershell-interactive
Get-Command -Verb Get -Noun AzVM* -Module Az.Compute
```

Para o ajudar a encontrar os comandos comuns, esta tabela lista o tipo de recurso, o módulo correspondente do Azure PowerShell e o prefixo do substantivo a utilizar com `Get-Command`:

|                              Tipo de recurso                              |                   Módulo do Azure PowerShell                    |    Prefixo do substantivo     |
| ----------------------------------------------------------------------- | ------------------------------------------------------------ | ------------------ |
| [Grupo de recursos](/azure/azure-resource-manager/resource-group-overview) | [Az.Resources](/powershell/module/az.resources#resources)    | `AzResourceGroup`  |
| [Máquinas virtuais](/azure/virtual-machines)                             | [Az.Compute](/powershell/module/az.compute#virtual_machines) | `AzVM`             |
| [Contas de armazenamento](/azure/storage/common/storage-introduction)          | [Az.Storage](/powershell/module/az.storage/)                 | `AzStorageAccount` |
| [Cofre de Chaves](/azure/key-vault/key-vault-whatis)                          | [Az.KeyVault](/powershell/module/az.keyvault)                | `AzKeyVault`       |
| [Aplicações Web](/azure/app-service)                                  | [Az.Websites](/powershell/module/az.websites)                | `AzWebApp`         |
| [Bases de Dados SQL](/azure/sql-database)                                    | [Az.Sql](/powershell/module/az.sql)                          | `AzSqlDatabase`    |

Para obter uma lista completa dos módulos no Azure PowerShell, veja a [lista de módulos do Azure PowerShell](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md) alojados no GitHub.

## <a name="telemetry"></a>Telemetria

O Azure PowerShell recolhe automaticamente dados telemétricos por predefinição. A Microsoft agrega os dados recolhidos para identificar padrões de utilização, identificar problemas comuns e melhorar a experiência do Azure PowerShell. O Microsoft Azure PowerShell não recolhe quaisquer dados pessoais ou privados. Para desativar a recolha de dados, tem de optar explicitamente por executar [Disable-AzDataCollection](/powershell/module/az.accounts/disable-azdatacollection).

## <a name="learn-azure-powershell-basics-with-quickstarts-and-tutorials"></a>Aprender as noções básicas do Azure PowerShell com inícios rápidos e tutoriais

Para começar a utilizar o Azure PowerShell, experimente um tutorial aprofundado sobre como configurar máquinas virtuais e como as consultar.

> [!div class="nextstepaction"]
> [Criar máquinas virtuais com o Azure PowerShell](azureps-vm-tutorial.yml)

Também existem inícios rápidos do Azure PowerShell para outros serviços populares do Azure:

* [Criar uma conta de armazenamento](/azure/storage/common/storage-quickstart-create-account?tabs=azure-powershell)
* [Transferir objetos de/para o armazenamento de Blobs do Azure](/azure/storage/blobs/storage-quickstart-blobs-powershell)
* [Criar e obter segredos do Azure Key Vault](/azure/key-vault/quick-create-powershell)
* [Criar uma firewall e base de dados SQL do Azure](/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell)
* [Executar um contentor no Azure Container Instances](/azure/container-instances/container-instances-quickstart-powershell)
* [Criar um Conjunto de Dimensionamento de Máquinas Virtuais](/azure/virtual-machine-scale-sets/quick-create-powershell)
* [Criar um balanceador de carga standard](/azure/load-balancer/quickstart-create-standard-load-balancer-powershell)

## <a name="next-steps"></a>Passos seguintes

* [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md)
* [Gerir subscrições do Azure com o Azure PowerShell](manage-subscriptions-azureps.md)
* [Criar principais de serviço com o Azure PowerShell](create-azure-service-principal-azureps.md)
* Obter ajuda da comunidade:
  * [Fórum do Azure no MSDN](https://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [Stack Overflow](https://go.microsoft.com/fwlink/?LinkId=320213)
