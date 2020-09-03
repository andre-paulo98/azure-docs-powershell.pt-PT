---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/26/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 00cb5542e8d805f6e5e79e2177270fcbb93af808
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89241906"
---
# <a name="install-azure-powershell"></a><span data-ttu-id="6cc63-103">Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6cc63-103">Install Azure PowerShell</span></span>

<span data-ttu-id="6cc63-104">Este artigo explica como instalar os módulos do Azure PowerShell com o [PowerShellGet](/powershell/scripting/gallery/installing-psget).</span><span class="sxs-lookup"><span data-stu-id="6cc63-104">This article explains how to install the Azure PowerShell modules using [PowerShellGet](/powershell/scripting/gallery/installing-psget).</span></span> <span data-ttu-id="6cc63-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="6cc63-105">These instructions work on Windows, macOS, and Linux platforms.</span></span>

<span data-ttu-id="6cc63-106">O Azure PowerShell também está disponível no Azure [Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="6cc63-106">Azure PowerShell is also available in Azure [Cloud Shell](/azure/cloud-shell/overview).</span></span>

## <a name="requirements"></a><span data-ttu-id="6cc63-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="6cc63-107">Requirements</span></span>

<span data-ttu-id="6cc63-108">O Azure PowerShell funciona com o PowerShell 5.1 ou superior no Windows, ou com o PowerShell Core 6.x e posterior em todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="6cc63-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="6cc63-109">Deverá instalar a [versão mais recente do PowerShell](/powershell/scripting/install/installing-powershell) disponível para o seu sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="6cc63-109">You should install the [latest version of PowerShell](/powershell/scripting/install/installing-powershell) available for your operating system.</span></span> <span data-ttu-id="6cc63-110">O Azure PowerShell não tem requisitos adicionais quando é executado no PowerShell 6.2.4 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="6cc63-110">Azure PowerShell has no additional requirements when run on PowerShell 6.2.4 and later.</span></span>

<span data-ttu-id="6cc63-111">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="6cc63-111">To check your PowerShell version, run the command:</span></span>

```azurepowershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="6cc63-112">Para utilizar o Azure PowerShell no PowerShell 5.1 no Windows:</span><span class="sxs-lookup"><span data-stu-id="6cc63-112">To use Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="6cc63-113">Atualize para o [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="6cc63-113">Update to [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell).</span></span>
   <span data-ttu-id="6cc63-114">Se utilizar o Windows 10, versão 1607 ou superior, já tem o PowerShell 5.1 instalado.</span><span class="sxs-lookup"><span data-stu-id="6cc63-114">If you're on Windows 10 version 1607 or higher, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="6cc63-115">Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="6cc63-115">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>
3. <span data-ttu-id="6cc63-116">Verifique se tem a versão mais recente do PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="6cc63-116">Make sure you have the latest version of PowerShellGet.</span></span> <span data-ttu-id="6cc63-117">Execute `Install-Module -Name PowerShellGet -Force`.</span><span class="sxs-lookup"><span data-stu-id="6cc63-117">Run `Install-Module -Name PowerShellGet -Force`.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="6cc63-118">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6cc63-118">Install the Azure PowerShell module</span></span>

> [!WARNING]
> <span data-ttu-id="6cc63-119">Não suportamos os módulos do AzureRM e do Az instalados em simultâneo para o PowerShell 5.1 para Windows.</span><span class="sxs-lookup"><span data-stu-id="6cc63-119">We do not support having both the AzureRM and Az modules installed for PowerShell 5.1 on Windows at the same time.</span></span> <span data-ttu-id="6cc63-120">Se precisar de manter o AzureRM disponível no sistema, instale o módulo do Az para o PowerShell 6.2.4 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="6cc63-120">If you need to keep AzureRM available on your system, install the Az module for PowerShell 6.2.4 or later.</span></span>

<span data-ttu-id="6cc63-121">A utilização dos cmdlets do PowerShellGet é o método de instalação preferido.</span><span class="sxs-lookup"><span data-stu-id="6cc63-121">Using the PowerShellGet cmdlets is the preferred installation method.</span></span> <span data-ttu-id="6cc63-122">Instale o módulo do Az apenas no utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="6cc63-122">Install the Az module for the current user only.</span></span> <span data-ttu-id="6cc63-123">Este é o âmbito de instalação recomendado.</span><span class="sxs-lookup"><span data-stu-id="6cc63-123">This is the recommended installation scope.</span></span> <span data-ttu-id="6cc63-124">Este método funciona da mesma forma nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="6cc63-124">This method works the same on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="6cc63-125">Execute o seguinte comando a partir de uma sessão do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6cc63-125">Run the following command from a PowerShell session:</span></span>

```powershell-interactive
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Scope CurrentUser
}
```

<span data-ttu-id="6cc63-126">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="6cc63-126">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="6cc63-127">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="6cc63-127">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the `Set-PSRepository` cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="6cc63-128">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="6cc63-128">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="6cc63-129">A instalação do módulo para todos os utilizadores num sistema requer privilégios elevados.</span><span class="sxs-lookup"><span data-stu-id="6cc63-129">Installing the module for all users on a system requires elevated privileges.</span></span> <span data-ttu-id="6cc63-130">Inicie a sessão do PowerShell com a opção **Executar como administrador** no Windows ou utilize o comando `sudo` no macOS ou Linux:</span><span class="sxs-lookup"><span data-stu-id="6cc63-130">Start the PowerShell session using **Run as administrator** in Windows or use the `sudo` command on macOS or Linux:</span></span>

```powershell-interactive
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Scope AllUsers
}
```

<span data-ttu-id="6cc63-131">O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6cc63-131">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="6cc63-132">A instalação do mesmo transfere todos os módulos do Az do PowerShell em disponibilidade geral e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="6cc63-132">Installing it downloads all of the generally available Az PowerShell modules, and makes their cmdlets available for use.</span></span>

## <a name="install-offline"></a><span data-ttu-id="6cc63-133">Instalar offline</span><span class="sxs-lookup"><span data-stu-id="6cc63-133">Install offline</span></span>

<span data-ttu-id="6cc63-134">Em alguns ambientes, não é possível ligar à Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6cc63-134">In some environments, it's not possible to connect to the PowerShell Gallery.</span></span> <span data-ttu-id="6cc63-135">Nessas situações, ainda pode instalar offline através de um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="6cc63-135">In those situations, you can still install offline using one of these methods:</span></span>

* <span data-ttu-id="6cc63-136">Transfira os módulos para outra localização na sua rede e utilize-os como uma origem de instalação.</span><span class="sxs-lookup"><span data-stu-id="6cc63-136">Download the modules to another location in your network and use that as an installation source.</span></span>
  <span data-ttu-id="6cc63-137">Este método permite-lhe colocar em cache os módulos do PowerShell num único servidor ou que seja implementada a partilha de ficheiros através do PowerShellGet para quaisquer sistemas desligados.</span><span class="sxs-lookup"><span data-stu-id="6cc63-137">This method allows you to cache PowerShell modules on a single server or file share to be deployed with PowerShellGet to any disconnected systems.</span></span> <span data-ttu-id="6cc63-138">Saiba como configurar um repositório local e instalar em sistemas desligados com a opção [Trabalhar com repositórios do PowerShellGet locais](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span><span class="sxs-lookup"><span data-stu-id="6cc63-138">Learn how to set up a local repository and install on disconnected systems with [Working with local PowerShellGet repositories](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span></span>
* <span data-ttu-id="6cc63-139">[Transferira o MSI do Azure PowerShell](install-az-ps-msi.md) para um computador ligado a uma rede e, em seguida, copie o instalador para os sistemas sem o acesso à Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6cc63-139">[Download the Azure PowerShell MSI](install-az-ps-msi.md) to a machine connected to the network, and then copy the installer to systems without access to PowerShell Gallery.</span></span> <span data-ttu-id="6cc63-140">Tenha em mente que o instalador MSI funciona apenas para o PowerShell 5.1 no Windows.</span><span class="sxs-lookup"><span data-stu-id="6cc63-140">Keep in mind that the MSI installer only works for PowerShell 5.1 on Windows.</span></span>
* <span data-ttu-id="6cc63-141">Guarde o módulo com [Guardar-Módulo](/powershell/module/PowershellGet/Save-Module) numa partilha de ficheiros ou guarde noutra fonte e faça a cópia manualmente para outros computadores:</span><span class="sxs-lookup"><span data-stu-id="6cc63-141">Save the module with [Save-Module](/powershell/module/PowershellGet/Save-Module) to a file share, or save it to another source and manually copy it to other machines:</span></span>

  ```powershell-interactive
  Save-Module -Name Az -Path '\\server\share\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a><span data-ttu-id="6cc63-142">Resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="6cc63-142">Troubleshooting</span></span>

