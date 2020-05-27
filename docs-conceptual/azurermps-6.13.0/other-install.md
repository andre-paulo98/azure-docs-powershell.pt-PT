---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell sem o PowerShellGet utilizar um MSI
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: e1d8877c185b4537c476128e279eda563f2575d1
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83385869"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a>Instalar o Azure PowerShell no Windows com o MSI

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

Este artigo explica como instalar o Azure PowerShell no Windows com um Instalador do MSI.  
Utilize estes métodos de instalação apenas se forem necessários para o seu sistema. A forma recomendada para instalar o Azure PowerShell no Windows é com o PowerShellGet. Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).

> [!NOTE]
> O método de instalação do Instalador de Plataforma Web já não está disponível para as versões 6.x e superiores do Azure PowerShell. Se precisar de utilizar o Instalador de Plataforma Web, considere utilizar o MSI em alternativa ou instale uma versão anterior do Azure PowerShell.

## <a name="install-or-update-on-windows-using-the-msi-package"></a>Instalar ou atualizar no Windows com o Pacote MSI

O Azure PowerShell para o Windows PowerShell 5.x pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v6.13.1-November2018). Se tiver instalado as versões anteriores dos módulos do Azure como um MSI, o instalador remove-as automaticamente. O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`. Ambos os módulos `AzureRM` e `Azure` são instalados.

> [!NOTE]
> Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.

Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
>
> Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module AzureRM`. Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.

Terá de repetir este passo para cada nova sessão do PowerShell que iniciar. Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).
