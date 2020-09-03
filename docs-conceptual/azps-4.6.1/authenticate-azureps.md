---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 7/7/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 8f18af8ed67ecf2aefd353208c07bf812df732d9
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89242176"
---
# <a name="sign-in-with-azure-powershell"></a>Iniciar sessão com o Azure PowerShell

O Azure PowerShell suporta vários métodos de autenticação. O [Azure Cloud Shell](/azure/cloud-shell/overview) é a forma mais fácil de começar, uma vez que regista automaticamente o utilizador. Com uma instalação local, pode iniciar sessão interativamente através do browser. Ao escrever scripts para automatização, a abordagem recomendada é utilizar um [principal de serviço](create-azure-service-principal-azureps.md) com as permissões necessárias. Ao restringir as permissões de início de sessão tanto quanto possível para o seu caso de utilização, ajuda a manter os recursos do Azure seguros.

Inicialmente, a sua sessão é iniciada na primeira subscrição que o Azure devolve se tiver acesso a mais do que uma subscrição. Os comandos são executados em relação a esta subscrição por predefinição. Para alterar a subscrição ativa para uma sessão, utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext). Para alterar a sua subscrição ativa e fazer com que esta persista entre sessões no mesmo sistema, utilize o cmdlet [Select-AzContext](/powershell/module/az.accounts/select-azcontext).

> [!IMPORTANT]
> As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.
> Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).

## <a name="sign-in-interactively"></a>Iniciar sessão interativamente

Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).

```azurepowershell-interactive
Connect-AzAccount
```

Quando é executado a partir da versão 6 e versões superiores do PowerShell, este cmdlet apresenta uma cadeia de token. Para iniciar sessão, copie esta cadeia e cole-a em [microsoft.com/devicelogin](https://microsoft.com/devicelogin) num browser. A sua sessão do PowerShell será autenticada para se ligar ao Azure. Pode especificar o parâmetro `UseDeviceAuthentication` para receber uma cadeia de token no Windows PowerShell.

> [!IMPORTANT]
> A autorização de credenciais Nome de Utilizador/Palavra-passe foi removida no Azure PowerShell devido a alterações na implementação de autorizações do Active Directory e a preocupações relacionadas com segurança. Se utiliza a autorização de credenciais para fins de automatização, [crie um principal de serviço](create-azure-service-principal-azureps.md) como alternativa.

Utilize o cmdlet [Get-AzContext](/powershell/module/az.accounts/get-azcontext) para armazenar o seu ID de inquilino numa variável que irá ser utilizada nas duas secções seguintes deste artigo.

```azurepowershell-interactive
$tenantId = (Get-AzContext).Tenant.Id
```

## <a name="sign-in-with-a-service-principal"></a>Iniciar sessão com um principal de serviço<a name="sp-signin"/>

Os principais de serviço são contas não interativas do Azure. Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory. Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.

Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).

Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`. Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço. A forma como inicia sessão com um principal de serviço depende do facto de este estar configurado para a autenticação baseada em palavra-passe ou baseada em certificado.

### <a name="password-based-authentication"></a>Autenticação baseada em palavra-passe

Crie um principal de serviço que irá ser utilizado nos exemplos desta secção. Para mais informações sobre como criar principais de serviço, consulte [Criar um principal de serviço do Azure com o Azure PowerShell](/powershell/azure/create-azure-service-principal-azureps).

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential). Este cmdlet apresenta um pedido de nome de utilizador e palavra-passe. Utilize o `applicationID` do principal de serviço para o nome de utilizador e converta o respetivo `secret` em texto simples para a palavra-passe.

```azurepowershell-interactive
# Retrieve the plain text password for use with `Get-Credential` in the next command.
$sp.secret | ConvertFrom-SecureString -AsPlainText

$pscredential = Get-Credential -UserName $sp.ApplicationId
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

Para cenários de automatização, tem de criar as credenciais a partir de um `applicationId` e um `secret` do principal de serviço:

```azurepowershell-interactive
$pscredential = New-Object -TypeName System.Management.Automation.PSCredential($sp.ApplicationId, $sp.Secret)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

Certifique-se de que utiliza boas práticas de armazenamento de palavras-passe quando automatizar as ligações do principal de serviço.

### <a name="certificate-based-authentication"></a>Autenticação baseada em certificado

A autenticação baseada em certificado precisa que o Azure PowerShell tenha a capacidade de obter informações de um arquivo de certificados local com base num thumbprint do certificado.

```azurepowershell-interactive
Connect-AzAccount -ApplicationId $appId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

Ao utilizar um principal de serviço em vez de uma aplicação registada, adicione o argumento `-ServicePrincipal` e forneça o ID da Aplicação do principal de serviço como o valor do parâmetro `-ApplicationId`.

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -ApplicationId $servicePrincipalId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

No PowerShell 5.1, o arquivo de certificados pode ser gerido e inspecionado com o módulo de [PKI](/powershell/module/pkiclient). No PowerShell Core 6.x e versões posteriores, o processo é mais complexo. Os scripts que se seguem mostram como importar um certificado existente para o arquivo de certificados acessível ao PowerShell.

#### <a name="import-a-certificate-in-powershell-51"></a>Importar um certificado no PowerShell 5.1

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-core-6x-and-later"></a>Importar um certificado no PowerShell Core 6.x e versões posteriores

```azurepowershell-interactive
# Import a PFX
$storeName = [System.Security.Cryptography.X509Certificates.StoreName]::My
$storeLocation = [System.Security.Cryptography.X509Certificates.StoreLocation]::CurrentUser
$store = [System.Security.Cryptography.X509Certificates.X509Store]::new($storeName, $storeLocation)
$certPath = <path to certificate>
$credentials = Get-Credential -Message "Provide PFX private key password"
$flag = [System.Security.Cryptography.X509Certificates.X509KeyStorageFlags]::Exportable
$certificate = [System.Security.Cryptography.X509Certificates.X509Certificate2]::new($certPath, $credentials.Password, $flag)
$store.Open([System.Security.Cryptography.X509Certificates.OpenFlags]::ReadWrite)
$store.Add($Certificate)
$store.Close()
```

## <a name="sign-in-using-a-managed-identity"></a>Iniciar sessão com uma identidade gerida

As identidades geridas são uma funcionalidade do Azure Active Directory. As identidades geridas são principais de serviço atribuídos aos recursos que são executados no Azure. Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos. As identidades geridas só estão disponíveis em recursos em execução numa cloud do Azure.

A ligação deste exemplo é estabelecida através da identidade gerida do ambiente anfitrião. Por exemplo, se for executado numa VirtualMachine com uma Identidade de Serviço Gerida atribuída, permite ao código iniciar sessão com essa identidade atribuída.

```azurepowershell-interactive
 Connect-AzAccount -Identity
```

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a>Iniciar sessão com um inquilino não predefinido ou como um Fornecedor de Soluções Cloud (CSP)

Se a sua conta estiver associada a mais do que um inquilino, o início de sessão requer a especificação do parâmetro `-Tenant` durante a ligação. Este parâmetro funciona com qualquer método de início de sessão. Quando iniciar sessão, o valor deste parâmetro pode ser o ID de objeto do Azure do inquilino (ID de Inquilino) ou o nome de domínio completamente qualificado do inquilino.

Se for um [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/), o valor `-Tenant`**tem** de ser um ID de inquilino.

```azurepowershell-interactive
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>Iniciar sessão noutra Cloud

Os serviços cloud do Azure oferecem ambientes em conformidade com as leis de processamento de dados regionais. Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`. Este parâmetro funciona com qualquer método de início de sessão. Por exemplo, se a sua conta está na cloud da China:

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

O comando seguinte obtém uma lista dos ambientes disponíveis:

```azurepowershell-interactive
Get-AzEnvironment | Select-Object -Property Name
```