<span data-ttu-id="6cc63-143">Seguem-se alguns problemas comuns vistos durante a instalação do módulo do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6cc63-143">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="6cc63-144">Se detetar um problema não mencionado neste artigo, [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="6cc63-144">If you experience a problem not listed here, [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="6cc63-145">O proxy bloqueia a ligação</span><span class="sxs-lookup"><span data-stu-id="6cc63-145">Proxy blocks connection</span></span>

<span data-ttu-id="6cc63-146">Se ocorrerem erros de `Install-Module` que indiquem que a Galeria do PowerShell não está acessível, pode estar atrás de um proxy.</span><span class="sxs-lookup"><span data-stu-id="6cc63-146">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="6cc63-147">Diferentes sistemas operativos e ambientes de rede têm requisitos diferentes para configurar um proxy ao nível do sistema.</span><span class="sxs-lookup"><span data-stu-id="6cc63-147">Different operating systems and network environment have different requirements for configuring a system-wide proxy.</span></span> <span data-ttu-id="6cc63-148">Contacte o administrador de sistema para obter as suas definições de proxy e saber como configurá-las para o seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="6cc63-148">Contact your system administrator for your proxy settings and how to configure them for your environment.</span></span>

<span data-ttu-id="6cc63-149">O PowerShell não pode ser configurado para utilizar este proxy automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6cc63-149">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="6cc63-150">Com o PowerShell 5.1 e posterior, pode configurar a sessão do PowerShell para utilizar um proxy com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="6cc63-150">With PowerShell 5.1 and later, configure the PowerShell session to use a proxy using the following commands:</span></span>

```powershell
$webClient = New-Object System.Net.WebClient
$webClient.Proxy.Credentials = [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="6cc63-151">Se as credenciais do seu sistema operativo estiverem configuradas corretamente, esta configuração encaminha os pedidos do PowerShell através do proxy.</span><span class="sxs-lookup"><span data-stu-id="6cc63-151">If your operating system credentials are configured correctly, this configuration routes PowerShell requests through the proxy.</span></span> <span data-ttu-id="6cc63-152">Para manter esta definição entre sessões, adicione os comandos ao seu [perfil do PowerShell](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="6cc63-152">To have this setting persist between sessions, add the commands to your [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="6cc63-153">Para instalar o pacote, o proxy tem de permitir ligações HTTPS no seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="6cc63-153">To install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="6cc63-154">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="6cc63-154">Sign in</span></span>

<span data-ttu-id="6cc63-155">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6cc63-155">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
> <span data-ttu-id="6cc63-156">Se tiver desativado o carregamento automático do módulo, importe o módulo manualmente com `Import-Module -Name Az`.</span><span class="sxs-lookup"><span data-stu-id="6cc63-156">If you've disabled module autoloading, manually import the module with `Import-Module -Name Az`.</span></span>
> <span data-ttu-id="6cc63-157">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="6cc63-157">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="6cc63-158">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="6cc63-158">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="6cc63-159">Para saber como manter o início de sessão do Azure entre sessões do PowerShell, veja [Manter as credenciais do utilizador entre sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="6cc63-159">To learn how to persist your Azure sign in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="6cc63-160">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6cc63-160">Update the Azure PowerShell module</span></span>

<span data-ttu-id="6cc63-161">Para atualizar qualquer módulo do PowerShell, deve utilizar o mesmo método utilizado para instalar o módulo.</span><span class="sxs-lookup"><span data-stu-id="6cc63-161">To update any PowerShell module, you should use the same method used to install the module.</span></span> <span data-ttu-id="6cc63-162">Por exemplo, se utilizou originalmente `Install-Module`, deve utilizar [Update-Module](/powershell/module/powershellget/update-module) para obter a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="6cc63-162">For example, if you originally used `Install-Module`, then you should use [Update-Module](/powershell/module/powershellget/update-module) to get the latest version.</span></span> <span data-ttu-id="6cc63-163">Se utilizou originalmente o pacote MSI, deve transferir e instalar o novo pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="6cc63-163">If you originally used the MSI package then you should download and install the new MSI package.</span></span>

<span data-ttu-id="6cc63-164">Os cmdlets do PowerShellGet não conseguem atualizar os módulos instalados a partir de um pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="6cc63-164">The PowerShellGet cmdlets cannot update modules that were installed from an MSI package.</span></span> <span data-ttu-id="6cc63-165">Os pacotes MSI não atualizam os módulos instalados com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="6cc63-165">MSI packages do not update modules that were installed using PowerShellGet.</span></span> <span data-ttu-id="6cc63-166">Se tiver problemas ao utilizar o PowershellGet, deve **reinstalá-lo**, em vez de **o atualizar**.</span><span class="sxs-lookup"><span data-stu-id="6cc63-166">If you have any issues updating using PowershellGet, then you should **reinstall**, rather than **update**.</span></span> <span data-ttu-id="6cc63-167">A reinstalação é feita como a instalação, mas terá ter de adicionar o parâmetro `-Force`:</span><span class="sxs-lookup"><span data-stu-id="6cc63-167">Reinstalling is done the same way as installing, but you need to add the `-Force` parameter:</span></span>

```powershell
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Force
}
```

<span data-ttu-id="6cc63-168">Ao contrário das instalações baseadas em MSI, instalar ou atualizar com o PowerShellGet não remove as versões mais antigas que possam existir no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="6cc63-168">Unlike MSI-based installations, installing or updating using PowerShellGet does not remove older versions that may exist on your system.</span></span> <span data-ttu-id="6cc63-169">Para remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="6cc63-169">To remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span> <span data-ttu-id="6cc63-170">Para obter mais informações sobre instalações baseadas em MSI, veja [Instalar o Azure PowerShell com um MSI](install-az-ps-msi.md).</span><span class="sxs-lookup"><span data-stu-id="6cc63-170">For more information about MSI-based installations, see [Install Azure PowerShell with an MSI](install-az-ps-msi.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="6cc63-171">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6cc63-171">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="6cc63-172">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6cc63-172">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="6cc63-173">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="6cc63-173">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | Select-Object -Property Name, Version
```

<span data-ttu-id="6cc63-174">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="6cc63-174">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="6cc63-175">Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.</span><span class="sxs-lookup"><span data-stu-id="6cc63-175">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

<span data-ttu-id="6cc63-176">Pode instalar ou carregar uma versão específica do módulo `Az` com o parâmetro `-RequiredVersion`:</span><span class="sxs-lookup"><span data-stu-id="6cc63-176">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` parameter:</span></span>

```powershell-interactive
# Install Az version 3.6.1
Install-Module -Name Az -RequiredVersion 3.6.1
# Load Az version 3.6.1
Import-Module -Name Az -RequiredVersion 3.6.1
```

## <a name="provide-feedback"></a><span data-ttu-id="6cc63-177">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="6cc63-177">Provide feedback</span></span>

<span data-ttu-id="6cc63-178">Se encontrar um erro no Azure PowerShell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="6cc63-178">If you find a bug in Azure PowerShell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="6cc63-179">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="6cc63-179">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6cc63-180">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="6cc63-180">Next Steps</span></span>

<span data-ttu-id="6cc63-181">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="6cc63-181">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span> <span data-ttu-id="6cc63-182">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="6cc63-182">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
